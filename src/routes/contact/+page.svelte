<script>
import Contact from "../../components/Contact.svelte";
</script>

<main>
	<h1 class="contact-header">Contact Me</h1>
	<section class="info">
		<h3>You can reach me through the following:</h3>
		<div class="list">
			<Contact contact="gh" link="https://github.com/sonicx180" />
			<Contact contact="slack" link="https://hackclub.slack.com"/>
			<Contact contact="discord" link="https://discord.com/users/1051295490358128662"/>
			<Contact contact="linkedin" link="https://linkedin.com/in/cheta-nzeogu" info="Cheta Nzeogu"/>
		</div>
		
	</section>
</main>

<style>
	main {
		text-align: center;
	}
	.list {
		display:grid;
		grid-template-columns:1fr ;
		gap:1.5rem;
	}
	@media screen and (min-width:500px) {
		.list {
			grid-template-columns: 1fr 1fr;
		}
	}
</style>
