<svelte:head>
	<title>Musify - Download</title>
</svelte:head>

<div class="download">
	<h2 class="premium-h1">Download Musify</h2>
	<p>Play millions of songs and podcasts on your device.</p>
	<button class="mt-6 py-4 px-12 bg-white rounded-full text-sm font-bold">Download</button>
</div>
<div class="features">
	<h2 class="premium-h2">One account, listen everywhere.</h2>
	<ul>
		<li>MOBILE</li>
		<li>COMPUTER</li>
		<li>TABLET</li>
		<li><a href="/">CAR</a></li>
		<li><a href="/">PLAYSTATION</a></li>
		<li><a href="/">XBOX</a></li>
		<li><a href="/">TV</a></li>
		<li><a href="/">SPEAKER</a></li>
		<li><a href="/">WEB PLAYER</a></li>
	</ul>
</div>

<style>
	.download {
		@apply bg-green-400 h-96 flex flex-col items-center justify-center text-center;
	}

	.premium-h1 {
		@apply text-2xl font-bold text-black mb-2;
	}
	p {
		@apply mb-2;
	}
	.features {
		@apply flex flex-col items-center justify-center h-screen bg-black text-center;
	}
	.premium-h2 {
		@apply font-bold text-4xl text-white;
	}
	ul {
		@apply mt-6 flex flex-col gap-4;
	}
	li {
		@apply text-white;
	}
</style>
