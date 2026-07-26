<script>
	import Typewriter from 'svelte-typewriter';
</script>

<div class="hero">
	<h1>
		<span class="pre"> Hey, it's </span> <br />
		<span class="name">
			Cheta Nzeogu <span class="accent">(Sonicx180) </span></span
		> <br />
		<Typewriter mode="loop" wordInterval={2500}>
			<span class="me">
				I like <span class="sub-me accent">building for the web </span>
			</span>
			<span class="me">
				I'm an aspiring <span class="sub-me accent"
					>Software Developer
				</span></span
			>
			<span class="me">
				I'm a <span class="sub-me accent">student </span></span
			>
		</Typewriter>
	</h1>
	<img src="/logo.png" alt="My logo" class="logo" />
</div>

<style>
	.hero {
		display: flex;
		align-items: center;
		flex-wrap: wrap;
		 gap: clamp(0.75rem, 10vw, 10rem);
		font-weight: var(--font-semi-bld);
		margin-left: 20px;
	}
	.logo {
		display:block;
		width: clamp(80px, 12vw, 160px);
		height: auto;
		object-fit:contain;
		border-radius:8px;
	}
	.name,
	.sub-me {
		font-family: var(--font-mono);
	}
</style>
