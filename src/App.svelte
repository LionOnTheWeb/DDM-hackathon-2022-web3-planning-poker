<script>
	// export let name;

	import Hello from './components/hello.svelte'
	import { Router, Link, Route } from "svelte-navigator";
	import Home from "./routes/Home.svelte";
	import Planning from "./routes/Plan.svelte";
</script>


<Router>
		<nav>
			<Link to="/">Home</Link>
			<Link to="/planning">Planning</Link>
		</nav>
		<div>
			<Route path="/">
				<Home/>
			</Route>
			<Route path="planning">
				<Planning/>
			</Route>
		</div>
</Router>


<style lang="scss">

</style>