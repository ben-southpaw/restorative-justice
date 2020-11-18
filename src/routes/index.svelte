<script>
	import Header from '../components/Header.svelte';
	import Nav from '../components/Nav.svelte';

	import { onMount } from 'svelte';


	var data;

	onMount(async () => {
		const res = await fetch(`../data/copy.json`);
    data = await res.json();
    console.log(data, 'out onmount');
	});




</script>

<svelte:head>
	<title>Restorative Justice</title>
</svelte:head>
<Nav />
<Header />




<style lang="css">
	
</style>