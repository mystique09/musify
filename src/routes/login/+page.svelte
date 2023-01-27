<script>
	import Button from '$lib/components/Button.svelte';
	import Input from '$lib/components/Input.svelte';
	import Divider from '$lib/components/Divider.svelte';
</script>

<svelte:head>
	<title>Musify - Login</title>
</svelte:head>

<div class="container md:flex md:flex-col md:items-center">
	<h2>To continue, login to Spotify.</h2>
	<div class="options">
		<Button callback="/" type="submit" size="md" color="secondary">CONTINUE WITH FACEBOOK</Button>
		<Button callback="/" type="submit" size="md" color="primary">CONTINUE WITH GOOGLE</Button>
		<Button callback="/" type="submit" size="md" color="bordered">CONINUE WITH APPLE</Button>
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
		<a class="forgot-password" href="/forgot-password">Forgot your password?</a>
		<div class="container">
			<Button callback="/" type="submit" size="lg" color="accent"
				><span class="text-sm">LOG IN</span></Button
			>
		</div>
	</form>
</div>
<Divider text="" />
<div class="no-account">
	<a href="/signup">Don't have an account?</a>
	<div class="flex items-center mt-2">
		<Button callback="/premium" type="anchor" size="lg" color="bordered">SIGN UP FOR MUSIFY</Button>
	</div>
</div>

<style>
	.container {
		@apply p-4;
	}
	h2 {
		@apply text-sm font-bold text-center;
	}
	.options {
		@apply m-4 flex flex-col items-center;
	}
	.no-account {
		@apply flex flex-col items-center mt-6;
	}

	.no-account a {
		text-decoration: none;
		@apply font-bold text-black text-sm;
	}
</style>
