<script>
	import Maconnerie from '$lib/images/maconnerie.png';
	import AnimatedIcon from './AnimatedIcon.svelte';
	import ContentBox from './ContentBox.svelte';
</script>

<ContentBox title="Maçon professionnel à Saint-Malo">
	<div slot="text">
		<h2 class="exo">Travaux de maçonnerie et de rénovation en Ille-et-Vilaine</h2>
		<p>
			<strong>SG Maçonnerie</strong> à Saint-Malo est une entreprise de<strong
				>&nbsp;maçonnerie</strong
			> est au service des particuliers.
		</p>

		<p>
			Je m’occupe de votre <strong>projet de rénovation</strong> et de
			<strong>construction </strong>avec rigueur et professionnalisme.
		</p>

		<p>
			De la <strong>création d’ouvertures</strong> au
			<strong>rejointoiement des pierres de vos murs</strong>, je vous accompagne étape par étape
			dans vos travaux.
		</p>

		<p>
			Confiez-moi aussi votre projet de <strong>terrassement</strong> pour la création de&nbsp;&nbsp;Dalle
			béton, Fondation...
		</p>

		<p>
			Avec 10 ans d’expérience dans le domaine de la maçonnerie, je vous garantis des prestations de
			qualité.
		</p>
	</div>
	<div slot="image">
		<img src={Maconnerie} alt="Maconnerie" />
	</div>
</ContentBox>

<div class="icons">
	<AnimatedIcon
		title="Maçonnerie générale"
		link="/maconnerie"
		src="https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/maconeriei.png"
	/>
	<AnimatedIcon
		title="Rénovation"
		link="/renovation"
		src="https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/renovation.png"
	/>
	<AnimatedIcon
		title="Mes réalisations"
		link="/realisations"
		src="https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/galerie.png"
	/>
</div>

<ContentBox borderless contrasted>
	<div slot="text">
		<h3>Entreprise de maçonnerie et de rénovation A SAINT-MALO ET SA COTE <br /> —</h3>

		<p>Je vous propose différentes prestations en <strong>maçonnerie générale</strong>.</p>

		<p>
			<strong>Élévation des murs, création de terrasses</strong>,<strong>
				Fondation, Création de mur de clôture</strong
			>… Je suis à votre disposition.
		</p>

		<p>Je me charge de l’extension et de l’agrandissement des pièces de vie.</p>

		<p>
			<strong>Terrassier à Saint Malo,&nbsp; et sa côte d'Émeraude</strong>, je réalise la
			<strong>réhabilitation de sols</strong>, le <strong>nivellement</strong> et la
			<strong>fondation</strong>.
		</p>

		<p>Tout est effectué selon le type et la nature de votre terrain.</p>

		<p>J’interviens également pour la rénovation de votre habitat.</p>

		<p>
			De la <strong>pose de carrelage</strong>&nbsp;au<strong> Dallage</strong> de votre sol, ainsi
			qu'au <strong>rejointoiement</strong> de vos murs. Je vous assure des travaux dans les règles de
			l'art.
		</p>
	</div>
	<div slot="image">
		<img
			src="https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/modif%2020-07-2023/Entreprise-de-ma%C3%A7onnerie-et-de-r%C3%A9novation-%C3%A0-saint-malo.png"
			alt="Maconnerie"
		/>
	</div>
</ContentBox>

<div class="content">
	<h3 style="text-align: center">Mes garanties en travaux de rénovation près de Dinan</h3>
	<p style="text-align: center">Maçon en Ille-et-Vilaine, je vous assure:</p>
	<div class="icons">
		<article>
			<p>
				<img
					alt="exp"
					src="https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/exp.png"
				/>
			</p>
			<p>La qualité des travaux</p>
		</article>
		<article>
			<p>
				<img
					alt="Le sérieux"
					src="https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/Le-s%C3%A9rieux.png"
				/>
			</p>

			<p>Le sérieux</p>
		</article>
		<article>
			<p>
				<img
					alt="a disponibilité"
					src="https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/a-disponibilit%C3%A9.png"
				/>
			</p>

			<p>La disponibilité</p>
		</article>
		<article>
			<p>
				<img
					alt="qualité"
					src="https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/qualit%C3%A9.png"
				/>
			</p>

			<p>L’expérience</p>
		</article>
	</div>
</div>

<div class="content">
	<h3>Zone d’intervention de votre expert en maçonnerie</h3>
	<article>
		<p>
			Pour réaliser vos <strong>travaux de maçonnerie</strong> et <strong>de rénovation</strong>, je
			me déplace dans un rayon de 40 km autour de Saint-Malo&nbsp;:
		</p>

		<ul class="with-list">
			<li>Saint-Malo</li>
			<li>Dinard</li>
			<li>Saint-Briac-sur-Mer&nbsp;</li>
			<li>Cancale</li>
			<li>Lancieux&nbsp;</li>
			<li>Dinan</li>
			<li>Dol-de-Bretagne</li>
			<li>Saint-Jouan-des-Guérets</li>
			<li>Saint-Méloir-des-Ondes</li>
			<li>Saint-Coulomb</li>
		</ul>
	</article>
</div>

<style>
	h2,
	h3 {
		font-size: 1.8rem;
	}
	p {
		margin-bottom: 0.5rem;
	}

	.exo {
		margin-bottom: 1rem;
		text-transform: uppercase;
	}

	.icons {
		display: flex;
		justify-content: center;
		text-align: center;
		gap: 3.5rem;
		padding: 2rem;
		width: 66%;
		margin: 0 auto;
	}
	.icons article {
		display: flex;
		flex-basis: 33%;
		flex-direction: column;
		animation: pulse 1s forwards;
	}
	.icons article:hover img {
		transform: scale(1.3) translateY(-10px);
		transition: all 200ms ease-in-out;
	}
	a {
		color: var(--main-color);
	}
</style>
