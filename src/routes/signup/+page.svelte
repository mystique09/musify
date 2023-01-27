<script>
	import Divider from '$lib/components/Divider.svelte';
	import Button from '$lib/components/Button.svelte';
	import Input from '$lib/components/Input.svelte';
</script>

<svelte:head>
	<title>Musify - Signup</title>
	<meta name="description" content="Musify - Signup to Musify for free" />
</svelte:head>


<div class="bg-white p-4">
	<div class="max-w-lg m-auto">
		<div class="py-4 text-center">
			<h2 class="font-bold text-lg mb-2">Musify</h2>
			<div class="text-2xl font-semibold m-8">Sign up for free to start listening.</div>
			<div class="p-2">
				<Button action="/" size="lg" color="secondary" type="anchor">Facebook</Button>
				<Divider text="or" />
			</div>
		</div>
		<div class="px-4">
			<form id="signup-form" method="POST">
				<h2 class="text-center font-semibold text-base mb-6">Signup with your Email</h2>
				<Input label="What's your Email?" placeholder="Enter your Email." name="email" id="email" />
				<Input
					label="Confirm your Email"
					placeholder="Enter your Email again."
					name="cornfirm_email"
					id="cornfirm_email"
				/>
				<Input
					label="Create a password"
					placeholder="Create a password."
					name="password"
					id="password"
				/>
				<Input
					label="What should we call you?"
					placeholder="Enter your profile name."
					name="password"
					id="password"
				/>
				<p class="-mt-4 text-sm">This appears on your profile</p>
				<div class="mt-8 flex flex-col items-start justify-center">
					<Button action="/" type="submit" size="md" color="accent">Sign up</Button>
					<p class="text-sm">
						Already have an account? <a class="text-green-700" href="/login">Login.</a>
					</p>
				</div>
			</form>
		</div>
	</div>
</div>
