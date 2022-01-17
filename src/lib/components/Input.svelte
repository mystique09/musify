<script>
	export let name;
	export let id;
	export let placeholder;
	export let label;
</script>

<label for={name}>{label}</label>
<div class="input-container">
	<input {placeholder} type="text" {name} {id} />
</div>

<style>
	.input-container {
		@apply mb-6;
	}
	input {
		@apply rounded-md outline outline-gray-300 py-4 px-2 w-full;
	}
	label {
		@apply font-bold text-sm;
	}
</style>
