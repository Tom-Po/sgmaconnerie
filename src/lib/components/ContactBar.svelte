<div class="contact-bar">
	<slot />
	<a href="/contact">Me contacter</a>
</div>

<style>
	.contact-bar {
		max-width: 50%;
		margin: 2rem auto;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		gap: 2rem;
		text-align: center;
	}
	a {
		background-color: black;
		color: white;
		border-radius: 20px;
		padding: 1rem 2rem;
		text-transform: uppercase;
		color: var(--main-color);
		border: 1px solid var(--main-color);
	}
	a:visited,
	a:focus {
		color: var(--main-color);
	}
</style>
