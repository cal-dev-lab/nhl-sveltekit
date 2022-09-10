<script>
	import Hero from "../lib/Components/Hero/Hero.svelte";
	import Plants from "../lib/Home/Plants/Plants.svelte";
</script>

<svelte:head>
	<title>Plantesk | Home</title>
	<meta name="description" content="Plantesk - The home of gardening." />
	<link rel="canonical" href="https://xyz.xyz/" />
</svelte:head>

<section>
	<!-- START: Hero -->
	<Hero title="Plantesk" image="3" desc="The home of plants" />
	<!-- END: Hero -->
	<!-- START: Plants -->
	<Plants />
	<!-- END: Plants -->
</section>