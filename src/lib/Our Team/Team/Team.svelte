<script>
    import Heading from "../../Components/Heading.svelte";
    import PersonCard from "../../Components/PersonCard.svelte";
    import FromLeft from "../../Components/ScrollAnimations/FromLeft.svelte";
    import FromRight from "../../Components/ScrollAnimations/FromRight.svelte";

    // Data to iterate over
    let people = [
        {
            name: "Callum Lees",
            job: "Developer",
            favPlant: "Chinese Evergreen",
            id: "1"
        },
        {
            name: "Claire Stark",
            job: "Author",
            favPlant: "Spider Plant",
            id: "2"
        },
        {
            name: "David Jones",
            job: "Journalist",
            favPlant: "Aloe Vera",
            id: "3"
        },
        {
            name: "Colin Chun",
            job: "Coffee Brewer",
            favPlant: "Peace Lily",
            id: "4"
        },
        {
            name: "Dominic Fitz",
            job: "Researcher",
            favPlant: "Crotonn",
            id: "5"
        },
        {
            name: "Theo Williams",
            job: "Content Writer",
            favPlant: "Dracaena",
            id: "6"
        },
    ]
</script>

<div class="max-w-7xl mx-auto py-16 px-4 sm:py-10 sm:px-6 lg:px-8">
        <div>
            <FromRight>
                <Heading title="A bunch of lovely seedlings!" />
                <p class="font-opensans text-xl text-center mb-20">What we do wouldn't be possible without this great bunch, they've really helped us grow! </p>
            </FromRight>
        </div>
    
        <div class="grid grid-cols-1 gap-y-10 sm:grid-cols-2 lg:grid-cols-3 gap-x-6 xl:gap-x-8 mx-auto">
            <!-- START: Iterate over data -->
            <!-- Props destructured -->
            {#each people as {name, job, favPlant, id}}
            <FromLeft>
                <PersonCard name={name} id={id} job={job}  favPlant={favPlant} />
            </FromLeft>
            {/each}
            <!-- END: Iterate over data -->
        </div>
    
</div>