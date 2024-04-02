<script>
	import Grenier from '$lib/images/grenier.jpg';
	import LogoBlanc from '$lib/images/logo-blanc.png';
</script>

<div class="display" style="background-image: url({Grenier})">
	<div class="overlay"></div>
	<img class="logo" src={LogoBlanc} alt="" />
	<div class="infos">
		<article>
			<p>35400 Saint-Malo</p>
		</article>
		<article>
			<p>07 85 42 98 86</p>
		</article>
		<article>
			<a
				class="social-link"
				href="https://www.instagram.com/sg_maconnerie35/?igshid=YmMyMTA2M2Y%3D"
				target="_blank"
				><img
					alt="Ins1"
					src="https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/Ins1.png"
				/></a
			><a class="social-link" href="https://goo.gl/maps/QmZsHZ4ju91QRf8D6" target="_blank"
				><img
					alt="gmb1"
					src="https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/gmb1.png"
				/></a
			><a class="social-link" href="https://www.facebook.com/" target="_blank"
				><img
					alt="fb1"
					src="https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/fb1.png"
				/></a
			>
		</article>
	</div>
</div>

<style>
	.display {
		padding-top: 2rem;
		min-height: 90vh;
		display: flex;
		align-items: center;
		justify-content: center;
		flex-direction: column;
		padding: 4rem;
		/* TODO background image */
		background-position: center 60%;
		position: relative;
	}

	.overlay {
		position: absolute;
		inset: 0;
		background-color: rgba(0, 0, 0, 0.3);
	}

	.display img {
		max-width: 350px;
		z-index: 100;
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
		min-width: 250px;
		border-right: 1px solid var(--white);
		display: flex;
		align-items: center;
		justify-content: center;
	}
	article:last-of-type {
		border: none;
	}
	article p {
		margin-bottom: 0;
	}

	.logo {
		animation: pulse 1s forwards cubic-bezier(0.4, -0.6, 0.2, 1);
	}

	.social-link {
		margin: 0 0.25rem;
	}
</style>
