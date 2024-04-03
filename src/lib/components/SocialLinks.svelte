<script>
	export let white = false;

	const socialLinks = [
		{
			path: 'https://www.instagram.com/sg_maconnerie35/?igshid=YmMyMTA2M2Y%3D',
			label: 'Instagram',
			logoSrc:
				'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/ins.png'
		},
		{
			path: 'https://goo.gl/maps/QmZsHZ4ju91QRf8D6',
			label: 'Google Maps',
			logoSrc:
				'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/gmb.png'
		},
		{
			path: 'https://www.facebook.com/',
			label: 'Facebook',
			logoSrc:
				'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/fb.png'
		}
	];
	const constrastedSocialLinks = [
		{
			path: 'https://www.instagram.com/sg_maconnerie35/?igshid=YmMyMTA2M2Y%3D',
			label: 'Instagram',
			logoSrc:
				'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/Ins1.png'
		},
		{
			path: 'https://goo.gl/maps/QmZsHZ4ju91QRf8D6',
			label: 'Google Maps',
			logoSrc:
				'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/gmb1.png'
		},
		{
			path: 'https://www.facebook.com/',
			label: 'Facebook',
			logoSrc:
				'https://local-fr-public.s3.eu-west-3.amazonaws.com/prod/webtool/userfiles/39524/fb1.png'
		}
	];

	let links = white ? constrastedSocialLinks : socialLinks;
</script>

<div>
	{#each links as { path, label, logoSrc }}
		<a href={path} target="_blank" class="social-link">
			<img src={logoSrc} alt={label} />
		</a>
	{/each}
</div>

<style>
	.social-link {
		margin: 0 0.25rem;
	}
</style>
