<script>
    import Button from "../Components/Button.svelte";
    export let image;
    export let title;
    export let desc;
    export let btnText;
</script>

<div class="max-w-7xl mx-auto py-16 px-4 sm:py-10 sm:px-6 lg:px-8">
    <div class="grid grid-cols-reverse order-1 grid-cols-1 gap-y-10 sm:grid-cols-2 gap-x-6 xl:gap-x-8 mx-auto justify-center items-center bg-white p-10 rounded-3xl">
        <div class="order-2 sm:order-1">
            <h2 class="z-50 text-5xl md:text-6xl lg:text-7xl font-grotesk font-bold text-center md:text-right">
                {title}
            </h2>
            <p class="text-justify text-xs mt-5 font-opensans leading-6 tracking-widest">
                {desc}
            </p>
            <Button text="{btnText}" />
        </div>
        <div class="w-full h-full z-10 order-1 sm:order-2">
            <img 
                class="z-10 h-full aspect-auto object-cover  md:rounded-r-3xl md:rounded-bl-none rounded-t-3xl sm:rounded-br-3xl sm:rounded-tl-none hover:scale-90 transition duration-300 md:w-full"
                src={'https://plantesk.sirv.com/plantesk/ImageRightTextLeft/' + image + '.jpg'} alt="title" 
                width="600"
            />
        </div>
    </div>
</div>