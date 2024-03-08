<script>
	import RigaMenu from '$components/RigaMenu.svelte';

	const piatti = [
		{
			nome: 'Pasta al pomodoro',
			prezzo: '12'
		},
		{
			nome: 'Pasta allo scoglio',
			prezzo: '15'
		},
		{
			nome: 'Pizza',
			prezzo: '7'
		},
		{
			nome: 'Bistecca',
			prezzo: '20'
		},
		{
			nome: 'Insalata',
			prezzo: '7'
		},
		{
			nome: 'Patate al forno',
			prezzo: '10'
		},
		{
			nome: 'Tiramisù',
			prezzo: '7'
		},
		{
			nome: 'Gelato',
			prezzo: '5'
		}
	];
</script>

<svelte:head>
	<link rel="stylesheet" href="https://unpkg.com/tailwindcss@3.4.1/src/css/preflight.css" />
</svelte:head>

<div class="menu">
	<h1>MENU</h1>
	<img class="menu_image" src="./_images/cover.jpg" alt="" />
	{#each piatti as piatto}
		<RigaMenu nome={piatto.nome} prezzo={piatto.prezzo}></RigaMenu>
	{/each}
</div>

<style>
	.menu {
		background-color: grey;
		padding: 200px;
		display: flex;
		flex-direction: column;
		align-items: center;
		font-size: 30px;
	}

	.menu_image {
		border-radius: 1000px;
		aspect-ratio: 1;
		height: 300px;
		object-fit: cover;
	}
</style>
