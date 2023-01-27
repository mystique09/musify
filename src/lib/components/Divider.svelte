<script>
	export let text;
</script>

<div class="container">
	<div class:divider={text} class:full={!text}>
		{#if text}
			<span>{text}</span>
		{/if}
	</div>
</div>

<style lang="postcss">
	.container {
		@apply relative w-full;
	}
	.divider {
		@apply m-6 font-thin relative text-center;
	}
	.full {
		@apply w-full h-[1px] bg-gray-300;
	}
	.divider::before,
	.divider::after {
		content: '';
		@apply absolute h-[1px] w-[105px] bg-gray-300;
	}
	.divider::before {
		@apply left-2 top-3;
	}
	.divider::after {
		@apply right-2 top-3;
	}
</style>
