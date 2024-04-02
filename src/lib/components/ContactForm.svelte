<script>
	let name = '';
	let email = '';
	let phoneNumber = '';
	let message = '';
</script>

<form action="#">
	<div class="box">
		<input type="text" bind:value={name} name="name" placeholder="Votre nom" />
	</div>

	<div class="box">
		<input type="email" bind:value={email} name="email" placeholder="Votre email" />
	</div>

	<div class="box">
		<input
			type="text"
			bind:value={phoneNumber}
			name="phoneNumber"
			placeholder="Votre numéro de téléphone"
		/>
	</div>
	<div class="box">
		<textarea bind:value={message} name="message" placeholder="Votre message" rows="10"></textarea>
	</div>
	<input type="submit" value="Envoyer" />
	<p class="disclaimer">
		Afin de traiter votre demande, SG MACONNERIE devra effectuer un traitement des données
		personnelles vous concernant. Les données sont conservées pendant 2 ans à compter de notre
		dernier contact et sont destinées exclusivement à SG MACONNERIE, elles ne seront pas transmises
		à des tiers.
		<br />
		<br />
		Conformément à la loi Informatique et Libertés du 6 janvier 1978 modifiée, vous bénéficiez d’un droit
		d’accès et de rectification des données vous concernant, d’un droit d’opposition pour motifs légitimes,
		d’un droit à l’effacement des données. Vous disposez également d’un droit à la récupération et à
		la portabilité des données dans certains cas spécifiquement prévus par la loi.
		<br />
		<br />
		Pour l’exercice de vos droits veuillez contacter :
		<br /> SG MACONNERIE, 16 Boulevard Villebois Mareuil, 35400 SAINT-MALO
		<br />
		contact@sgmaconnerie.fr
	</p>
</form>

<style>
	form {
		width: 70%;
		margin: 0 auto;
		display: flex;
		flex-direction: column;
		align-items: stretch;
		gap: 0.5rem;
		margin-bottom: 1rem;
	}

	.box input,
	.box textarea {
		background-color: #eeeeee;
		width: 100%;
		border: none;
		box-shadow: none;
		padding: 0.5rem 1rem;
	}
	input[type='submit'] {
		border-radius: 0;
		box-shadow: none;
		border: none;
		text-transform: uppercase;
		padding: 0.5rem 1rem;
		background-color: #cccccc;
	}
	.disclaimer {
		font-size: 8px;
		text-align: center;
	}
</style>
