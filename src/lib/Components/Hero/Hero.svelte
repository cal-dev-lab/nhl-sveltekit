<script>
	// Props for component
    export let image;	// Choose a number from /hero/ folder on Sirv
    export let title;	// Input own title
    export let desc;	// Input own description
</script>

<section>
	<div class="relative">
		<div class="w-full h-full flex flex-col absolute top-0 justify-center mx-auto items-center text-center place-items-center">
			<div class="rounded-3xl p-10 bg-gray-100/[0.01] backdrop-filter backdrop-blur-sm bg-opacity-5">
				<div class="tracking-tighter text-6xl md:text-7xl lg:text-9xl font-bold font-grotesk">
					{title}
				</div>
				<p class="tracking-wider text-lg md:text-xl py-2 px-3 rounded-md font-bold mb-0 uppercase font-opensans">
					{desc}
            	</p>
			</div>
			
		</div>
		<img src={'https://plantesk.sirv.com/plantesk/hero/' + image + '.jpg'} alt="{title}" class="h-96 w-screen object-cover aspect-auto" />
	</div>
</section>