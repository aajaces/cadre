<script lang="ts">
	import "../app.css";
	import favicon from "$lib/assets/favicon.svg";

	let { children } = $props();
	import { injectAnalytics } from "@vercel/analytics/sveltekit";
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<script
		src="https://code.iconify.design/iconify-icon/2.1.0/iconify-icon.min.js"
	></script>
</svelte:head>

{@render children()}
