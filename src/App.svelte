<script>
<<<<<<< HEAD
	// export let name;

	import Hello from './components/hello.svelte'
	import UserView from './components/userView.svelte'
=======
>>>>>>> main
	import { Router, Link, Route } from "svelte-navigator";

	import Layout from "./components/Layout.svelte";
	import Nav from "./components/Nav.svelte";
	import Home from "./routes/Home.svelte";
	import UserView from "./routes/User.svelte";
	import FacilitatorView from "./routes/Facilitator.svelte";
	import Planning from "./routes/Plan.svelte";
<<<<<<< HEAD
	import userView from "./routes/userView.svelte";
=======

	let navItems = [
		{
			title: "Home",
			location: "/",
			component: Home
		},
		{
			title: "Planning",
			location: "/planning",
			component: Planning
		},
		// {
		// 	title: "Login",
		// 	location: "/login",
		// 	class: "login"
		// },
		{
			title: "User",
			location: "/user",
			component: UserView,
			class: "login"
		}, 
		{
			title: "Facilitator",
			location: "/facilitator",
			component: FacilitatorView
		}
	]
>>>>>>> main
</script>


<Router>
<<<<<<< HEAD
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
=======
		<Nav navItems={navItems}/>
		<Layout>
			{#if navItems}
				{#each navItems as navItem}
					<Route path="{navItem.location}" component={navItem.component}/>
				{/each}
			{/if}
		</Layout>
</Router>
>>>>>>> main
