<script>

	let menuShow = false;
		
	function toggleNavbar() {
		menuShow = !menuShow;
	}

</script>

<header class="sticky top-0 z-50 border-2 shadow-lg border-slate-900/[0.06] backdrop-filter backdrop-blur-lg bg-opacity-30">
	<div class="flex flex-wrap">
		<div class="w-full">
			<nav class="relative flex flex-wrap items-center justify-between px-2 py-3 navbar-expand-lg bg-white/50">
				<div class="container max-w-5xl px-4 mx-auto flex flex-wrap items-center justify-between">
					<div class="w-full relative flex justify-between lg:w-auto px-4 lg:static lg:block lg:justify-start">
						<a class="text-3xl font-bold tracking-widest inline-block mr-4 py-2 whitespace-no-wrap text-gray-900 hover:drop-shadow-xl" href="/#">
							nhl
						</a>
						<button class="text-gray-900 cursor-pointer text-xl leading-none px-3 py-1 border border-solid border-transparent rounded bg-transparent block lg:hidden outline-none focus:outline-none" type="button" on:click={toggleNavbar}>
							{#if menuShow === false}
								<span>Open</span>
							{:else}
								<span>Close</span>
							{/if}
						</button>
					</div>
					<div class="lg:flex lg:flex-grow items-center {menuShow ? 'flex':'hidden'}">
						<ul class="flex flex-col lg:flex-row list-none lg:ml-auto">
							<li class="nav-item">
								<a class="px-3 py-2 flex items-center text-md uppercase font-bold leading-snug text-gray-900 hover:opacity-75" href="/#">
									The Team
								</a>
							</li>
							<li class="nav-item">
								<a class="px-3 py-2 flex items-center text-md uppercase font-bold leading-snug text-gray-900 hover:opacity-75" href="/#">
									Statistics
								</a>
							</li>
							<li class="nav-item">
								<a class="px-3 py-2 flex items-center text-md uppercase font-bold leading-snug text-gray-900 hover:opacity-75" href="/#">
									Gallery
								</a>
							</li>
						</ul>
					</div>
				</div>
			</nav>
		</div>
	</div>
</header>