<script lang="ts">
	import '../app.css';
	import { TextInput } from 'carbon-components-svelte';
	import { Link } from 'carbon-components-svelte';
	import { Theme, Button } from 'carbon-components-svelte';
	import 'carbon-components-svelte/css/all.css';

	let { children } = $props();
</script>

{@render children?.()}

<main
	class="container mt-6 mb-4 sm:mt-20 mx-auto bg-[#262424] w-full sm:max-w-[500px] flex flex-col justify-center"
>
	<div class="container p-8 gap-y-8 flex flex-col">
		<div class="flex items-center text-white">
			<div class="mr-3 rounded bg-[#3d70b2] py-5 px-2 font-bold">JW.ORG</div>
			<h1 class="text-2xl font-light">Log In</h1>
		</div>

		<div class="flex flex-col">
			<div class="gap-4 mb-2 flex flex-col">
				<theme theme="g80">
					<TextInput size="xl" labelText="User name" />
				</theme>
			</div>
			<Link href="https://www.carbondesignsystem.com/" target="_blank" class="text-blue-500 mb-4">
				forgot password?</Link
			>
			<!--button-->
			<Theme theme="g100" />

			<div class="flex justify-center my-4 bg-blue-500 p-4">Next</div>

			<!-- Divider OR -->
			<div class="flex justify-center text-sm text-[#8b8684]">
				<span class=" px-3">OR</span>
			</div>

			<!-- Passkey Button -->

			<button
				class="flex my-4 bg-[#22202000] p-4 cursor-pointer justify-center items-center text-center border-2 border-blue-500 w-full"
			>
				Use a Passkey to Log In
			</button>
		</div>
	</div>
</main>

<div class="pb-4 flex flex-col items-center justify-center">
	<div class="mb-4">
		<h4>Do you need an account?</h4>
	</div>

	<a href="/signup">
		<Button kind="secondary" class="w-full">Create New Account</Button>
	</a>
</div>
