<script>
	import ContactBar from '$lib/components/ContactBar.svelte';
	import Content from '$lib/components/Content.svelte';
	import Gallery from '$lib/components/Gallery.svelte';
	const galleryImages = [
		{
			id: 0,
			src: 'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/modif 20-07-2023/Des-travaux-de-rénovation-exterieur-à-saint-malo.png',
			alt: 'Des travaux de rénovation exterieur à saint malo'
		},
		{
			id: 1,
			src: 'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/modif 20-07-2023/équipement-de-maçonnorie-à-saint-malo02.png',
			alt: 'équipement de maçonnorie à saint malo02'
		},
		{
			id: 2,
			src: 'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/modif 20-07-2023/équipement-de-travail-de-maçonnorie-à-saint-malo02.png',
			alt: 'équipement de travail de maçonnorie à saint malo02'
		},
		{
			id: 3,
			src: "https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/modif 20-07-2023/Rénovation-intérieur-d'un-maison-à-Saint-Malo02.png",
			alt: "Rénovation intérieur d'un maison à Saint Malo02"
		}
	];
</script>

<Content />
<Gallery images={galleryImages} />
<ContactBar>
	<p>N’hésitez pas à me contacter pour plus de renseignements sur mes préstations.</p>
</ContactBar>

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
