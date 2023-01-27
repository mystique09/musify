<script>
	import Divider from '$lib/components/Divider.svelte';
	import { slide } from 'svelte/transition';
	let toggle = false;
	const toggleNavbar = () => {
		toggle = !toggle;
	};
</script>

<nav class="px-4 flex items-center justify-between h-16 bg-black z-10">
	<a class="decoration-none" href="/">
		<h1 class="font-bold text-xl text-green-400 tracking-wider">Musify</h1>
	</a>
	<ul
		class="hidden md:flex md:flex-row md:items-center md:justify-between md:gap-4 text-xs text-white font-bold tracking-wider"
	>
		<li><a href="/download">Download</a></li>
		<li><a href="/premium">Premium</a></li>
		<li><a href="/terms-and-condition">Terms and Condition</a></li>
	</ul>
	<div class="block md:hidden" on:click={toggleNavbar} on:keydown={toggleNavbar}>
		<svg
			xmlns="http://www.w3.org/2000/svg"
			fill="none"
			viewBox="0 0 24 24"
			stroke-width="1.5"
			stroke="currentColor"
			class="w-6 h-6 md:w-12 md:h-12 stroke-white"
		>
			<path stroke-linecap="round" stroke-linejoin="round" d="M3.75 9h16.5m-16.5 6.75h16.5" />
		</svg>
	</div>
</nav>
{#if toggle}
	<div
		in:slide={{ duration: 500 }}
		out:slide={{ duration: 400 }}
		class="fixed top-0 bg-black z-50 h-screen w-full p-6"
		class:inactive={!toggle}
		class:active={toggle}
	>
		<div
			on:click={toggleNavbar}
			on:keydown={toggleNavbar}
			class="absolute close text-4xl right-4 font-bold text-white"
		>
			<svg
				xmlns="http://www.w3.org/2000/svg"
				fill="none"
				viewBox="0 0 24 24"
				stroke-width="1.5"
				stroke="currentColor"
				class="w-6 h-6"
			>
				<path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
			</svg>
		</div>
		<a on:click={toggleNavbar} href="/" class="mt-4 font-bold text-green-400"> Musify </a>
		<div class="mb-6 text-white">
			<ul class="flex flex-col mt-12">
				<li class="mt-4">
					<a class="font-bold text-2xl" on:click={toggleNavbar} href="/download">Download</a>
				</li>
				<li class="mt-4">
					<a class="font-bold text-2xl" on:click={toggleNavbar} href="/premium">Premium</a>
				</li>
				<li class="mt-4">
					<a class="font-bold text-2xl" on:click={toggleNavbar} href="/terms-and-condition"
						>Terms and Condition</a
					>
				</li>
			</ul>
		</div>
		<Divider text="" />
	</div>
{/if}
