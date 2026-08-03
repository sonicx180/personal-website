<script>
	const gh_light = '/logos/gh_light.png';
	const gh_dark = '/logos/gh_dark.png';
    import {onMount} from 'svelte'

    let isDark = $state(false);


</script>

<div class="contact">
	<a href="https://github.com/sonicx180" class="gh">
		<img src={gh_light} alt="github logo" /> : Sonicx180
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
        vertical-align:middle;
	}
	.gh {
		display:inline-flex;
        align-items:center;
        gap:0.35rem;
        line-height:1;
	}
</style>
