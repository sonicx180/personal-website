<script lang="ts">
	import '../app.css';
	import Navbar from '../components/Navbar.svelte';
	import Footer from '../components/Footer.svelte';
	let { children } = $props();
</script>

<svelte:head>
	<title>Cheta Nzeogu | Sonicx180</title>
	<link rel="icon" href="/logo.png" type="image/png" />
</svelte:head>

<Navbar />
{@render children()}
<Footer />
