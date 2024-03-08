<script>
	export let nome;
	export let prezzo;
</script>

<div class="riga_menu">
	<p>{nome}</p>
	<p>{prezzo}€</p>
</div>

<style>
	.riga_menu {
		display: flex;
		justify-content: space-between;
		min-width: 650px;
		padding-top: 20px;
		font-family: sans-serif;
	}
</style>
