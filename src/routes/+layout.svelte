<script lang="ts">
	import Header from './Header.svelte';
	import '../app.css';
	
	let { children } = $props();
</script>

<div class="min-h-screen flex flex-col">
	<Header />

	<main class="flex-1">
		{@render children()}
	</main>
</div>
