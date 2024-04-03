<script>
	import ContactBar from '$lib/components/ContactBar.svelte';
	import ContentBox from '$lib/components/ContentBox.svelte';
	import Gallery from '$lib/components/Gallery.svelte';
	const galleryImages = [
		{
			src: 'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/modif 20-07-2023/Des-travaux-de-rénovation-exterieur-à-saint-malo.png',
			alt: 'Des travaux de rénovation exterieur à saint malo'
		},
		{
			src: 'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/modif 20-07-2023/équipement-de-maçonnorie-à-saint-malo02.png',
			alt: 'équipement de maçonnorie à saint malo02'
		},
		{
			src: 'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/modif 20-07-2023/équipement-de-travail-de-maçonnorie-à-saint-malo02.png',
			alt: 'équipement de travail de maçonnorie à saint malo02'
		},
		{
			src: "https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/modif 20-07-2023/Rénovation-intérieur-d'un-maison-à-Saint-Malo02.png",
			alt: "Rénovation intérieur d'un maison à Saint Malo02"
		},
		{
			src: 'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/media/cache/auto_tmb_600/userfiles/39524/modif 20-07-2023/Le--terrassement---à-saint-malo.png',
			alt: 'Le terrassement à saint malo'
		}
	];
</script>

<ContentBox title="Entreprise de maçonnerie à Saint-Malo" borderless centered>
	<div slot="text">
		<h2 class="exo dark">Confiez vos projets a sg maconnerie sur la cote d'emeraude</h2>
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

<ContentBox contrasted themed>
	<div slot="text">
		<h2 class="themed">
			Maçon Sur la cote d'emeraude<br /> —
		</h2>
		<p>Faites-moi part de vos <strong>travaux de maçonnerie</strong>.</p>

		<p>
			Mon <strong>entreprise de maçonnerie</strong> intervient dans les appartements, les villas et
			les maisons pour l’<strong>extension des murs</strong> ou la pose de cloisons.
		</p>

		<p>Vous pouvez me faire confiance pour le <strong>terrassement de votre terrain.</strong></p>

		<p>
			Préparation du sol, <strong>réhabilitation du terrain</strong>, fondation… Je suis à votre
			disposition.
		</p>

		<p>
			Je réalise également l’<strong>élévation des murs</strong>, pose de parrpaing, mur de
			soutainement, création de mur en pierre, pose de pillier de portail en different matériaux.
		</p>
	</div>
	<div class="gallery" slot="image">
		<img
			src="https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/media/cache/tmb_gallery_option/rc/TlvAsMBM/userfiles/39524/modif 20-07-2023/Aménagement-exterieur--à-saint-malo02.png"
			alt="Maconnerie"
		/>
		<img
			src="https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/media/cache/tmb_gallery_option/rc/1hkDxDBM/userfiles/39524/modif 20-07-2023/Travaux-de-terassement--à-saint-malo02.png"
			alt="Travaux de terassement à saint malo02"
		/>
	</div>
</ContentBox>

<Gallery images={galleryImages} />
<ContactBar>
	<p>Confiez-moi aussi vos travaux de <u>Maçonnerie.</u></p>
</ContactBar>

<style>
	h2,
	p {
		margin-bottom: 1rem;
	}
	.gallery {
		display: flex;
		margin-bottom: 6rem;
	}
	.gallery img {
		max-width: 50%;
	}
	.themed {
		color: var(--main-color);
	}
</style>
