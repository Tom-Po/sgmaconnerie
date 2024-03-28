<script>
	import { page } from '$app/stores';
	import MobileNav from '$lib/components/MobileNav.svelte';
	let open = false;
	function toggleMenu() {
		open = !open;
	}
</script>

<header>
	<nav class="desktop-nav">
		<ul>
			<li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
				<a href="/" class={$page.url.pathname === '/' ? 'active' : undefined} target="">
					Accueil
				</a>
			</li>
			<li aria-current={$page.url.pathname === '/maconnerie' ? 'page' : undefined}>
				<a
					href="/maconnerie"
					class={$page.url.pathname === '/maconnerie' ? 'active' : undefined}
					target=""
				>
					Maçonnerie générale
				</a>
			</li>
			<li aria-current={$page.url.pathname === '/renovation' ? 'page' : undefined}>
				<a
					href="/renovation"
					class={$page.url.pathname === '/renovation' ? 'active' : undefined}
					target=""
				>
					Rénovation
				</a>
			</li>
			<li aria-current={$page.url.pathname === '/realisations' ? 'page' : undefined}>
				<a
					href="/realisations"
					class={$page.url.pathname === '/realisations' ? 'active' : undefined}
					target=""
				>
					Mes réalisations
				</a>
			</li>
			<li aria-current={$page.url.pathname === '/contact' ? 'page' : undefined}>
				<a
					href="/contact"
					class={$page.url.pathname === '/contact' ? 'active' : undefined}
					target=""
					>Contact
				</a>
			</li>
		</ul>
	</nav>
	<nav class="mobile-nav">
		<button on:click={toggleMenu}>Menu</button>
		<div>{$page.url.pathname.slice(1).toLocaleUpperCase()}</div>
		<MobileNav bind:open />
	</nav>
</header>

<style>
	.mobile-nav button {
		border: none;
		background: none;
	}
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
	a {
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
	.Debug {
		position: fixed;
		top: 0;
		left: 0;
		padding: 3rem;
		background-color: red;
		z-index: 1200;
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
