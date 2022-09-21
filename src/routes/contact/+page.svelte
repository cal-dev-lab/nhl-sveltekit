<script>
import Animate from "../../lib/Animate.svelte";

</script>

<svelte:head>
	<title>Get in touch | Plantesk</title>
	<meta name="description" content="Contact Plantesk" />
	<link rel="canonical" href="https://plantesk.netlify.app/contact/" />
</svelte:head>

<Animate>
	<div class="max-w-7xl mx-auto py-16 px-4 sm:py-10 sm:px-6 lg:px-8">
		<div class="grid grid-cols-1 gap-y-10 sm:grid-cols-2 gap-x-6 xl:gap-x-8 mx-auto justify-center items-center bg-white p-10 rounded-3xl">
			<div class="w-full h-full z-10">
				<img 
					class="z-10 h-full aspect-auto object-cover md:rounded-l-3xl md:rounded-tr-none rounded-t-3xl hover:scale-90 transition duration-300 md:w-full"
					src={'https://plantesk.sirv.com/plantesk/contact/image.jpg'} alt="title"
					width="600"
				/>
			</div>
			<div>
				<h2 class="z-50 text-5xl md:text-6xl lg:text-7xl font-grotesk font-bold text-center md:text-left">
					Get in touch
				</h2>
				<p class="text-justify mt-5 font-opensans tracking-widest">
					We want to connect with you as much as we want you to connect with nature!
					<span class="font-bold">We would love to hear from you.</span>
				</p>
				<!-- START: Form -->
				<div class="w-full mt-5">
					<form class="space-y-4 font-opensans" id="form">
						<!-- Name -->
						<div>
							<input
								type="text"
								class="border-2 border-gray-200 w-full p-2 rounded outline-none focus:border-green-500"
								id="user_name"
								name="user_name"
								placeholder="Your name"
							/>
						</div>
						<!-- Email -->
						<div>
							<input
								type="email"
								class="border-2 border-gray-200 w-full p-2 rounded outline-none focus:border-green-500"
								id="user_email"
								name="user_email"
								placeholder="we.love@nature.com"
							/>
						</div>
						<!-- Comment -->
						<div>
							<p>Enter message</p>
							<textarea  class="w-full h-16 px-3 py-2 text-base text-gray-700 placeholder-gray-600 border rounded-lg focus:border-green-500"></textarea>
						</div>
						<!-- Checkbox -->
						<div class="flex items-center">
							<input type="checkbox" id="agree" />
							<label for="agree" class="ml-2 text-sm">
								I agree to the terms and conditions.
							</label>
						</div>
						<!-- Submit -->
						<!-- Should be a button -->
						<a
							href="/"
							class="block bg-green-100 text-green-500 hover:bg-green-300 hover:text-white transition duration-300 w-full p-2 rounded text-center"
						>
							Submit
						</a>
					</form>
				</div>
				<!-- END: Form -->
			</div>
		</div>
	</div>
</Animate>