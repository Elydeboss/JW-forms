<script lang="ts">
	import '../app.css';
	import { TextInput } from 'carbon-components-svelte';
	import { Link } from 'carbon-components-svelte';
	import { Theme, Button } from 'carbon-components-svelte';
	import 'carbon-components-svelte/css/all.css';

	let { children } = $props();
</script>

{@render children?.()}
