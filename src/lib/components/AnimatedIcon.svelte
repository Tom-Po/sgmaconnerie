<script lang="ts">
	export let src = '';
	export let title = '';
	export let link = '';
	let animated = false;

	const options = {};
	function actionWhenInViewport(e: any) {
		const observer = new IntersectionObserver((entries) => {
			if (entries[0].isIntersecting) {
				// element in viewport
				observer.disconnect();
				animated = true;
			}
		}, options);

		observer.observe(e);
	}
</script>

<article class:animated use:actionWhenInViewport>
	<a href={link}><img alt="exp" {src} /></a>
	<a class="exo" href={link}>{title}</a>
</article>

<style>
	article {
		display: flex;
		flex-basis: 33%;
		flex-direction: column;
		opacity: 0;
		transition: all 200ms 500ms ease-in-out;
	}
	.animated {
		opacity: 1;
		transition-delay: opacity 1s;
		animation: pulse 1s 0.5s forwards;
	}
	article:hover img {
		opacity: 0.7;
		transform: translateY(-10px);
		transition: all 200ms ease-in-out;
	}
	a {
		color: var(--main-color);
	}
</style>
