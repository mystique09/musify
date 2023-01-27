<script>
	import Button from '$lib/components/Button.svelte';
</script>

<svelte:head>
	<title>Musify - Premium Subscription</title>
    <meta name="description" content="Musify - Premium" />
</svelte:head>

<div class="min-h-screen">
	<div class="bg-blue-600">
		<div class="max-w-xl m-auto text-center p-6 h-96 ">
			<h2 class="font-bold text-white text-2xl">Get Premium free for 1 month</h2>
			<p class="mt-2 font-normal text-lg text-white">Just ₱129/month after. Cancel anytime.</p>

			<div class="options flex flex-col mt-6">
				<Button action="/" type="anchor" size="md" color="primary">Get Started</Button>
				<Button action="/" type="anchor" size="md" color="transparent">View Plans</Button>
			</div>
			<p class="font-light text-sm text-white mt-4">
				<a class="text-green-400" href="/terms-and-condition">Terms and conditions apply.</a> 1 month
				free not available for users who have already tried Premium.
			</p>
		</div>
	</div>
	<div class="bg-indigo-700">
		<div class="max-w-xl m-auto text-center p-6 h-96">
			<h2 class="font-bold text-white text-2xl">Introducing Premium Mini</h2>
			<p class="mt-2 font-normal text-lg text-white">
				30 song downloads and unlimited ad-free music listening, on 1 mobile device.
			</p>

			<div class="options flex flex-col mt-6">
				<Button action="/" type="anchor" size="md" color="primary">GET 1 DAY FOR ₱7</Button>
				<Button action="/" type="anchor" size="md" color="transparent">GET 1 WEEK FOR ₱26</Button>
			</div>
			<p class="font-light text-sm text-green-400 mt-8">
				<a href="/terms-and-condition">Terms and conditions apply.</a>
			</p>
		</div>
	</div>
</div>
