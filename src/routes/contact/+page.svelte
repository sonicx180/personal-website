<script>
import Contact from "../../components/Contact.svelte";
</script>

<main>
	<h1 class="contact-header">Contact Me</h1>
	<section class="info">
		<h3>You can reach me through the following:</h3>
		<div class="list">
			<Contact contact="gh" />
			<Contact contact="slack" />
		</div>
		
	</section>
</main>

<style>
	main {
		text-align: center;
	}
	.list {
		display:flex;
		flex-direction:column;
		gap:3rem;
	}
</style>
