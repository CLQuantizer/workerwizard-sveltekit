<script lang="ts">
	import { page } from '$app/state';
	import logo from '$lib/images/svelte-logo.svg';
	import github from '$lib/images/github.svg';
</script>

<header class="flex justify-between items-center px-4 py-4 border-b">
	<div class="w-12 h-12">
		<a href="/" class="flex items-center justify-center w-full h-full">
			<img src={logo} alt="WorkerWizard" class="w-8 h-8 object-contain" />
		</a>
	</div>

	<nav class="flex items-center">
		<ul class="flex items-center space-x-6">
			<li>
				<a 
					href="/" 
					class="text-sm font-medium transition-colors hover:text-primary"
					class:font-bold={page.url.pathname === '/'}
				>
					Home
				</a>
			</li>
			<li>
				<a 
					href="/about" 
					class="text-sm font-medium transition-colors hover:text-primary"
					class:font-bold={page.url.pathname === '/about'}
				>
					About
				</a>
			</li>
			<li>
				<a 
					href="https://github.com/CLQuantizer/workerwizard-sveltekit" 
					target="_blank" 
					rel="noopener noreferrer"
					class="text-sm font-medium transition-colors hover:text-primary"
				>
					GitHub
				</a>
			</li>
		</ul>
	</nav>

	<div class="w-12 h-12">
		<a 
			href="https://sveltekit.workerwizard.com" 
			target="_blank" 
			rel="noopener noreferrer"
			class="flex items-center justify-center w-full h-full"
		>
			<img src={github} alt="Live Demo" class="w-8 h-8 object-contain" />
		</a>
	</div>
</header>