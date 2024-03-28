<script>
	export let title = '';
	export let borderless = false;
	export let contrasted = false;
</script>

<div class="content-box {contrasted && 'contrasted'}">
	<div class="inner">
		{#if title !== ''}
			<h1>{title}</h1>
		{/if}
	</div>
	<div class="wrapper">
		<div class="text {borderless && 'borderless'}">
			<slot name="text">
				<p>Missing text</p>
			</slot>
		</div>
		<div class="image">
			<slot name="image" />
		</div>
	</div>
</div>

<style>
	h1 {
		font-size: 2.3rem;
		font-weight: 400;
		text-align: center;
		margin: 0 auto 0.5rem auto;
		padding: 1rem;
	}
	p {
		margin-bottom: 0.5rem;
	}

	.wrapper {
		display: flex;
		align-items: center;
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
</style>
