<script>
	import ContactBar from '$lib/components/ContactBar.svelte';
	import ContentBox from '$lib/components/ContentBox.svelte';
	import Gallery from '$lib/components/Gallery.svelte';

	const galleryImages = [
		{
			id: 0,
			src: 'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/media/cache/auto_tmb_600/userfiles/39524/modif 20-07-2023/Rénovation-intérieur-de-maisonà-saint-malo.png',
			alt: 'Rénovation maison Saint Malo'
		},
		{
			id: 1,
			src: 'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/media/cache/auto_tmb_600/userfiles/39524/modif 20-07-2023/Des-services-de-rénovation-exterieur-de-maison-à-Saint-Malo..png',
			alt: 'Rénovation maison Saint Malo'
		},
		{
			id: 2,
			src: 'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/media/cache/auto_tmb_600/userfiles/39524/modif 20-07-2023/Maçonnerie-générale-et-rénovation-à-Saint-Malo..png',
			alt: 'Rénovation maison Saint Malo'
		},
		{
			id: 3,
			src: "https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/media/cache/auto_tmb_600/userfiles/39524/modif 20-07-2023/Maçonnorie-et-rénovation-exterieur-d'un-maison--à-saint-malo.png",
			alt: 'Rénovation maison Saint Malo'
		},
		{
			id: 0,
			src: 'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/media/cache/auto_tmb_600/userfiles/39524/modif 20-07-2023/Rénovation-intérieur-de-maisonà-saint-malo.png',
			alt: 'Rénovation maison Saint Malo'
		}
	];
	const galleryImagesRenov = [
		{
			id: 0,
			src: "https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/media/cache/tmb_gallery_option/rc/6MsA9kkN/userfiles/39524/modif%2020-07-2023/R%C3%A9novation-d'espace-exterieur-%C3%A0-saint-malo.png",
			alt: 'Rénovation maison Saint Malo'
		},
		{
			id: 2,
			src: 'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/media/cache/tmb_gallery_option/rc/w9ouJFTb/userfiles/39524/modif 20-07-2023/Des-rénovations-exterieurs--à-Saint-Malo..png',
			alt: 'Rénovation maison Saint Malo'
		},
		{
			id: 3,
			src: "https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/media/cache/tmb_gallery_option/rc/49KmvkiX/userfiles/39524/modif 20-07-2023/Une-rénovation-intérieur-d'un-maison-à-Saint-Malo.png",
			alt: 'Rénovation maison Saint Malo'
		},
		{
			id: 0,
			src: 'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/media/cache/tmb_gallery_option/rc/C8rfd1SX/userfiles/39524/modif 20-07-2023/Travaux-de-rénovation-exterieur-et-de-maçonnerie-à-saint-malo.png',
			alt: 'Rénovation maison Saint Malo'
		}
	];
</script>

<ContentBox title="La galerie photos de votre maçon à Saint-Malo" borderless centered>
	<div slot="text">
		<h2 class="exo">
			Découvrez en images mes réalisations en maçonnerie et rénovation d’habitats en Ille-et-Vilaine
		</h2>
		<p>
			Consultez la galerie photos de <a href="/maconnerie"><u><strong>SG Maçonnerie</strong></u></a>
			à Saint-Malo.
		</p>
	</div>
</ContentBox>

<ContentBox title="MAÇONNERIE GÉNÉRALE a saint-malo" borderless></ContentBox>
<Gallery images={galleryImages} />

<ContentBox title="Travaux de RÉNOVATION " borderless></ContentBox>
<div class="gallery-wrapper">
	<Gallery images={galleryImagesRenov} />
</div>

<ContactBar />

<style>
	.gallery-wrapper {
		max-width: 60%;
		margin: 0 auto;
	}
	h2 {
		margin-bottom: 2rem;
	}
</style>
