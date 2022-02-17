<script>
	export let name;

	import Hello from './components/hello.svelte'
</script>

<main>
	<Hello msg={'DDM Planning Poker Team!'}/>
	<h1>and hello {name}</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
	<form>
	<input type="text"/>
	</form>
</main>


<style lang="scss">
	$test-scss-var: palegreen;

	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: $test-scss-var;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}

	form {
		background-color: blue;
		height: 400px;
		width: 500px;
	}
</style>