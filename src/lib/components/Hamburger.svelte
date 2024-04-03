<script>
	export let open = false;
	export let toggleMenu = () => {};
</script>

<!-- svelte-ignore a11y-click-events-have-key-events -->
<!-- svelte-ignore a11y-no-static-element-interactions -->
<div class:open on:click={toggleMenu}>
	<span class="top" />
	<span class="middle" />
	<span class="bottom" />
</div>

<style>
	div {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: space-between;
		height: 26px;
		width: 32px;
		margin-top: 0.5rem;
		z-index: 2000;
		margin-left: 1rem;
	}
	.open .middle {
		transition: transform 0.2s ease-in-out;
		transform: scaleY(0);
	}

	.open .top {
		transform-origin: 0% 0%;
		transition: transform 0.4s ease-in-out;
		transform: rotate(45deg);
	}
	.open .bottom {
		transform-origin: 0% 100%;
		transition: transform 0.4s ease-in-out;
		transform: rotate(-45deg);
	}

	span {
		display: block;
		height: 4px;
		background-color: var(--white);
		transition: all 300ms ease-in-out;
		width: 100%;
		border-radius: 10px;
	}
</style>
