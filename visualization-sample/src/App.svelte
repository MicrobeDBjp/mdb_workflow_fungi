<script>
	const message = "So What?"
	let current = 0;
	const toggle = () => current = (current+1) % 2;
	const ala = () => console.log("ok??");
</script>



<main>
	{message[current]}
	<select name="NCBI_Gene_ID" id="ncbi_gene_id" on:change={ala}>
		<option value="">--Please choose an Gene ID</option>
		<option value="1">alpha-1-B glycoprotein (A1BG)</option>
		<option value="9">N-acetyltransferase (NAT1)</option>
		<option value="10">N-acetyltransferase 2 (NAT2)</option>
	</select>

	

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