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
	class="container mx-auto mt-8 p-4 bg-[#222020] w-[550px] h-[400px] flex flex-col justify-center"
>
	<div class="h-[1000px] container mt-6">
		<div class="mx-4 mb-6 flex items-center text-white">
			<div class="mr-3 rounded bg-[#3d70b2] py-5 px-2 font-bold">JW.ORG</div>
			<h1 class="text-2xl font-light">Log In</h1>
		</div>

		<div class="flex flex-col mx-4">
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

			<div class="text-center items-center px-12 py-4">
				<Button class="w-full">Next</Button>
			</div>

			<!-- Divider OR -->
			<div class=" text-sm text-[#8b8684] text-center items-center mb-4">
				<span class=" px-3">OR</span>
			</div>

			<!-- Passkey Button -->
			<div class=" text-center items-center mb-8">
				<Button kind="tertiary" class="w-full">Use a Passkey to Log In</Button>
			</div>
		</div>
	</div>
</main>

<div class="container mx-auto mt-8 p-4 flex flex-col items-center justify-center">
	<div class="mb-4">
		<h4>do you need an account?</h4>
	</div>
	<div>
		<a href="/signup">
			<Button kind="secondary" class="w-full">Create One</Button>
		</a>
	</div>
</div>
