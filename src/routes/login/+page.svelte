<script>
	import Button from '$lib/components/Button.svelte';
	import Input from '$lib/components/Input.svelte';
	import Divider from '$lib/components/Divider.svelte';
</script>

<svelte:head>
	<title>Musify - Login</title>
	<meta name="description" content="Musify - Signin to Musify" />
</svelte:head>

<div class="container container-lg m-auto p-4">
	<div class="max-w-lg m-auto">
		<h2 class="text-sm font-bold text-center">To continue, login to Spotify.</h2>
		<div class="m-4 flex flex-col items-center">
			<Button action="/" type="submit" size="lg" color="secondary">FACEBOOK</Button>
			<Button action="/" type="submit" size="lg" color="primary">GOOGLE</Button>
			<Button action="/" type="submit" size="lg" color="bordered">APPLE</Button>
			<Divider text="or" />
		</div>
		<form>
			<Input
				label="Email address or username"
				placeholder="Email address or username"
				name="username"
				id="username"
			/>
			<Input label="Password" placeholder="Password" name="password" id="password" />
			<a class="text-xs text-green-700" href="/forgot-password">Forgot your password?</a>
			<div class="mt-6">
				<Button action="/" type="submit" size="md" color="accent"
					><span class="text-sm">LOG IN</span></Button
				>
			</div>
		</form>
		<Divider text="" />
		<div class="flex flex-col items-center mt-6 font-bold text-black text-sm decoration-none">
			<p class="font-light mb-4">
				Not registered? <a class="text-green-700" href="/signup">Click here to create</a>
			</p>
			<Button action="/premium" type="anchor" size="md" color="bordered">Get premium</Button>
		</div>
	</div>
</div>
