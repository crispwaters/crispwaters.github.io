<script lang="ts">
	import favicon from '$lib/assets/favicon.ico';
	import '../app.css';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<div class="bg-blue-200 dark:bg-gray-950 min-h-svh">
	{@render children()}
</div>
