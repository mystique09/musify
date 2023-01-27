<script>
	import Divider from '$lib/components/Divider.svelte';
	import Button from '$lib/components/Button.svelte';
	import Input from '$lib/components/Input.svelte';
</script>

<svelte:head>
	<title>Musify - Signup</title>
</svelte:head>

<div class="main">
	<div class="signup-fb">
		<h2 class="branding-logo">Musify</h2>
		<div class="para">Sign up for free to start listening.</div>
		<div class="p-2">
			<Button callback="/" size="lg" color="secondary" type="anchor">Signup with Facebook</Button>
			<Divider text="or" />
		</div>
	</div>
	<div class="form-container">
		<form id="signup-form" method="POST" accept-charset="utf-8">
			<h2>Signup with your Email</h2>
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
			<div class="submit-btn-wrapper">
				<Button callback="/" type="submit" size="lg" color="accent">Sign up</Button>
				<p>
					Have an account? <a href="/login">Login.</a>
				</p>
			</div>
		</form>
	</div>
</div>

<style>
	.main {
		@apply bg-white p-4;
	}
	.signup-fb {
		@apply py-4 text-center;
	}
	.branding-logo {
		@apply font-bold text-lg mb-2;
	}
	.para {
		@apply text-2xl font-semibold m-8;
	}
	.form-container {
		@apply px-4;
	}
	h2 {
		@apply text-center font-semibold text-base mb-6;
	}
	.submit-btn-wrapper {
		@apply mt-8 flex flex-col items-center justify-center;
	}
</style>
