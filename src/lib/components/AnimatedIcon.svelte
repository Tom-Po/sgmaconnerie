<script>
	export let src = '';
	export let title = '';
	export let link = '';
</script>

<article>
	<a href={link}><img alt="exp" {src} /></a>
	<a class="exo" href={link}>{title}</a>
</article>

<style>
	article {
		display: flex;
		flex-basis: 33%;
		flex-direction: column;
		animation: pulse 1s forwards;
	}
	article:hover img {
		opacity: 0.7;
		transform: translateY(-10px);
		transition: all 200ms ease-in-out;
	}
	a {
		color: var(--main-color);
	}

	@keyframes pulse {
		0% {
			transform: scale(1, 1);
		}

		50% {
			transform: scale(1.1, 1.1);
		}

		100% {
			transform: scale(1, 1);
		}
	}
</style>
