<script>
	import { Router, Link, Route } from "svelte-navigator";

	import Layout from "./components/Layout.svelte";
	import Nav from "./components/Nav.svelte";
	import Home from "./routes/Home.svelte";
	import UserView from "./routes/User.svelte";
	import Planning from "./routes/Plan.svelte";

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
		{
			title: "Login",
			location: "/login",
			class: "login"
		},
		{
			title: "User",
			location: "/user"
		}, 
		{
			title: "Facilitator",
			location: "/facilitator"
		}
	]
</script>


<Router>
		<Nav navItems={navItems}/>
		<Layout>
			{#if navItems}
				{#each navItems as navItem}
					<Route path="{navItem.location}" component={navItem.component}/>
				{/each}
			{/if}
		</Layout>
</Router>