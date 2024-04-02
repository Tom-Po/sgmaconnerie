<script lang="ts">
	type ImageType = {
		id: number;
		alt: string;
		src: string;
	};
	export let images: ImageType[] = [];
</script>

<div class="gallery">
	{#each images as img}
		<a target="_blank" href={img.src}>
			<img src={img.src} alt={img.alt} />
		</a>
	{/each}
</div>

<style>
	.gallery {
		display: flex;
		align-items: stretch;
		justify-content: center;
		gap: 0.5rem;
		margin: 0 1rem;
	}
	.gallery a {
		overflow: hidden;
		display: flex;
	}
	.gallery img {
		transition: all 300ms ease-in-out;
	}
	.gallery img:hover {
		transform: scale(1.2);
	}
	@media screen and (max-width: 1200px) {
		.gallery {
			flex-wrap: wrap;
		}
		.gallery a {
			flex-basis: calc(50% - 1rem);
		}
	}
	@media screen and (max-width: 768px) {
		.gallery a {
			flex-basis: 100%;
			align-items: center;
			justify-content: center;
		}
	}
</style>
