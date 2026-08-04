<script>
	const gh_light = '/logos/gh_light.png';
	const gh_dark = '/logos/gh_dark.png';
	const slack_light = '/logos/slack_light.png';
	import { onMount } from 'svelte';
	let { contact, info = 'sonicx180' } = $props();
	let link = '';
	let isDark = $state(false);

	if (contact == 'gh') {
		link = gh_light;
	} else if (contact == 'slack') {
		link = slack_light;
	}
</script>

<div class="contact">
	<a href="https://github.com/sonicx180" class="contact-link" target="_blank">
		<img src={link} alt="{info}'s {contact}" /> : {info}
	</a>
</div>

<style>
	.contact {
		display: flex;
		align-items: center;
		justify-content: center;
	}
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
		line-height: 1;
	}
	.contact-link:visited {
		color: var(--accent-clr);
	}
</style>
