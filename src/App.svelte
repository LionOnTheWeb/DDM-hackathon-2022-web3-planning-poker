<script>
	// export let name;

	import Hello from './components/hello.svelte'
	import UserView from './components/userView.svelte'
	import { Router, Link, Route } from "svelte-navigator";
	import Home from "./routes/Home.svelte";
	import Planning from "./routes/Plan.svelte";
	import userView from "./routes/userView.svelte";
</script>


<Router>
		<nav class="nav">
			<Link to="/">Home</Link>
			<Link to="/planning">Planning</Link>
			<Link class="login" to="/login">Login</Link>
			<Link to="/userView">userView</Link>
		</nav>
		<div>
			<Route path="/">
				<Home/>
			</Route>
			<Route path="planning" component={Planning}/>
			<Route path="userView" component={userView}/>
		</div>
</Router>


<style lang="scss">

</style>