<script>

    /************
    Props to be populated in:
    /lib/Components/PlantCard.svelte
    *************/

    export let title;
    export let tag;
    export let synopsisHeading;
    export let synopsisBody;

</script>

<div class="relative group hover:scale-110 transition duration-300 drop-shadow-md hover:drop-shadow-xl">
    <div class="p-8 absolute inset-0 z-10 bg-white text-center flex flex-col items-center justify-center opacity-0 rounded-3xl hover:opacity-100 bg-opacity-90 duration-300">
        <h3 class="text-2xl font-bold font-grotesk">
            {synopsisHeading}
        </h3>
        <p class="font-opensans">
            {synopsisBody}
        </p>
    </div>
    <div class="w-full rounded-t-lg bg-transparent">
        <img src={'https://plantesk.sirv.com/plantesk/plant-loops/' + title + '.jpg'} alt="{title}" class="h-64 w-full object-cover rounded-t-3xl" />
    </div>
    <div class="p-6 bg-white rounded-b-3xl">
        <p id="category" class="text-sm uppercase font-opensans font-thin py-2 text-green-600">
            {tag}
        </p>
        <p id="title" class="text-3xl font-bold font-grotesk">
            {title}
        </p>
    </div>
</div>