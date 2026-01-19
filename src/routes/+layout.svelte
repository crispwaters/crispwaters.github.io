<script lang="ts">
	import favicon from '$lib/assets/favicon.svg';
	import "../app.css";

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<div class="h-screen grid grid-rows-[auto_1fr_auto]">
	<!-- Header -->
	<header class="p-4">(header)</header>
	<!-- Main -->
	<main class="p-4 space-y-4">
		{@render children()}
	</main>
	<!-- Footer -->
	<footer class="p-4">(footer)</footer>
</div>


