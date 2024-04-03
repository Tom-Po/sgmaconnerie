<script lang="ts">
	import type { ImageType } from '$lib/types';

	export let images: ImageType[] = [];
</script>

<div class="gallery">
	{#each images as { src, alt }}
		<a target="_blank" href={src}>
			<img {src} {alt} />
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

	a {
		overflow: hidden;
		display: flex;
		max-height: 500px;
	}

	img {
		transition: all 300ms ease-in-out;
	}

	img:hover {
		transform: scale(1.2);
	}

	@media screen and (max-width: 1200px) {
		.gallery {
			flex-wrap: wrap;
		}
		a {
			flex-basis: calc(50% - 1rem);
		}
	}
	@media screen and (max-width: 768px) {
		a {
			flex-basis: 100%;
			align-items: center;
			justify-content: center;
		}
	}
</style>
