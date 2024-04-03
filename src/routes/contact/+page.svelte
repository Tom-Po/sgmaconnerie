<script>
	import ContactForm from '$lib/components/ContactForm.svelte';
	import ContentBox from '$lib/components/ContentBox.svelte';
</script>

<ContentBox title="Contactez mon entreprise de maçonnerie et de rénovation à Saint-Malo " centered>
	<div slot="text">
		<h2 class="exo dark">
			Laissez votre message à propos mes prestations en maçonnerie en Ille-et-Vilaine
		</h2>
		<p>
			N’hésitez pas à m’adresser vos demandes à l’aide de ce formulaire de contact. Je vous
			répondrai dans les plus brefs délais.
		</p>
	</div>
</ContentBox>
<ContactForm />
<div class="infos">Mes horaires Du lundi au samedi de 8 h à 18 h 30</div>

<style>
	h2,
	p {
		margin-bottom: 2rem;
	}

	@media screen and (max-width: 992px) {
		h2,
		p {
			margin-bottom: 0.5rem;
		}
	}
</style>
