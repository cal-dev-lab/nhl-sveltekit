<script>
	import Navbar from '$lib/Navbar/Navbar.svelte';
	import '../app.css';
	import { onMount } from "svelte";
	import Loader from '../lib/Components/Loader.svelte';

	// For page loading
	let isPageLoaded = false;

	onMount(() => {

		isPageLoaded = true;

		if ( isPageLoaded ) {
			console.log("Page has loaded successfully!");
		} else {
			console.log("Oh no, something has gone wrong here...");
		}
		
	});
</script>

{#if !isPageLoaded}
	<Loader />
{/if}

<Navbar />

<main>
	<slot />
</main>