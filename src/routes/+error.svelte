<script>
	import { page } from '$app/stores';
</script>

<svelte:head>
	<title>Musify - ${$page.status} {$page.error.message}</title>
	<meta name="description" content={$page.error.message} />
</svelte:head>

<div class="min-h-screen bg-green-400 w-full p-2">
	<div class="h-screen w-full max-w-2xl m-auto">
		<div class="h-full flex flex-col items-center justify-center gap-2">
			<div class="text-center text-2xl md:text-5xl font-bold text-black">
				{$page.status}
				{$page.error.message}
			</div>
			<p class="text-center text-sm md:text-base font-normal text-black">
				The page you are looking for does not exist.
			</p>
			<a class="underline text-sm md:text-base font-light underline-offset-4" href="/"
				>Go back to homepage</a
			>
		</div>
	</div>
</div>
