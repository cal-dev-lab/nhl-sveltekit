<script>

    // The card to pass props to
    import PlantCard from "../../Components/PlantCard.svelte";

    // Dummy data to iterate over
    let plants = [
        {name: "Spider Plant", id: "1", img: "../../../images/plant-loops/1.jpg"},
        {name: "Aloe Vera", id: "2", img: "../../../images/plant-loops/2.jpg"},
        {name: "Epipremnum", id: "3", img: "../../../images/plant-loops/3.jpg"},
        {name: "Snake Plant", id: "4", img: "../../../images/plant-loops/4.jpg"},
        {name: "Peace Lily", id: "5", img: "../../../images/plant-loops/5.jpg"},
        {name: "Dracaena", id: "6", img: "../../../images/plant-loops/6.jpg"},
        {name: "Croton", id: "7", img: "../../../images/plant-loops/7.jpg"},
        {name: "Chinese Evergreen", id: "8", img: "../../../images/plant-loops/8.jpg"},
        {name: "Fern", id: "9", img: "../../../images/plant-loops/9.jpg"},
    ]

</script>

<section>
    {#each plants as plant}
        <PlantCard title={plant.name} />
    {/each}
</section>