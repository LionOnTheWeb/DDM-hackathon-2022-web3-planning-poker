<script>
import Input from '../components/Input.svelte'
let current = "Add Ticket";
</script>

<div class = "inputs">
<Input label="Enter Name" placeholder="Enter your name..." />
<Input label="Room Name" placeholder="Enter room name..." />
<Input label="Planning Strategy" placeholder="Fibonacci Planning Poker Strategy" />
<Input label="Ticket Title" placeholder="Ticket title (e.g. DDM-1234...)" />
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