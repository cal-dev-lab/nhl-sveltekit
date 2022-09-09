<script>
    const imgUrl = new URL('../../../images/3.jpg', import.meta.url).href
</script>

<section>
	<div class="relative">
		<div class="w-full h-full top-0 absolute"></div>
		<div class="w-full h-full flex flex-col-reverse absolute top-0 justify-center mx-auto md:pl-28 items-center">
			<a href="/#">
				<p class="tracking-wider text-2xl md:text-md py-2 px-3 rounded-md font-bold mb-0 uppercase font-opensans">
				The home of plants
                </p>
			</a>
			<div class="tracking-tighter text-7xl md:text-9xl font-bold font-grotesk">Plantesk</div>
			</div>
			<img src={imgUrl} alt="A green plant." class="h-96 w-screen object-cover aspect-auto" />
		</div>
</section>