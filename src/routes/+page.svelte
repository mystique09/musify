<svelte:head>
	<title>Musify</title>
	<meta name="description" content="Musify - a Spotify clone made with Sveltekit" />
</svelte:head>

<div
	class="flex items-center justify-center flex-col h-screen relative p-8 text-center bg-blue-800 overflow-hidden"
>
	<div class="circle circle-1" />
	<div class="mb-4">
		<h2 class="text-green-400 font-bold text-2xl md:text-6xl">Listening is everything</h2>
	</div>
	<p class="text-green-400 text-sm md:text-base tracking-wider">
		Millions of songs and podcasts. No credit card needed.
	</p>
	<div class="mt-6 p-6">
		<a
			class="rounded-full bg-green-400 px-10 text-xs md:text-sm md:px-16 py-4 uppercase font-bold text-blue-800 text-none"
			href="/signup">Get Musify free</a
		>
	</div>
	<div class="circle circle-2" />
</div>

<style lang="postcss">
	.circle {
		@apply absolute h-64 w-64 rounded-full bg-green-400;
	}

	.circle-1 {
		@apply -top-24 -right-32;
	}

	.circle-2 {
		@apply -bottom-24 -left-24 h-72 w-72;
	}
</style>
