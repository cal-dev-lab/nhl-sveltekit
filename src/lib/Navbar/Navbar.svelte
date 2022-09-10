<script>

	import FaPagelines from 'svelte-icons/fa/FaPagelines.svelte';

	let menuShow = false;
		
	const toggleNavbar = () => {
		menuShow = !menuShow;
	}

	const isOpen = () => {
		if ( menuShow ) {
			menuShow = !menuShow
		}
	}

</script>

<header class="sticky top-0 z-50 border-2 shadow-sm border-slate-900/[0.06] backdrop-filter backdrop-blur-lg bg-opacity-30 rounded-b-3xl sm:rounded-b-none -pt-4">
	<div class="flex flex-wrap">
		<div class="w-full">
			<nav class="relative flex flex-wrap items-center justify-between px-2 py-3 navbar-expand-lg bg-white/50 rounded-b-3xl sm:rounded-b-none">
				<div class="container max-w-7xl px-4 mx-auto flex flex-wrap items-center justify-between">
					<div class="w-full relative flex justify-between lg:w-auto px-4 lg:static lg:block lg:justify-start">
						<a class="font-grotesk text-3xl font-bold tracking-tighter flex mr-4 py-2 whitespace-no-wrap text-gray-900 border-b-2 border-green-600" href="/">
							<div class="logo-icon">
								<FaPagelines />
							</div>
							Plantesk
						</a>
						<button class="text-gray-900 cursor-pointer text-xl leading-none px-3 py-1 border border-solid border-transparent rounded bg-transparent block lg:hidden outline-none focus:outline-none" type="button" on:click={toggleNavbar}>
							{#if menuShow === false}
								<span>
									<svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-8 h-8 hover:text-green-600 transition duration-300 hover:scale-150">
										<path stroke-linecap="round" stroke-linejoin="round" d="M3.75 9h16.5m-16.5 6.75h16.5" />
								</svg>									  
								</span>
							{:else}
								<span>
									<svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-8 h-8	hover:text-green-600 transition duration-300 hover:scale-150">
										<path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
									</svg>
								</span>
							{/if}
						</button>
					</div>
					<div class="lg:flex lg:flex-grow items-center {menuShow ? 'flex':'hidden'}">
						<ul class="flex flex-col lg:flex-row list-none lg:ml-auto gap-x-14 mr-4 my-8 lg:my-0">
							<li class="nav-item hover:border-b-2 hover:border-green-600">
								<a on:click={isOpen} class="font-opensans tracking-wider py-4 flex items-center text-md leading-snug text-gray-900 " href="/">
									Sanctuary
								</a>
							</li>
							<li class="nav-item hover:border-b-2 hover:border-green-600">
								<a on:click={isOpen} class="font-opensans tracking-wider py-4 flex items-center text-md leading-snug text-gray-900 " href="/our-team">
									Our Team
								</a>
							</li>
							<li class="nav-item hover:border-b-2 hover:border-green-600">
								<a on:click={isOpen} class="font-opensans tracking-wider py-4 flex items-center text-md leading-snug text-gray-900 " href="/contact">
									Contact
								</a>
							</li>
						</ul>
					</div>
				</div>
			</nav>
		</div>
	</div>	
</header>

<style>
	.logo-icon {
		width: 32px;
		height: 32px;
		margin-right: 3px;
	}
</style>