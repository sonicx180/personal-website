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
		font-weight: var(--font-semi-bld);
		height:100%;
		margin-left: 20px;
	}
	h1 {
		flex: 1;
		line-height:1.5;
	}
	.logo {
		display: block;
		width: clamp(80px, 15vw, 160px);
		height: auto;
		object-fit: contain;
		border-radius: 8px;
		margin-right: 1.5rem;
	}
	.name,
	.sub-me {
		font-family: var(--font-mono);
	}
	@media screen and (max-width:400px) {
		.logo {
			display:none;
		}
		.hero {
			text-align:center;
		}
	}
</style>
