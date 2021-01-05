<script>
	export let subject;
	export let action1;
	export let action2;
	export let action3;
	export let action4;
	export let search1;
	export let search2;
	export let has1;
	export let has2;
	export let comment;
	export let result;

	function calculate() {
		if(subject && action1 && action2 && action3 && action4 && search1 && search2 && has1 && has2 && comment){
			result = `${subject} moi ? Sérieusement ^^ haha on me l avait pas sortie celle la depuis loooongtemps 🙂 demande a mes potes si je suis ${subject} tu vas voir les réponses que tu vas te prendre XD rien que la semaine passee j ai ${action1} dont chuuuuut ferme la ${subject} de merde car toi tu m as tout tout l air d un bon ${subject} de merde car souvent vous etes frustrer de ne pas ${action2} 🙂 ses agreable de ${action3} ou ${action4} hein ? tu peux pas répondre car tu ne sais pas ce que c ou alors tu le sais mais tu as du taper dans ta barre de recherche « ${search1} » ou « ${search2} » pour comprendre ce que c etait mdddrrr !! cest grave quoiquil en soit....pour revenir a moi, je pense que je suis le mec le moins ${subject} de ma bande de 11 meilleurs amis pas psk j ai eu le plus de ${has1} mais psk j ai eu ${has2} que mes amis 😀 ses pas moi qui le dit, ses eux qui commente sous mes photos insta « ${comment} notamment! »`;
		}
	}
</script>
<main>
	<h1>Sérieusement ^^</h1>
	<h3>Sérieusement ^^</h3>
	<p>Qu'est ce que vous n'etes pas ? </p><input type="text" bind:value={subject} placeholder="Sujet"/>
	<p>haha on me l avait pas sortie celle la depuis loooongtemps 🙂</p>
	<input type="text" bind:value={action1} placeholder="Action 1"/>
	<input type="text" bind:value={action2} placeholder="Action 2"/>
	<input type="text" bind:value={action3} placeholder="Action 3"/>
	<input type="text" bind:value={action4} placeholder="Action 4"/>
	<p>Qu'est ce que les rageux recherchent ? </p>
	<input type="text" bind:value={search1} placeholder="Recherche 1"/>
	<input type="text" bind:value={search2} placeholder="Recherche 2"/>
	<p>Qu'est ce que vous avez n'avez pas plus que vos 11 meilleurs amis ? </p>
	<input type="text" bind:value={has1}/>
	<p>Qu'est ce que vous avez avez de plus que vos 11 meilleurs amis ? </p>
	<input type="text" bind:value={has2}/>
	<p>Qu'est ce que vous vos 11 meilleurs amis commentent notamment ? </p>
	<input type="text" bind:value={comment} placeholder="Commentaire instagram" />
	<br>
	<button class="btn" on:click={calculate}> Générer </button>
	<p>Pavé : </p>
	{#if result}
	<p> { result } </p>
	{/if}
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
