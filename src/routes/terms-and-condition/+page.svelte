<script>
	import Button from '$lib/components/Button.svelte';
</script>

<svelte:head>
	<title>Musify - Terms and Condition</title>
	<meta name="description" content="Musify - a Spotify clone made with Sveltekit" />
</svelte:head>

<div class="min-h-screen">
	<div class="bg-blue-600">
		<div
			class="h-screen max-w-2xl m-auto text-center text-white flex flex-col items-center justify-center p-2"
		>
			<h2 class="mb-4 font-bold text-2xl md:text-6xl tracking-wide">Terms and Condition</h2>
			<p class="mb-6 font-light text-sm tracking-wider">
				This website is not the official Spotify website, this is just a hobby project hosten on
				vercel. So, don't abuse the website.
			</p>
			<Button type="anchor" className="text-green-400" size="sm" color="" action="/"
				>Go back to Homepage</Button
			>
		</div>
	</div>
</div>
