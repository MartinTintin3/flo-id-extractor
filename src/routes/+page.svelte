<script>
	let input = "";

	const people_pattern = /^http[s]?:\/\/(?:www\.)?flowrestling\.org\/people\/.+/g;
	const athlete_pattern = /^http[s]?:\/\/(?:www\.)?flowrestling\.org\/athletes\/([^\/]+)(?:\/.*)?/g;
</script>

<div class="container">
	<div class="input-container">
		<input type="text" bind:value={input} placeholder="Athlete name, ID, or profile link">
		<button type="button">Search</button>
	</div>
</div>

<style>
	* {
		text-align: center;
		margin: auto;
		font-family: Arial, Helvetica, sans-serif;
	}

	:global(.red) {
		color: red;
	}

	:global(.green) {
		color: green;
	}

	.container {
		padding: 0.7em;
		display: flex;
		flex-direction: column;
		gap: 1em;
	}

	.id-input {
		padding: 10px;
		display: flex;
		gap: 0.3em;
		flex-direction: column;
	}

	input {
		padding: 5px;
		border-radius: 5px;
		border: 1px solid #ccc;
	}

	button {
		padding: 5px;
		border-radius: 5px;
		border: 1px solid #ccc;
		background-color: #eee;
	}

	button:hover {
		background-color: #ddd;
	}

	button:active {
		background-color: #ccc;
	}

	a:visited {
		color: blue;
	}
</style>