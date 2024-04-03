<script lang="ts">
	import { page } from '$app/stores';
	import MobileNav from '$lib/components/MobileNav.svelte';
	import type { Route } from '$lib/types';
	import Hamburger from './Hamburger.svelte';
	let open = false;

	const allRoutes: Route[] = [
		{
			pathname: '/',
			label: 'Accueil'
		},
		{
			pathname: '/maconnerie',
			label: 'Maconnerie générale'
		},
		{
			pathname: '/renovation',
			label: 'Rénovation'
		},
		{
			pathname: '/realisations',
			label: 'Réalisations'
		},
		{
			pathname: '/contact',
			label: 'Contact'
		}
	];

	function toggleMenu() {
		open = !open;
	}

	let innerWidth = 0;
	function handleResize() {
		if (innerWidth >= 992) open = false;
	}
</script>

<svelte:window on:resize={handleResize} bind:innerWidth />

<header>
	<nav class="desktop-nav">
		<ul>
			{#each allRoutes as { pathname, label }}
				{@const active = $page.url.pathname === pathname}
				<li aria-current={active ? 'page' : undefined}>
					<a href={pathname} class:active>
						{label}
					</a>
				</li>
			{/each}
		</ul>
	</nav>
	<nav class="mobile-nav">
		<Hamburger {toggleMenu} {open} />
		<MobileNav {toggleMenu} routes={allRoutes} bind:open />
	</nav>
</header>

<style>
	nav {
		display: flex;
		background-color: var(--main-color);
	}
	ul {
		display: flex;
		margin: 0 auto;
		gap: 0.25rem;
		padding: 0;
	}
	nav a {
		color: var(--white);
		padding: 1rem;
		display: block;
	}
	header {
		position: fixed;
		left: 0;
		right: 0;
		top: 0;
		z-index: 1000;
	}
	.mobile-nav {
		display: none;
	}
	@media screen and (max-width: 1000px) {
		.mobile-nav {
			display: flex;
			min-height: 40px;
		}
		.desktop-nav {
			display: none;
		}
	}
</style>
