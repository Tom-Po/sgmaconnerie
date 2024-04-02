<div class="contact-bar">
	<slot />
	<button>Me contacter</button>
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
	}
	button {
		background-color: black;
		color: white;
		border-radius: 20px;
		padding: 1rem 2rem;
		text-transform: uppercase;
		color: var(--main-color);
		border: 1px solid var(--main-color);
		cursor: pointer;
	}
	button:hover {
		text-decoration: underline;
	}
</style>
