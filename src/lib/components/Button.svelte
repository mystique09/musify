<script>
	export let type;
	export let callback;
	export let size;
	export let color;
</script>

{#if type === 'anchor'}
	<a class={`btn btn__${size} btn_${color}`} href={callback || '/'}>
		<slot />
	</a>
{/if}
{#if type !== 'anchor'}
	<button {type} class={`btn btn__${size} btn_${color}`} on:click|preventDefault={callback}>
		<slot />
	</button>
{/if}

<style>
	.btn_primary {
		@apply bg-black text-white;
	}
	.btn_secondary {
		@apply bg-blue-600 text-white;
	}
	.btn_accent {
		@apply bg-green-600 text-white;
	}
	.btn {
		@apply text-base rounded-full py-3 mb-2 font-semibold w-full text-center;
	}
	.btn__sm {
		@apply px-8 text-sm;
	}
	.btn__md {
		@apply px-10 text-base;
	}
	.btn__lg {
		@apply px-16 text-lg;
	}
	.btn_bordered {
		@apply bg-white text-gray-400 text-base outline-none ring ring-black rounded-full font-semibold;
	}
	.btn_transparent {
		@apply rounded-full text-white font-semibold bg-transparent ring ring-white;
	}
	a {
		text-decoration: none;
	}
</style>
