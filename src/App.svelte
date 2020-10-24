<script>
	export let name;
	let angka1 = 2;
	let angka2 = 4;

	const cobaKlik = () => {
		const hasil = document.getElementById('hasil')
		const tambah = angka1+angka2;
		const kurang = angka1-angka2;
		const kali = angka1*angka2;
		const bagi = angka1/angka2;

		hasil.innerHTML = `${tambah}, ${kurang}, ${kali}, ${bagi}` ;
	}
</script>

<main>
	<h1>Hello {name}!</h1>
	<p>Hasil dari +, -, x, / dari {angka1} & {angka2}</p>
	<button on:click={cobaKlik}>Hasil</button>
	<div id="hasil"></div>
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