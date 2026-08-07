<script>
</script>

<main>
	<section class="top">
		<h1>Projects</h1>
		<p>You can view some of my projects here</p>
	</section>
	<section class="projects">
		<div class="projects-grid">
			<div class="project">
				<img alt="Screenshot of FindYourCut" />
				<a href="https://findyourcut.vercel.app" target="_blank"
					><h3>FindYourCut</h3>
				</a>
				<p>
					A website made to find haircuts. Looking back this is one of
					the worst looking sites I've made.
				</p>
				<p>I built this mid 2025</p>
			</div>
			<div class="project">
				<img alt="Screenshot of Ginz & Associates" />
				<a href="https://ginz-associates.us" target="_blank"
					><h3>Ginz & Associates</h3>
				</a>

				<p>A website made for my dad for his business. Not official.</p>
				<p>I built this in the winter of 2025</p>
			</div>
			<div class="project">
				<img alt="Screenshot of Pokebot in use" />
				<a href="https://github.com/sonicx180/pokebot" target="_blank"
					><h3>Pokebot</h3></a
				>
				<p>
					Slack bot that gives information on pokemon. This is only
					avaliable on the Hack Club Slack for now.
				</p>
				<p>
					I built this in the summer of 2026 to learn how to build
					slack bots
				</p>
			</div>
		</div>
	</section>
</main>

<style>
	main {
		text-align: center;
	}
	.projects {
		margin: 5px;
	}
	.projects-grid {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
		gap: 1rem;
	}
	.project {
		border: 3px solid var(--border-clr);
		border-radius: 8px;
		padding: 10px;
	}
	.project > a,
	.project > a:visited {
		color: var(--secondary-clr);
		text-decoration: underline;
	}
</style>
