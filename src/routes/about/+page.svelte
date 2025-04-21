<script lang="ts">
	import { Card, CardContent, CardDescription, CardHeader, CardTitle } from "$lib/components/ui/card";
	import { 
		Code2, 
		Cloud, 
		Globe, 
		Rocket, 
		Zap, 
		Wrench,
		ArrowRight,
		BookOpen,
		Lightbulb,
		Users
	} from 'lucide-svelte';
</script>

<svelte:head>
	<title>About WorkerWizard</title>
	<meta name="description" content="Learn about WorkerWizard - Deploy SvelteKit to Cloudflare Workers" />
</svelte:head>

<section class="py-16 px-4">
	<div class="max-w-4xl mx-auto">
		<div class="text-center mb-16">
			<h1 class="text-4xl font-bold mb-4">About WorkerWizard</h1>
			<p class="text-xl text-muted-foreground">
				Simplifying SvelteKit deployments to Cloudflare Workers
			</p>
		</div>

		<div class="grid grid-cols-1 md:grid-cols-2 gap-8 mb-16">
			<Card>
				<CardHeader>
					<CardTitle class="flex items-center gap-2">
						<Lightbulb class="w-6 h-6 text-primary" />
						Our Mission
					</CardTitle>
				</CardHeader>
				<CardContent>
					<CardDescription>
						WorkerWizard was created to make deploying SvelteKit applications to Cloudflare Workers as simple as possible. We believe in the power of edge computing and want to help developers leverage it effectively.
					</CardDescription>
				</CardContent>
			</Card>

			<Card>
				<CardHeader>
					<CardTitle class="flex items-center gap-2">
						<Users class="w-6 h-6 text-primary" />
						For Developers
					</CardTitle>
				</CardHeader>
				<CardContent>
					<CardDescription>
						Built by developers, for developers. WorkerWizard is open source and community-driven, with a focus on simplicity and best practices.
					</CardDescription>
				</CardContent>
			</Card>
		</div>

		<div class="grid grid-cols-1 md:grid-cols-3 gap-8 mb-16">
			<Card>
				<CardHeader>
					<CardTitle class="flex items-center gap-2">
						<Code2 class="w-6 h-6 text-primary" />
						Modern Stack
					</CardTitle>
				</CardHeader>
				<CardContent>
					<CardDescription>
						Built with SvelteKit, TypeScript, and the latest web technologies for a modern development experience.
					</CardDescription>
				</CardContent>
			</Card>

			<Card>
				<CardHeader>
					<CardTitle class="flex items-center gap-2">
						<Cloud class="w-6 h-6 text-primary" />
						Cloudflare Workers
					</CardTitle>
				</CardHeader>
				<CardContent>
					<CardDescription>
						Leverage Cloudflare's global edge network for lightning-fast performance and global distribution.
					</CardDescription>
				</CardContent>
			</Card>

			<Card>
				<CardHeader>
					<CardTitle class="flex items-center gap-2">
						<BookOpen class="w-6 h-6 text-primary" />
						Documentation
					</CardTitle>
				</CardHeader>
				<CardContent>
					<CardDescription>
						Comprehensive documentation and examples to help you get started quickly.
					</CardDescription>
				</CardContent>
			</Card>
		</div>

		<div class="text-center">
			<h2 class="text-2xl font-bold mb-4">Ready to Get Started?</h2>
			<p class="text-muted-foreground mb-8">
				Join the growing community of developers using WorkerWizard
			</p>
			<a href="https://github.com/CLQuantizer/workerwizard-sveltekit" target="_blank" rel="noopener noreferrer">
				<button class="inline-flex items-center justify-center rounded-md text-sm font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 bg-primary text-primary-foreground hover:bg-primary/90 h-10 px-4 py-2">
					View on GitHub
					<ArrowRight class="w-4 h-4 ml-2" />
				</button>
			</a>
		</div>
	</div>
</section>
