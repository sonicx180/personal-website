<script lang="ts">
	import Hero from '../components/Hero.svelte';
</script>

<main>
	<Hero />
	<hr />
	<section id="about">
		<h2>About Me</h2>
		<p>
			I'm a teen dev that is interested in learning more about practically
			anything in the <span class="accent"> swe </span> side of things. I
			started coding back in 2021, and since then have made quite a few
			<a href="/projects" class="accent"> projects </a>. For now, I'm a
			full time student that's looking to continue building software in my
			free time, learn more programming languages, and immerse myself
			further in the tech industry.
		</p>
		<h2>Need to reach out?</h2>
		<p>Head over to my <a href="/contact" class = "accent">contact page</a>!</p>
	</section>
</main>

<style>
	#about {
		text-align: center;
	}
	#about a {
		text-decoration: underline;
		text-decoration-thickness: 3px;
	}
	#about a:hover,
	#about a:active {
		color: var(--teritary-clr);
	}
	hr {
		width: 75%;
	}
	p {
		line-height: 1.5;
		margin:5px;
	}
</style>
