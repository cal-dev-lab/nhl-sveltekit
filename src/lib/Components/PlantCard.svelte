<script>
    /*
    *   Props to be populated in:
    *   /lib/Components/PlantCard.svelte
    */
    export let title;
    export let img;
</script>

<div>
    <h1>{title}</h1>
    <img {img} alt="{title}" />
</div>