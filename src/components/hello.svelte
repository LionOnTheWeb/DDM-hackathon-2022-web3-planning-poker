	<script>
  export let msg;

  import Input from './Input.svelte'
  </script>

  <h1>Hello {msg}!</h1>
  <Input type="text" label="Facilitator"/>

<style lang="scss">

	h1 {
		color: $primary-blue;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}
</style>