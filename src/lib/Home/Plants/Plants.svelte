<script>

    // The component to pass props to/from
    import PlantCard from "../../Components/PlantCard.svelte"

    // Data to iterate over
    let plants = [
        {
            name: "Spider Plant", 
            id: "1", 
            tag: "House plant", 
            synopsisB: "Chlorophytum comosum 'Variegatum', or the Spider Plant as it’s more commonly known, is an iconic choice that remains enduringly popular. With a cascading habit, its bright glossy foliage spills over the edge of the pot making this an excellent choice for high windowsills or shelves. Spider plants are also fantastic at cleaning the air in the room."
        },
        {
            name: "Aloe Vera", 
            id: "2", 
            tag: "House plant", 
            synopsisB: "Known for its medicinal properties, Aloe Vera is a firm favourite in many households. As a succulent it enjoys a warm spot on a sunny windowsill, but it also tolerates some neglect and doesn’t mind if you forget to water it occasionally! The distinctive fleshy green foliage is filled with cooling sap that’s good for cooling burns and soothing dry, sun-damaged skin."
        },
        {
            name: "Epipremnum", 
            id: "3", 
            tag: "House plant", 
            synopsisB: "A native of warm countries like Australia, Indonesia and India, Epipremnum aureum, or Devil's Ivy, is an easy-to-care-for plant that looks great in a well-lit corner away from direct sunlight. This vigorous house plant swiftly scales a moss pole to create a lush, tropical-looking feature that takes up very little floor space."
        },
        {
            name: "Snake Plant", 
            id: "4", 
            tag: "House plant", 
            synopsisB: "The most efficient of the air purifiers, Sansevieria trifasciata var. laurentii (also known as the snake plant or Mother-in-Law's Tongue) is a must for many households. It grows almost anywhere in the home, surviving happily in areas of lower light and putting up with some neglect when it comes to watering. The upright habit of the Snake Plant gives it an architectural quality too, perfect for modern decor."
        },
        {
            name: "Peace Lily", 
            id: "5", 
            tag: "House plant", 
            synopsisB: "Not only an elegant plant to enjoy in your home, the Spathiphyllum 'Torelli' , or Peace Lily helps remove benzene, formaldehyde, trichloroethylene, toluene and xylene from the air, all of which can be found in everyday household products. Requiring very little by way of attention, position your Peace Lily away from direct sunlight and let it get to work!"
        },
        {
            name: "Dracaena", 
            id: "6", 
            tag: "House plant", 
            synopsisB: "Also known as the dragon plant, Dracaena is available in a number of different varieties and does a great job of purifying the air in your home. Twisting dark green foliage with bold lime green margins make this house plant incredibly alluring! As a young plant, Dracaena fragrans ‘Tornado’ has a low rounded shape that sits nicely on a worktop or coffee table. With maturity, it gradually extends upwards to form an upright central stem, making a fine floor-standing specimen."
        },
        {
            name: "Croton", 
            id: "7", 
            tag: "House plant", 
            synopsisB: "Croton absolutely loves the higher humidity levels in warm bathrooms, conservatories, kitchens or even indoor swimming pools! Sometimes called 'Joseph's Coat' due to its technicolour foliage, its large, glossy leaves feature striking patterns in red, gold and green. For maximum impact, a croton is the perfect show-stopper."
        },
        {
            name: "Chinese Evergreen", 
            id: "8", 
            tag: "House plant", 
            synopsisB: "Almost impossible to kill, Aglaonema 'Christina' (or Chinese evergreen) has lovely, long green leaves that are streaked or dappled with either yellow or white. Naturally tropical plants, they love the humid conditions found in bathrooms and kitchens."
        },
        {
            name: "Fern", 
            id: "9", 
            tag: "House plant", 
            synopsisB: "Ferns love damp conditions and so will readily thrive in kitchens and bathrooms where they'll absorb the humid air. Producing magnificent, textural fronds with a prehistoric feel, these ancient plants prefer a spot out of direct sunlight."
        },
    ]

</script>

<section>
    <div class="max-w-7xl mx-auto py-16 px-4 sm:py-10 sm:px-6 lg:max-w-7xl lg:px-8">
        <div class="grid grid-cols-1 gap-y-10 sm:grid-cols-2 lg:grid-cols-3 gap-x-6 xl:gap-x-8 mx-auto">
            <!-- START: Iterate over data -->
            <!-- Props destructured -->
            {#each plants as {name, id, tag, synopsisB}}
                <PlantCard title={name} id={id} tag={tag} synopsisHeading={name} synopsisBody={synopsisB} />
            {/each}
            <!-- END: Iterate over data -->
        </div>
    </div>
</section>