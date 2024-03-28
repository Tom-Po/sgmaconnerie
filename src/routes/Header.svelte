<script>
	import { page } from '$app/stores';
</script>

<header>
	<nav>
		<ul>
			<li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
				<a href="/" class={$page.url.pathname === '/' ? 'active' : undefined} target="">
					<span data-hover="Accueil">Accueil</span>
				</a>
			</li>
			<li aria-current={$page.url.pathname === '/maconnerie' ? 'page' : undefined}>
				<a
					href="/maconnerie"
					class={$page.url.pathname === '/maconnerie' ? 'active' : undefined}
					target=""
				>
					<span data-hover="Maçonnerie générale">Maçonnerie générale</span>
				</a>
			</li>
			<li aria-current={$page.url.pathname === '/renovation' ? 'page' : undefined}>
				<a
					href="/renovation"
					class={$page.url.pathname === '/renovation' ? 'active' : undefined}
					target=""
				>
					<span data-hover="Rénovation">Rénovation</span>
				</a>
			</li>
			<li aria-current={$page.url.pathname === '/realisations' ? 'page' : undefined}>
				<a
					href="/realisations"
					class={$page.url.pathname === '/realisations' ? 'active' : undefined}
					target=""
				>
					<span data-hover="Mes réalisations">Mes réalisations</span>
				</a>
			</li>
			<li aria-current={$page.url.pathname === '/contact' ? 'page' : undefined}>
				<a
					href="/contact"
					class={$page.url.pathname === '/contact' ? 'active' : undefined}
					target=""
				>
					<span data-hover="Contact">Contact</span>
				</a>
			</li>
		</ul>
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
</style>
