<script>
	// export let name;

	import Hello from './components/hello.svelte'
	import UserView from './components/userView.svelte'
	import { Router, Link, Route } from "svelte-navigator";
	import Home from "./routes/Home.svelte";
	import Planning from "./routes/Plan.svelte";
</script>


<Router>
		<nav>
			<Link to="/">Home</Link>
			<Link to="/">User View</Link>
		</nav>
</Router>

<main>
	<UserView userName={'John'}/>
</main>


<style lang="scss">
	// $test-scss-var: palegreen;

	// main {
	// 	text-align: center;
	// 	padding: 1em;
	// 	max-width: 240px;
	// 	margin: 0 auto;
	// }

	// h1 {
	// 	color: $test-scss-var;
	// 	text-transform: uppercase;
	// 	font-size: 4em;
	// 	font-weight: 100;
	// }

	// @media (min-width: 640px) {
	// 	main {
	// 		max-width: none;
	// 	}
	// }

	// form {
	// 	background-color: blue;
	// 	height: 400px;
	// 	width: 500px;
	// }
</style>