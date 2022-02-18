<script>
import Layout from '../components/Layout.svelte'
import Input from '../components/Input.svelte'
let current = "Add Ticket";
let msg = "";
</script>

<h1>Home Route</h1>
<div class = "inputs">

<Input bind:value={msg} placeholder="Enter your name..." />
<p>Welcome {msg} </p>
<Input placeholder="Enter room name..." />
<Input placeholder="Fibonacci" />
<Input placeholder="Ticket" />
</div>

<button
	class:selected="{current === 'Add Ticket'}"
	on:click="{() => current = 'Add Ticket'}"
>Add Ticket</button>

<style>
.inputs {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  height: auto;
  text-align:center;
}

:global(.inputs input) {
  padding: 10px;
  width: auto;
  margin: 8px 8%;
}
	
</style>