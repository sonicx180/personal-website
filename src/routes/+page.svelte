<script lang="ts">
	import Hero from '../components/Hero.svelte';
</script>

<main>
	<Hero />
	<hr />
	<section id="about">
		<h2>About Me</h2>
		<p>I'm a teen dev that is interested in learning more about practically anything in the <span class = "accent"> swe </span> side of things.</p>
		<p> I started coding back in 2021, and since then have made some pretty simple projects.</p>
	</section>
</main>

<style>
	#about {
		text-align: center;
	}

	hr {
		width:75%;
	}
</style>
