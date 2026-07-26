<script lang="ts">
	import { page } from '$app/stores';
	
    let path = $state("");
	$effect(() => {
		const currentPage = $page.url.pathname + $page.url.hash;
        console.log(currentPage);
        path = currentPage;
        
	});
   
</script>

<nav class="navbar">
{#if path == "/#about"}
hi
{/if}
	<a href="/"> Home</a>
	<a href="/#about"> About</a>
	<a href="/projects"> Projects</a>
	<a href="/contact"> Contact</a>
</nav>

<style>
	.navbar {
		margin: 10px;
		margin-left: auto;
		font-family: var(--font-mono);
	}
	a {
		color: var(--accent-clr);
	}
</style>
