<script lang="ts">
	import Navbar from '$lib/components/navbar.svelte';
	import Lenis from 'lenis';
	import '../app.css';
	import { browser } from '$app/environment';
	let { children } = $props();

	if (browser) {
		new Lenis({
			autoRaf: true
		});
	}
</script>

<Navbar />

{@render children()}

<style>
	:global(html) {
		scroll-behavior: smooth;
		color: #90a1b9;
	}
</style>
