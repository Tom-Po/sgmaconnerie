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
</script>

<ContentBox title="Entreprise de rénovation à Saint-Malo" borderless centered>
	<div slot="text">
		<h2 class="exo">
			Embellissez votre habitat avec votre spécialiste en travaux de rénovation sur la cote
			d'emeraude
		</h2>
		<p>
			<a class="inherit-links" href="http://www.sgmaconnerie.fr/"
				><u><strong>SG Maçonnerie</strong></u></a
			>
			est le partenaire qu’il vous faut à Saint-Malo pour la <strong>rénovation </strong>intérieure
			et extérieure<strong> de votre habitation</strong>.
		</p>

		<p>
			<strong>Rejointoiement de vos murs</strong>,
			<strong>agrandissement de pièces de vies, ouverture de murs porteurs</strong>… Je réalise vos
			travaux de A à Z.
		</p>

		<p>Faites-moi confiance pour la rénovation de votre terrasse.&nbsp;</p>

		<p>Tout est réalisé en fonction de votre budget et de vos envies.&nbsp;</p>
	</div>
</ContentBox>

<ContentBox contrasted themed>
	<div slot="text">
		<h2 class="themed">
			Travaux de Rénovation d’habitats à Saint-malo et sa cote.<br /> —
		</h2>
		<p>Confiez-moi la rénovation de votre bien immobilier.</p>

		<p>
			Pour sublimer votre extérieur, j'effectue le <strong>rejointoiement</strong> à la chaux de vos
			murs, pose d'<strong>enduits</strong> (finition grattée, taloché...) à la chaux.
		</p>

		<p>
			Je suis en mesure de <strong>refaire le carrelage</strong> de votre intérieur comme extérieur.
		</p>

		<p>
			Je réalise vos <strong>ouvertures</strong> sur mur porteur, avec pose de
			<strong>linteaux</strong>
			en béton ou<strong> IPN.</strong> Je m'occupe également de la fermeture des
			<strong>ouvertures</strong> (fenêtre, porte), en pierre ou parpaing
		</p>
	</div>
	<div slot="image">
		<img
			src="https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/modif%2020-07-2023/Travaux-de-r%C3%A9novation-%C3%A0-saint-malo02.png"
			alt="Rénovation"
		/>
	</div>
</ContentBox>

<Gallery images={galleryImages} />
<ContactBar>
	<p>
		Pour répondre à tous vos besoins, je me charge de vos travaux de <u>maçonnerie générale</u>.
	</p>
</ContactBar>

<style>
	h2 {
		color: var(--black);
		font-size: 30px;
	}
	h2,
	p {
		margin-bottom: 1rem;
	}

	.themed {
		color: var(--main-color);
	}
</style>
