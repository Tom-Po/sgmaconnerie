<script>
	import Banner from '$lib/components/Banner.svelte';
	import Content from '$lib/components/Content.svelte';
	import Header from './Header.svelte';
	import './styles.css';
</script>

<svelte:head>
	<link href="https://fonts.googleapis.com/css?family=Exo|Oswald" rel="stylesheet" />
</svelte:head>
<Header />

<Banner />
<Content />
