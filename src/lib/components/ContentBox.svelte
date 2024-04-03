<script>
	export let title = '';
	export let borderless = false;
	export let contrasted = false;
	export let centered = false;
	export let themed = false;
	export let titleOnly = false;
</script>

<div class:contrasted class:centered class="content-box">
	<div class="inner">
		{#if title !== ''}
			<h1>{title}</h1>
		{/if}
	</div>
	{#if !titleOnly}
		<div class="wrapper">
			<div class:borderless class:themed class="text">
				<slot name="text" />
			</div>
			<div class="image">
				<slot name="image" />
			</div>
		</div>
	{/if}
</div>

<style>
	.centered {
		text-align: center;
	}
	.centered .text {
		flex-basis: 100%;
		border: none;
		margin: 0 auto;
	}
	.text.themed {
		border-color: var(--main-color);
	}
	.text {
		flex-basis: 41%;
		flex-shrink: 0;
		flex-grow: 1;
		margin-right: auto;
		padding: 1rem;
		border-left: 1px solid var(--black);
		margin-left: 10%;
		margin-top: 2rem;
	}
	h1 {
		font-size: 2.3rem;
		font-weight: 400;
		text-align: center;
		margin: 0 auto 0.5rem auto;
		padding: 1rem;
	}

	.wrapper {
		display: flex;
		align-items: center;
	}

	.image {
		margin-right: 10rem;
		flex-shrink: 1;
	}

	.borderless {
		border: none;
	}
	.contrasted {
		padding-top: 2rem;
		padding-top: 2rem;
		padding-bottom: 2rem;
		background-color: rgba(235, 235, 235, 1);
		margin-top: 3%;
	}

	@media screen and (max-width: 1200px) {
		.wrapper {
			flex-direction: column;
			justify-content: center;
		}
		.text {
			margin: 2rem;
		}
		.image {
			margin-right: 0;
		}
	}
	@media screen and (max-width: 992px) {
		h1 {
			padding: 0 0.5rem;
		}
		.text {
			padding-top: 0;
			padding-bottom: 0;
			margin: 1rem;
		}
	}
	@media screen and (max-width: 768px) {
		.text,
		.centered {
			margin: 1rem 0.5rem;
		}
	}
</style>
