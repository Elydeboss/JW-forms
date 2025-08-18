<script lang="ts">
	import { TextInput } from 'carbon-components-svelte';
	import { Link } from 'carbon-components-svelte';
	import { Theme, Button } from 'carbon-components-svelte';
	import 'carbon-components-svelte/css/all.css';
</script>

<main
	class="container mx-auto mt-8 p-4 bg-gray-600 w-[600px] h-[400px] flex flex-col justify-center"
>
	<div class="h-[1000px] container mt-6">
		<div class="mx-4 my-4 flex items-center text-white">
			<div class="mr-6 rounded bg-[#3d70b2] py-5 px-2 font-bold">JW.ORG</div>
			<h1 class="text-2xl font-light">Create Account</h1>
		</div>

		<div class="flex flex-col mx-4">
			<div class="gap-4 my-4 flex flex-col">
				<TextInput size="xl" labelText="User name" placeholder="Enter user name..." />
			</div>

			<!--button-->
			<Theme theme="g100" />

			<div class="text-center items-center px-12 py-4">
				<Button class="w-full">Next</Button>
			</div>
		</div>
	</div>
</main>
