<script>
	import Divider from '$lib/components/Divider.svelte';
	let toggle = false;
	const toggleNavbar = () => {
		toggle = !toggle;
	};
</script>

<nav class="nav">
	<a href="/">
		<h1>Musify</h1>
	</a>
	<div class="menu md:hidden" on:click={toggleNavbar}>
		<span />
		<span />
		<span />
	</div>
</nav>
<div class="nav-mobile p-6" class:inactive={!toggle} class:active={toggle}>
	<div on:click={toggleNavbar} class="absolute close text-4xl right-4 font-bold">&times;</div>
	<a on:click={toggleNavbar} href="/" class="mt-4 font-bold text-white"> Spotify </a>
	<div class="mb-6">
		<ul>
			<li><a on:click={toggleNavbar} href="/download">Download</a></li>
			<li><a on:click={toggleNavbar} href="/premium">Premium</a></li>
			<li><a on:click={toggleNavbar} href="/terms-and-condition">Terms and Condition</a></li>
		</ul>
	</div>
	<Divider text="" />
</div>

<style>
	.nav {
		@apply px-4 flex items-center justify-between h-16 bg-black z-10;
	}
	.nav a {
		text-decoration: none;
	}
	h1 {
		@apply font-bold text-lg text-white;
	}
	.menu {
		@apply flex flex-col items-center justify-between h-5 w-6;
	}
	span:nth-child(1),
	span:nth-child(3) {
		@apply w-6;
	}
	span {
		@apply rounded-md w-full h-1 bg-white;
	}
	.nav-mobile {
		@apply fixed top-0 bg-black z-50 h-screen w-full;
	}
	.active {
		@apply block left-0;
		animation: slide 500ms;
	}
	.inactive {
		@apply hidden;
	}
	ul {
		@apply flex flex-col mt-12;
	}
	li {
		@apply mt-4;
	}
	li a {
		text-decoration: none;
		@apply font-bold text-2xl;
	}

	@keyframes slide {
		from {
			left: 444px;
			opacity: 0;
		}
		to {
			left: 0;
			opacity: 1;
		}
	}
</style>
