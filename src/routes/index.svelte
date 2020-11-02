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
<main>
	<article><h1>Services</h1></article>

	<aside><p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> twats.</p></aside>
</main>
<footer>Footer</footer>




<style>
	* {
		box-sizing: border-box;
		overflow: hidden;
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
	main > article {
		flex: 1;
		height: 150vh;
	}
	main > nav,
	main > aside {
		flex: 0 0 20vw;
		background: beige;
	}
	main > nav {
		order: -1;
	}
	Header, footer {
		background: yellowgreen;
		height: 20vh;
	}
	Header, footer, article, nav, aside {
		padding: 1em;
	}
	header {
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

	aside {
		display: none;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>