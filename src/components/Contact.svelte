<script lang="ts">
	const gh_light = '/logos/gh_light.png';
	const gh_dark = '/logos/gh_dark.png';
	const slack_light = '/logos/slack_light.png';
	const discord_light = '/logos/discord.png';
	const linkedin = '/logos/linkedin.png';
	import { onMount } from 'svelte';
	let { contact, info = 'sonicx180', link } = $props();
	let img = '';
	let isDark = $state(false);

	if (contact == 'gh') {
		img = gh_light;
	} else if (contact == 'slack') {
		img = slack_light;
	}
	else if (contact == 'discord') {
		img = discord_light;
	}
	else {
		img = linkedin;
	}

</script>

<div class="contact">
	<a href={link} class="contact-link" target="_blank">
		<img src={img} alt="{info}'s {contact}" /> : {info}
	</a>
</div>

<style>
	img {
		width: clamp(30px, 5vw, 600px);
		display: inline-block;
		vertical-align: middle;
		border-radius: 8px;
	}
	.contact-link {
		display: inline-flex;
		align-items: center;
		gap: 0.35rem;
		line-height: 1.5;
	}
	@media screen and (max-width:500px) {
		img {
			width:40px;
		}
	}
</style>
