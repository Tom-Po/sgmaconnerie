<script>
	import SocialLinks from './SocialLinks.svelte';
</script>

<footer>
	<div class="company">
		<div class="logo">
			<img
				class="logo"
				src={'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/logo.png'}
				alt=""
			/>
		</div>
		<div class="infos">
			<article>
				<p><i class="fa-solid fa-location-dot" /></p>
				<p>35400 Saint-Malo</p>
			</article>
			<article>
				<p><i class="fa-solid fa-mobile-phone" /></p>
				<p>07 85 42 98 86</p>
			</article>
			<article>
				<SocialLinks />
			</article>
		</div>
	</div>
	<div class="bottom">
		<div>
			<a href="http://www.sgmaconnerie.fr/mentions-legales" target="_self" rel="nofollow"
				>Mentions Légales</a
			>
		</div>
		<div>
			<a href="http://www.sgmaconnerie.fr/credits-photos" target="_self" rel="nofollow"
				>Crédits Photos</a
			>
		</div>
		<div>
			<a href="https://www.localetmoi.fr" class="block-link" target="_blank" rel="nofollow"
				>Mettre à jour mon site internet</a
			>
		</div>
	</div>
</footer>

<style>
	footer {
		background-image: url('https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/modif%2020-07-2023/Une%20entreprise-de-ma%C3%A7onnerie--%C3%A0-saint-malo.png');
		background-position: center center;
		background-size: cover;
		background-attachment: scroll;
		background-repeat: no-repeat;
	}
	.logo {
		max-width: 350px;
	}
	.company {
		max-width: 60%;
		margin-left: auto;
		margin-right: 4rem;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
	}
	.logo img {
		max-width: 200px;
	}
	.infos {
		display: flex;
		color: var(--black);
		z-index: 100;
		padding: 2rem 0;
	}
	article {
		flex-basis: 33%;
		text-align: center;
		padding: 1rem 2rem;
		min-width: 250px;
		border-right: 1px solid var(--black);
		display: flex;
		align-items: center;
		justify-content: center;
	}
	article:last-of-type {
		border: none;
	}
	article p {
		margin-bottom: 0;
		font-size: 20px;
	}

	.logo {
		animation: pulse 1s forwards cubic-bezier(0.4, -0.6, 0.2, 1);
	}

	.bottom {
		background-color: #000;
		color: var(--white);
		display: flex;
		justify-content: space-between;
	}
	.bottom > div {
		display: flex;
		justify-content: center;
		flex-grow: 1;
	}
	.bottom a {
		color: var(--white);
		text-align: center;
		text-transform: none;
		font-size: 15px;
		font-weight: 400;
		padding: 0.25rem;
	}

	@media screen and (max-width: 992px) {
		.company {
			max-width: unset;
			margin: 0 auto;
		}
		.company article {
			border: none;
			flex-direction: column;
		}
		.logo {
			margin: 0 auto;
			display: flex;
			justify-content: center;
		}
		.bottom {
			padding: 0.5rem 0;
		}
		.bottom,
		.infos {
			flex-direction: column;
		}
	}
</style>
