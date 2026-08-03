<script lang="ts">
	import { page } from '$app/stores';

	let path = $state('');

	$effect(() => {
		const currentPage = $page.url.pathname + $page.url.hash;
		/* console.log(currentPage); */
		path = currentPage;
	});
</script>

<nav class="navbar">
	<a href="/" class:active={path === '/'}> Home</a>
	<a href="/#about" class:active={path === '/#about'}> About</a>
	<a href="/projects" class:active={path === '/projects'}> Projects</a>
	<a href="/contact" class:active={path === '/contact'}> Contact</a>
</nav>

<style>
	a {
		color: var(--accent-clr);
	}
	.navbar {
		margin: 10px;
		margin-left: auto;
		font-family: var(--font-mono);
	}
	.active {
		color: var(--teritary-clr);
	}
	a:hover,
	a:active {
		color: var(--teritary-clr);
	}
	@media screen and (max-width: 400px) {
		.navbar {
			margin: 0;
			margin-top: 5px;
			text-align: center;
		}
	}
</style>
