<script>
	export let name;
	var newColour='black';

	const onClick=()=> {newColour=newColour}

</script>

<main>
	<h1>When I am bored <br><span>being Quarantined!</span></h1>
	<h2 style="color:{newColour}" id="p-text">{newColour} is colour</h2>
	<button on:click={onClick}>Update Colour</button>
	<input type="text" bind:value={newColour}>
	<h3 style="color:{newColour}">sforsaiif</h3>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h2 {
		font-size: 3em;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 3.6em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>