<script>
	export let type;
	export let action;
	export let size;
	export let color;
    export let className = "";
</script>

{#if type === 'anchor'}
	<a class={`btn btn__${size} btn_${color} ${className}`} href={action || '/'}>
		<slot />
	</a>
{/if}
{#if type !== 'anchor'}
	<button {type} class={`btn btn__${size} btn_${color} ${className}`} on:click|preventDefault={action}>
		<slot />
	</button>
{/if}

<style lang="postcss">
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
		@apply text-base  tracking-wider rounded-full py-3 mb-2 font-semibold w-full text-center;
	}
	.btn__sm {
		@apply px-8 text-sm;
	}
	.btn__md {
		@apply px-10 text-base;
	}
	.btn__lg {
		@apply px-24 py-4 text-sm;
	}
	.btn_bordered {
		@apply bg-gray-50 hover:bg-white ring ring-black text-sm;
	}
	.btn_transparent {
		@apply rounded-full text-white bg-transparent ring ring-white;
	}
	a {
		text-decoration: none;
	}
</style>
