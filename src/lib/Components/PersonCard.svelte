<script>
    export let name;
    export let job;
    export let favPlant;
    export let id;
</script>

<div class="p-10 bg-white flex flex-col mx-auto justify-center rounded-3xl shadow-md hover:scale-110 transition duration-300">
    <div class="w-full">
        <img src={'https://plantesk.sirv.com/plantesk/team/' + name + '.jpg'} class="h-64 w-64 rounded-full object-cover" alt="{name}" />
    </div>
    <div>
        <h3 class="mb-5 mt-10 font-grotesk font-bold text-3xl">{name}</h3>
        <hr class="mb-5" />
        <div class="flex flex-col">
            <p class="text-2xl font-opensans">{job}</p>
            <div class="mt-5">
                <p class="text-xl font-grotesk">Favourite plant:</p>
                <p class="font-opensans">{favPlant}</p>
            </div>
            
        </div>
    </div>
</div>