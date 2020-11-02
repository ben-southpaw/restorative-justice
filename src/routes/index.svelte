<script>
	import Header from '../components/Header.svelte';
	import Nav from '../components/Nav.svelte';
	export let name;
</script>

<svelte:head>
	<title>Restorative Justice</title>
</svelte:head>
<Nav />
<Header />




<style lang="scss">
	* {
		box-sizing: border-box;

	}

	img  {
		height: 300px;
		width: 500px;
	}
	body {
		display: flex;
		min-height: 100vh;
		flex-direction: column;
		margin: 0;
	}
	main {
		display: flex;
		flex: 1;

		text-align: center;
		//padding: 1em;
		//max-width: 240px;
		margin: 0 auto;

	}

	header {
		text-align: center;
		//padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	aside {
		display: none;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>