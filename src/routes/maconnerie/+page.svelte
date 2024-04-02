<script>
	import ContactBar from '$lib/components/ContactBar.svelte';
	import ContentBox from '$lib/components/ContentBox.svelte';
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
		},
		{
			id: 4,
			src: 'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/media/cache/auto_tmb_600/userfiles/39524/modif 20-07-2023/Le--terrassement---à-saint-malo.png',
			alt: 'Le terrassement à saint malo'
		}
	];
</script>

<ContentBox title="Entreprise de maçonnerie à Saint-Malo" borderless>
	<div slot="text">
		<h2>Confiez vos projets a sg maconnerie sur la cote d'emeraude</h2>
		<p>
			<a class="inherit-links" href="http://www.sgmaconnerie.fr/"
				><u><strong>SG Maçonnerie</strong></u></a
			> est à votre service à Saint-Malo et aux alentours.
		</p>

		<p>
			Je m’occupe de votre <strong>projet de construction,&nbsp;</strong>que vous soyez à
			Saint-Malo, Cancale, Saint-Briac...
		</p>

		<p>
			De la <strong>pose de dalles</strong> à la <strong>création d’ouvertures</strong>, je vous
			accompagne dans l’ensemble de vos travaux.
		</p>
	</div>
</ContentBox>

<Gallery images={galleryImages} />
<ContactBar>
	<p>Confiez-moi aussi vos travaux de <u>Maçonnerie.</u></p>
</ContactBar>
