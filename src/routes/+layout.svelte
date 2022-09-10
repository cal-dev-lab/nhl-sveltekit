<script>
	import Navbar from '$lib/Navbar/Navbar.svelte';
	import '../app.css';
	import { onMount } from "svelte";

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

<Navbar />

{#if !isPageLoaded}
	<div id="load" class="grid h-screen items-center place-items-center mx-auto">
		<img src="/tail-spin.svg" alt="Loader icon" />
	</div>
{/if}

<main>
	<slot />
</main>