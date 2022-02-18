	<script>
  export let msg;

  import Input from './Input.svelte'
  import Image from './image.svelte'
  </script>

  <h1>Hello {msg}!</h1>
  <Input type="text" label="Facilitator"/>
  <Image alt = "test"/>
<style >

	h1 {
		color: green;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}
</style>