<script>
	import PokemonCard from './atoms/PokemonCard.svelte';
	import database from './data/pokemons.js';

	const pokemons = Object.keys(database.pokemons).map(key => (database.pokemons[key]));
	let name = "Maya"
</script>

<style>
	h1 {
		color: purple;
		text-align: center;
	}
	div {
		display: flex;
		flex-wrap: wrap;
	}
</style>

<h1>Pokemons Svelte Test</h1>
<div class="grid-container">
	{#each pokemons as pokemon (pokemon.publicId)}
	<PokemonCard card={pokemon}/>
	{/each}
</div>