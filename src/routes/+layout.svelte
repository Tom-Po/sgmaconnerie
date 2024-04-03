<script>
	import Banner from '$lib/components/Banner.svelte';
	import Footer from '$lib/components/Footer.svelte';
	import Header from '$lib/components/Header.svelte';
	import '@fortawesome/fontawesome-free/css/all.min.css';
	import './styles.css';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
	<link href="https://fonts.googleapis.com/css?family=Exo|Oswald" rel="stylesheet" />
</svelte:head>

<Header />
<Banner />
<slot />
<Footer />

<style>
	@keyframes -global-pulse {
		0% {
			transform: scale(0);
			animation-timing-function: ease-in;
			opacity: 0;
		}
		38% {
			transform: scale(1);
			animation-timing-function: ease-out;
			opacity: 1;
		}
		55% {
			transform: scale(0.7);
			animation-timing-function: ease-in;
		}
		72% {
			transform: scale(1);
			animation-timing-function: ease-out;
		}
		81% {
			transform: scale(0.84);
			animation-timing-function: ease-in;
		}
		89% {
			transform: scale(1);
			animation-timing-function: ease-out;
		}
		95% {
			transform: scale(0.95);
			animation-timing-function: ease-in;
		}
		100% {
			transform: scale(1);
			animation-timing-function: ease-out;
		}
	}
</style>
