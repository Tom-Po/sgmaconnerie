<script>
	import LogoBlanc from '$lib/images/logo-blanc.png';
</script>

<div class="footer">
	<img src="" alt="" />
	<div class="company-infos">
		<div class="company-logo">
			<img class="logo" src={LogoBlanc} alt="" />
		</div>
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
						src="https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/ins.png"
					/></a
				><a class="social-link" href="https://goo.gl/maps/QmZsHZ4ju91QRf8D6" target="_blank"
					><img
						alt="gmb1"
						src="https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/gmb.png"
					/></a
				><a class="social-link" href="https://www.facebook.com/" target="_blank"
					><img
						alt="fb1"
						src="https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/fb.png"
					/></a
				>
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
</div>

<style>
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
	.logo {
		max-width: 350px;
	}
	.company-infos {
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
	}
	.infos {
		display: flex;
		color: var(--black);
		z-index: 100;
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
	}

	.logo {
		animation: pulse 1s forwards cubic-bezier(0.4, -0.6, 0.2, 1);
	}

	.social-link {
		margin: 0 0.25rem;
	}
</style>
