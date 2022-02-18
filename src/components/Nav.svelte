<script>
  export let navItems = [];

  import { Link } from "svelte-navigator";
</script>

<nav class="nav">
  {#if navItems}
    {#each navItems as navItem}
      <Link to="{navItem.location}" class="{navItem.class}">{navItem.title}</Link>
    {/each}
  {/if}
</nav>

<style lang="scss">
	.nav {
		font-size: 16px;
		display: flex;
    background: $nav-background-color;
	}

	:global(.nav .login) {
		margin-left: auto;
		padding-right: 8px;
		color: $nav-font-color;
	}

	:global(.nav a) {
		color: $nav-font-color;
		padding: 12px 8px;
	}

	:global(.nav a:hover) {
		color: $nav-font-color-hover;
		text-decoration: none;
	}
</style>