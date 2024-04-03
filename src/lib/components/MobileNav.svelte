<script lang="ts">
	import { fly } from '$lib/transitions';
	import type { Route } from '$lib/types';

	export let open = false;
	export let routes: Route[] = [];
	export let toggleMenu = () => {};
</script>

<svelte:window
	on:wheel|nonpassive={(e) => {
		if (open) e.preventDefault();
	}}
/>

{#if open}
	<div transition:fly={{ y: -100 }}>
		{#each routes as { pathname, label }}
			<a on:click={toggleMenu} href={pathname}>{label}</a>
		{/each}
	</div>
{/if}

<style>
	div {
		background-color: var(--main-color);
		text-align: center;
		font-size: 1.5em;
		letter-spacing: 0.15em;
		color: #eef;
		z-index: 1500;
		position: fixed;
		inset: 0;
		display: flex;
		align-items: center;
		flex-direction: column;
		justify-content: center;
	}

	a {
		margin: 0.5rem auto;
	}
</style>
