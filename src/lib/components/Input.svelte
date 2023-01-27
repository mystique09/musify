<script>
	export let name;
	export let id;
	export let placeholder;
	export let label;
</script>

<label class="font-light text-sm" for={name}>{label}</label>
<div class="mb-6">
	<input
		class="focus:border-none focus:outline-none duration-150 rounded-sm ring ring-gray-400 hover:ring hover:ring-green-400 text-base py-2 px-2 w-full"
		{placeholder}
		type="text"
		{name}
		{id}
	/>
</div>
