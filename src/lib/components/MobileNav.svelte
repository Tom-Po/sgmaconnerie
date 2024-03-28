<script type="ts">
	export let open = false;
</script>

{#if open}
	<div>
		{#each ['/', 'maconnerie', 'renovation', 'realisations'] as link, i}
			<p>
				<a on:click={() => (open = !open)} href={link}>{link === '/' ? 'Home' : link}</a>
			</p>
		{/each}
	</div>
{/if}

<style>
	div {
		background-color: var(--main-color);
		text-align: center;
		font-size: 1.5em;
		letter-spacing: 0.15em;
		padding: 1em;
		padding-top: 0;
		color: #eef;
		z-index: 2000;
		position: fixed;
		inset: 0;
		display: flex;
		align-items: center;
		flex-direction: column;
	}
	p {
		cursor: pointer;
		width: max-content;
		margin: 1rem auto;
	}
	p:hover {
		text-decoration: underline;
	}
</style>
