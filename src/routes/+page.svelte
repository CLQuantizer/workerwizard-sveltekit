<script lang="ts">
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcomeFallback from '$lib/images/svelte-welcome.png';
	import { Button } from "$lib/components/ui/button";
	import { Card, CardContent, CardDescription, CardHeader, CardTitle } from "$lib/components/ui/card";
	import { Tooltip, TooltipContent, TooltipTrigger } from "$lib/components/ui/tooltip";
	import { Avatar, AvatarFallback, AvatarImage } from "$lib/components/ui/avatar";
	import { 
		Rocket, 
		Zap, 
		Wrench, 
		Globe, 
		Code2, 
		Cloud, 
		Github, 
		ExternalLink,
		ArrowRight
	} from 'lucide-svelte';
</script>

<svelte:head>
	<title>WorkerWizard - SvelteKit on Cloudflare Workers</title>
	<meta name="description" content="Deploy your SvelteKit applications to Cloudflare Workers with ease" />
</svelte:head>

<section class="min-h-[80vh] flex flex-col justify-center items-center px-4 py-16 text-center">
	<div class="max-w-3xl mx-auto">
		<div class="relative w-full aspect-[2048/495] mb-8">
			<picture>
				<source srcset={welcome} type="image/webp" />
				<img 
					src={welcomeFallback} 
					alt="Welcome" 
					class="absolute inset-0 w-full h-full object-contain"
				/>
			</picture>
		</div>

		<h1 class="text-4xl md:text-5xl font-bold mb-4">
			Deploy SvelteKit to<br />Cloudflare Workers
		</h1>

		<p class="text-xl text-muted-foreground mb-8">
			A streamlined solution for deploying SvelteKit applications to Cloudflare Workers
		</p>

		<div class="flex flex-col sm:flex-row gap-4 justify-center">
			<Tooltip>
				<TooltipTrigger>
					<a href="https://github.com/CLQuantizer/workerwizard-sveltekit" target="_blank" rel="noopener noreferrer">
						<Button size="lg" class="flex items-center gap-2">
							<Github class="w-5 h-5" />
							View on GitHub
						</Button>
					</a>
				</TooltipTrigger>
				<TooltipContent>
					<p>Check out the source code</p>
				</TooltipContent>
			</Tooltip>

			<Tooltip>
				<TooltipTrigger>
					<a href="https://sveltekit.workerwizard.com" target="_blank" rel="noopener noreferrer">
						<Button variant="outline" size="lg" class="flex items-center gap-2">
							<ExternalLink class="w-5 h-5" />
							Live Demo
						</Button>
					</a>
				</TooltipTrigger>
				<TooltipContent>
					<p>See it in action</p>
				</TooltipContent>
			</Tooltip>
		</div>
	</div>
</section>

<section class="py-16 px-4 bg-muted">
	<div class="max-w-6xl mx-auto">
		<div class="grid grid-cols-1 md:grid-cols-3 gap-8">
			<Card>
				<CardHeader>
					<CardTitle class="flex items-center gap-2">
						<Rocket class="w-6 h-6 text-primary" />
						Fast Deployment
					</CardTitle>
				</CardHeader>
				<CardContent>
					<CardDescription>
						Deploy your SvelteKit applications to Cloudflare Workers in minutes
					</CardDescription>
				</CardContent>
			</Card>

			<Card>
				<CardHeader>
					<CardTitle class="flex items-center gap-2">
						<Zap class="w-6 h-6 text-primary" />
						Edge Computing
					</CardTitle>
				</CardHeader>
				<CardContent>
					<CardDescription>
						Leverage Cloudflare's global network for lightning-fast performance
					</CardDescription>
				</CardContent>
			</Card>

			<Card>
				<CardHeader>
					<CardTitle class="flex items-center gap-2">
						<Wrench class="w-6 h-6 text-primary" />
						Easy Setup
					</CardTitle>
				</CardHeader>
				<CardContent>
					<CardDescription>
						Simple configuration and deployment process
					</CardDescription>
				</CardContent>
			</Card>
		</div>

		<div class="mt-16 grid grid-cols-1 md:grid-cols-2 gap-8">
			<Card>
				<CardHeader>
					<CardTitle class="flex items-center gap-2">
						<Globe class="w-6 h-6 text-primary" />
						Global Distribution
					</CardTitle>
				</CardHeader>
				<CardContent>
					<CardDescription>
						Your app runs on Cloudflare's edge network, ensuring low latency worldwide
					</CardDescription>
				</CardContent>
			</Card>

			<Card>
				<CardHeader>
					<CardTitle class="flex items-center gap-2">
						<Code2 class="w-6 h-6 text-primary" />
						Modern Stack
					</CardTitle>
				</CardHeader>
				<CardContent>
					<CardDescription>
						Built with SvelteKit and TypeScript for a modern development experience
					</CardDescription>
				</CardContent>
			</Card>
		</div>
	</div>
</section>

<section class="py-16 px-4">
	<div class="max-w-4xl mx-auto text-center">
		<h2 class="text-3xl font-bold mb-6">Ready to Get Started?</h2>
		<p class="text-xl text-muted-foreground mb-8">
			Deploy your SvelteKit app to Cloudflare Workers today
		</p>
		<div class="flex justify-center">
			<a href="https://github.com/CLQuantizer/workerwizard-sveltekit" target="_blank" rel="noopener noreferrer">
				<Button size="lg" class="flex items-center gap-2">
					Get Started
					<ArrowRight class="w-5 h-5" />
				</Button>
			</a>
		</div>
	</div>
</section>
