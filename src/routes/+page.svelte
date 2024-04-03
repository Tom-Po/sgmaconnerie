<script>
	import ContactBar from '$lib/components/ContactBar.svelte';
	import Gallery from '$lib/components/Gallery.svelte';
	import HomeContent from '$lib/components/HomeContent.svelte';
	const galleryImages = [
		{
			id: 0,
			src: 'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/media/cache/tmb_gallery_option/rc/Kw5n7oci/userfiles/39524/modif 20-07-2023/Transformez-votre-espace-extérieur-avec-un-maçon-qualifié-à-Saint-Malo..png',
			alt: 'Des travaux de rénovation exterieur à saint malo'
		},
		{
			id: 1,
			src: 'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/media/cache/tmb_gallery_option/rc/BRvPEtsB/userfiles/39524/modif 20-07-2023/Des-services-de-maçonnerie-générale-à-saint-malo.png',
			alt: 'équipement de maçonnorie à saint malo02'
		},
		{
			id: 2,
			src: 'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/media/cache/tmb_gallery_option/rc/vPcnGCnC/userfiles/39524/modif 20-07-2023/Des-services-de-maçonnerie-générale-de-qualité-pour-toutes-les-projets-résidentiels-à-Saint-Malo..png',
			alt: 'équipement de travail de maçonnorie à saint malo02'
		},
		{
			id: 3,
			src: "https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/media/cache/tmb_gallery_option/rc/vH0v3eYd/userfiles/39524/modif 20-07-2023/Rénovation-éxterieur-d'un-maison-à-Saint-Malo..png",
			alt: "Rénovation intérieur d'un maison à Saint Malo02"
		}
	];
</script>

<HomeContent />
<Gallery images={galleryImages} />
<ContactBar>
	<p>N’hésitez pas à me contacter pour plus de renseignements sur mes préstations.</p>
</ContactBar>
