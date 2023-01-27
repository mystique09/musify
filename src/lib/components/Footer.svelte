<script>
	import Navigator from '$lib/components/Navigator.svelte';
</script>

<footer class="bg-black">
	<div class="px-4 py-6 flex flex-col justify-between">
		<div class="mt-4 flex items-start text-white">
			<a class="text-white" href="/">
				<h3 class="text-2xl font-bold tracking-wider text-green-400">Musify</h3>
			</a>
		</div>
		<div class="mt-8 flex flex-col items-start justify-between">
			<Navigator url="/" heading="Company" list={['About', 'Jobs', 'For The Record']} />
			<Navigator
				url="/"
				heading="Community"
				list={['For Artist', 'Developers', 'Advertising', 'Inventors', 'Vendors']}
			/>
			<Navigator url="/" heading="Useful Links" list={['Support', 'Web Player', 'Mobile App']} />
		</div>
		<div class="flex flex-row h-24 items-end text-xs">
			<div class="text-white mr-4">
				<a rel="noreferrer" href="https://github.com/mystique09">
					<span>Github</span>
				</a>
			</div>
			<div class="text-white mr-4">
				<a rel="noreferrer" href="https://www.linkedin.com/in/benjie-ben-garcia-916261202">
					<span>LinkedIn</span>
				</a>
			</div>
		</div>
	</div>
</footer>
