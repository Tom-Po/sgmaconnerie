<script>
	import Grenier from '$lib/images/grenier.jpg';
	import LogoBlanc from '$lib/images/logo-blanc.png';
	import SocialLinks from './SocialLinks.svelte';
</script>

<div class="banner" style="background-image: url({Grenier})">
	<div class="overlay"></div>
	<img class="logo" src={LogoBlanc} alt="" />
	<div class="infos">
		<article>
			<p><i class="fa-solid fa-location-dot" /></p>
			<p>35400 Saint-Malo</p>
		</article>
		<article>
			<p><i class="fa-solid fa-mobile-screen"></i></p>
			<p>07 85 42 98 86</p>
		</article>
		<article>
			<SocialLinks white />
		</article>
	</div>
</div>

<style>
	.banner {
		overflow: hidden;
		padding-top: 2rem;
		min-height: 90vh;
		display: flex;
		align-items: center;
		justify-content: center;
		flex-direction: column;
		padding: 4rem;
		background-position: center 60%;
		position: relative;
	}

	.overlay {
		position: absolute;
		inset: 0;
		background-color: rgba(0, 0, 0, 0.65);
	}

	.infos {
		display: flex;
		color: var(--white);
		z-index: 100;
	}
	article {
		flex-basis: 33%;
		text-align: center;
		padding: 1rem 2rem;
		min-width: 300px;
		border-right: 1px solid var(--white);
		display: flex;
		align-items: center;
		justify-content: center;
		flex-direction: column;
		gap: 1rem;
	}

	article:last-of-type {
		border: none;
	}

	article p {
		margin-bottom: 0;
		font-size: 18px;
	}

	.logo {
		animation: pulse 1s forwards cubic-bezier(0.4, -0.6, 0.2, 1);
		margin-bottom: 1rem;
		max-width: 350px;
		z-index: 100;
	}

	i {
		font-size: 1.5rem;
	}

	@media screen and (max-width: 992px) {
		.infos {
			flex-direction: column;
		}
		article {
			border: none;
			padding-top: 0;
			padding-bottom: 0;
			margin-bottom: 1rem;
		}
	}
</style>
