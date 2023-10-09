<script>
	import "milligram/dist/milligram.min.css";

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
</script>
<main>
	<div style="margin-left:5rem;margin-right:5rem; margin-top: 5rem;">
		<div>
		<h1>Sérieusement ^^</h1>
		<h3>haha on me l avait pas sortie celle la depuis loooongtemps 🙂</h3>

	</div>
		<div class="row">
			<div class="column">
			<div class="row">
				<div class="column">
					<label for="subject">Qu'est ce que vous n'etes pas ? </label>
					<input id="subject" type="text" bind:value={subject} placeholder="Sujet"/>
				</div>
			</div>
			<label for="action1" style="margin-top: 20px; margin-bottom: 0">Qu'est ce que vous faites alors ? (que des verbes)</p>
			<div class="row">
				<input id="action1" class="column" style="margin:10px" type="text" bind:value={action1} placeholder="Action 1"/>
				<input class="column" style="margin:10px" type="text" bind:value={action2} placeholder="Action 2"/>
				<input class="column" style="margin:10px" type="text" bind:value={action3} placeholder="Action 3"/>
				<input class="column" style="margin:10px" type="text" bind:value={action4} placeholder="Action 4"/>
			</div>
			<label for="search1" style="margin-top: 20px; margin-bottom: 0">Qu'est ce que les rageux recherchent ? </p>
			<div class="row">
				<input id="search1" class="column" style="margin:10px" type="text" bind:value={search1} placeholder="Recherche 1"/>
				<input class="column" style="margin:10px" type="text" bind:value={search2} placeholder="Recherche 2"/>
			</div>
			<label for="has1" style="margin-top: 20px; margin-bottom: 0">Qu'est ce que vous n'avez pas plus que vos 11 meilleurs amis ? </p>
			<input id="has1" type="text" style="margin:10px" bind:value={has1}/>
			<label for="has2" style="margin-top: 20px; margin-bottom: 0">Qu'est ce que vous avez de plus que vos 11 meilleurs amis ? </p>
			<input id="has2" type="text" style="margin:10px" bind:value={has2}/>
			<label for="comment"  style="margin-top: 20px; margin-bottom: 0">Qu'est ce que vos 11 meilleurs amis commentent notamment ? </p>
			<input id="comment" type="text" style="margin:10px" bind:value={comment} placeholder="Commentaire instagram" />
		</div>
		<div class="column">
			<div style="font-size:20px;margin:20px 50px;text-align: justify;">

				<strong>{subject || '{sujet}'}</strong> moi ? Sérieusement ^^ haha on me l avait pas sortie celle la depuis loooongtemps 🙂 demande a mes potes si je suis <strong>{subject || '{sujet}'}</strong> tu vas voir les réponses que tu vas te prendre XD rien que la semaine passee j ai <strong>{action1 || '{action 1}'}</strong> dont chuuuuut ferme la <strong>{subject || '{sujet}'}</strong> de merde car toi tu m as tout tout l air d un bon <strong>{subject || '{sujet}'}</strong> de merde car souvent vous etes frustrer de ne pas <strong>{action2 || '{action 2}'}</strong> 🙂 ses agreable de <strong>{action3 || '{action 3}'}</strong> ou <strong>{action4 || '{action 4}'}</strong> hein ? tu peux pas répondre car tu ne sais pas ce que c ou alors tu le sais mais tu as du taper dans ta barre de recherche « <strong>{search1 || '{recherche 1}'}</strong> » ou « <strong>{search2|| '{recherche 2}'}</strong> » pour comprendre ce que c etait mdddrrr !! cest grave quoiquil en soit....pour revenir a moi, je pense que je suis le mec le moins <strong>{subject || '{sujet}'}</strong> de ma bande de 11 meilleurs amis pas psk j ai eu le plus de <strong>{has1 || '{truc que j\'ai eu 1}'}</strong> mais psk j ai eu <strong>{has2 || '{truc que j\'ai eu 2}'}</strong> que mes amis 😀 ses pas moi qui le dit, ses eux qui commente sous mes photos insta « <strong>{comment || '{commentaire}'}</strong> notamment! »
			</div>
				<div style="text-align: center;">
					<img style="width:150px;border-radius: 100%; text-align: center;" src="/moi.png">
				</div>
			</div>
		</div>
	</div>
</main>

<style scoped>
	strong {
		color: #cf2f74;
	}
</style>
