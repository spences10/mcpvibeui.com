<script lang="ts">
	import claymorphic from '$lib/assets/themes/claymorphic-theme.webp';
	import cyberpunk from '$lib/assets/themes/cyberpunk-theme.webp';
	import editorial from '$lib/assets/themes/editorial-theme.webp';
	import flat from '$lib/assets/themes/flat-theme.webp';
	import glassmorphic from '$lib/assets/themes/glassmorphic-theme.webp';
	import industrial from '$lib/assets/themes/industrial-theme.webp';
	import japaneseMinimalist from '$lib/assets/themes/japanese-minimalist-theme.webp';
	import monochrome from '$lib/assets/themes/monochrome-theme.webp';
	import neuBrutalist from '$lib/assets/themes/neu-brutalist-theme.webp';
	import neumorphic from '$lib/assets/themes/neumorphic-theme.webp';
	import organicFlow from '$lib/assets/themes/organic-flow-theme.webp';
	import pixelArt from '$lib/assets/themes/pixel-art-theme.webp';
	import retroFuturism from '$lib/assets/themes/retro-futurism-theme.webp';
	import typographic from '$lib/assets/themes/typographic-theme.webp';
	import wireframe from '$lib/assets/themes/wireframe-theme.webp';
	import type { SchemaOrgProps, SeoConfig } from 'svead';
	import { Head, SchemaOrg } from 'svead';
	import { fade, fly } from 'svelte/transition';

	const themes = [
		{ name: 'Cyberpunk', slug: 'cyberpunk', img: cyberpunk },
		{ name: 'Glassmorphic', slug: 'glassmorphic', img: glassmorphic },
		{ name: 'Neumorphic', slug: 'neumorphic', img: neumorphic },
		{
			name: 'Neu-Brutalist',
			slug: 'neu-brutalist',
			img: neuBrutalist,
		},
		{ name: 'Claymorphic', slug: 'claymorphic', img: claymorphic },
		{ name: 'Editorial', slug: 'editorial', img: editorial },
		{ name: 'Flat', slug: 'flat', img: flat },
		{ name: 'Industrial', slug: 'industrial', img: industrial },
		{
			name: 'Japanese Minimalist',
			slug: 'japanese-minimalist',
			img: japaneseMinimalist,
		},
		{ name: 'Monochrome', slug: 'monochrome', img: monochrome },
		{ name: 'Organic Flow', slug: 'organic-flow', img: organicFlow },
		{ name: 'Pixel Art', slug: 'pixel-art', img: pixelArt },
		{
			name: 'Retro Futurism',
			slug: 'retro-futurism',
			img: retroFuturism,
		},
		{ name: 'Typographic', slug: 'typographic', img: typographic },
		{ name: 'Wireframe', slug: 'wireframe', img: wireframe },
	];

	let current_index = $state(0);
	let is_paused = $state(false);

	$effect(() => {
		if (is_paused) return;
		const interval = setInterval(() => {
			current_index = (current_index + 1) % themes.length;
		}, 5000);
		return () => clearInterval(interval);
	});

	const seo_config: SeoConfig = {
		title: 'mcp-vibe-ui — Design Tokens for AI-Generated Interfaces',
		description:
			'An MCP server that provides complete design systems to LLMs. 15 production themes with Tailwind v4 CSS, component patterns, typography, and effects.',
		url: 'https://mcpvibeui.com',
	};

	const schema_org: SchemaOrgProps['schema'] = {
		'@type': 'SoftwareApplication',
		name: 'mcp-vibe-ui',
		applicationCategory: 'DeveloperApplication',
		operatingSystem: 'Any',
		description:
			'MCP server providing design tokens for LLM-powered UI generation with 15 distinct themes',
		url: 'https://mcpvibeui.com',
		author: { '@type': 'Person', name: 'Scott Spence' },
		offers: { '@type': 'Offer', price: '0', priceCurrency: 'USD' },
	};
</script>

<Head {seo_config} />
<SchemaOrg schema={schema_org} />

<div
	class="min-h-screen"
	style="background-color: var(--color-background); color: var(--color-foreground); font-family: var(--font-body);"
>
	<!-- Nav -->
	<nav
		class="fixed top-0 right-0 left-0 z-50 backdrop-blur-md"
		style="background-color: oklch(99% 0.01 240 / 0.8); border-bottom: 1px solid var(--color-border);"
	>
		<div
			class="mx-auto flex max-w-7xl items-center justify-between px-6 py-4"
		>
			<a
				href="/"
				class="text-sm font-semibold tracking-tight"
				style="font-family: var(--font-mono);"
			>
				mcp-vibe-ui
			</a>
			<div class="flex items-center gap-6">
				<a
					href="#themes"
					class="text-sm transition hover:opacity-70"
					style="color: var(--color-muted-foreground);">Themes</a
				>
				<a
					href="https://github.com/spences10/mcp-vibe-ui"
					target="_blank"
					rel="noopener"
					class="text-sm transition hover:opacity-70"
					style="color: var(--color-muted-foreground);">GitHub</a
				>
				<a
					href="https://www.npmjs.com/package/mcp-vibe-ui"
					target="_blank"
					rel="noopener"
					class="px-4 py-2 text-sm font-medium transition hover:opacity-90"
					style="background-color: var(--color-foreground); color: var(--color-background); border-radius: var(--radius-sm);"
				>
					npm
				</a>
			</div>
		</div>
	</nav>

	<!-- Hero -->
	<section class="relative px-6 pt-32 pb-20">
		<div class="mx-auto max-w-7xl">
			<div class="grid gap-12 lg:grid-cols-2 lg:gap-16">
				<!-- Left: Text -->
				<div class="flex flex-col justify-center">
					<p
						class="mb-4 text-sm font-medium tracking-widest uppercase"
						style="color: var(--color-primary);"
					>
						MCP Server for Design Systems
					</p>
					<h1
						class="mb-6 text-5xl leading-[1.1] tracking-tight md:text-6xl lg:text-7xl"
						style="font-family: var(--font-display); font-weight: 600;"
					>
						One prompt.<br />
						<span style="color: var(--color-primary);">
							15 themes.
						</span>
					</h1>
					<p
						class="mb-8 max-w-lg text-lg leading-relaxed"
						style="color: var(--color-muted-foreground);"
					>
						Give your LLM access to complete design systems. Tailwind
						v4 tokens, component patterns, typography, and effects —
						all from a single tool call.
					</p>

					<div class="flex flex-wrap gap-3">
						<a
							href="#themes"
							class="px-6 py-3 text-sm font-semibold transition hover:opacity-90"
							style="background-color: var(--color-foreground); color: var(--color-background); border-radius: var(--radius-sm);"
						>
							View all themes
						</a>
						<a
							href="https://github.com/spences10/mcp-vibe-ui#readme"
							target="_blank"
							rel="noopener"
							class="px-6 py-3 text-sm font-semibold transition hover:opacity-80"
							style="border: 1px solid var(--color-border); border-radius: var(--radius-sm);"
						>
							Documentation
						</a>
					</div>
				</div>

				<!-- Right: Live Preview -->
				<div class="relative">
					<div
						class="relative overflow-hidden"
						style="border-radius: var(--radius-lg); border: 1px solid var(--color-border); box-shadow: 0 25px 50px -12px rgba(0,0,0,0.15);"
					>
						<!-- Browser chrome -->
						<div
							class="flex items-center gap-2 px-4 py-3"
							style="background-color: var(--color-muted); border-bottom: 1px solid var(--color-border);"
						>
							<div class="flex gap-1.5">
								<div
									class="h-3 w-3 rounded-full"
									style="background-color: oklch(65% 0.2 25);"
								></div>
								<div
									class="h-3 w-3 rounded-full"
									style="background-color: oklch(80% 0.15 85);"
								></div>
								<div
									class="h-3 w-3 rounded-full"
									style="background-color: oklch(75% 0.15 145);"
								></div>
							</div>
							<div
								class="ml-4 flex-1 rounded px-3 py-1 text-xs"
								style="background-color: var(--color-background); color: var(--color-muted-foreground); font-family: var(--font-mono);"
							>
								localhost:5173
							</div>
						</div>

						<!-- Theme preview -->
						<button
							type="button"
							class="relative block aspect-video w-full cursor-pointer"
							onmouseenter={() => (is_paused = true)}
							onmouseleave={() => (is_paused = false)}
							onclick={() =>
								(current_index = (current_index + 1) % themes.length)}
						>
							{#key current_index}
								<img
									src={themes[current_index].img}
									alt="{themes[current_index].name} theme"
									class="absolute inset-0 h-full w-full object-cover object-top"
									in:fade={{ duration: 400 }}
								/>
							{/key}
						</button>

						<!-- Theme name overlay -->
						<div
							class="absolute right-4 bottom-4 left-4 flex items-center justify-between rounded px-4 py-2 backdrop-blur-md"
							style="background-color: oklch(0% 0 0 / 0.7);"
						>
							{#key current_index}
								<span
									class="text-sm font-medium"
									style="color: white; font-family: var(--font-mono);"
									in:fly={{ y: 10, duration: 300 }}
								>
									{themes[current_index].slug}
								</span>
							{/key}
							<span
								class="text-xs tabular-nums"
								style="color: oklch(100% 0 0 / 0.5);"
							>
								{current_index + 1}/{themes.length}
							</span>
						</div>
					</div>

					<!-- Prompt badge -->
					<div
						class="mt-4 rounded p-4"
						style="background-color: var(--color-muted); border: 1px solid var(--color-border); border-radius: var(--radius-lg);"
					>
						<p
							class="text-xs tracking-wider uppercase"
							style="color: var(--color-muted-foreground); margin-bottom: 0.5rem;"
						>
							Prompt used
						</p>
						<p
							class="text-sm"
							style="font-family: var(--font-mono); color: var(--color-foreground);"
						>
							create a <span style="color: var(--color-primary);"
								>{themes[current_index].slug}</span
							> landing page for a cat dating app
						</p>
					</div>

					<p
						class="mt-6 text-base leading-relaxed"
						style="color: var(--color-muted-foreground);"
					>
						Every theme on this site was generated with that <span
							style="color: var(--color-primary);">exact prompt</span
						>. One-shot. No follow-ups. Each was a fresh Claude Code
						session — the only thing that changed was the theme name.
					</p>
				</div>
			</div>
		</div>
	</section>

	<!-- How it works -->
	<section
		class="px-6 py-20"
		style="background-color: var(--color-muted);"
	>
		<div class="mx-auto max-w-7xl">
			<h2
				class="mb-12 text-center text-3xl tracking-tight md:text-4xl"
				style="font-family: var(--font-display); font-weight: 600;"
			>
				How it works
			</h2>
			<div class="grid gap-8 md:grid-cols-3">
				<div class="text-center">
					<div
						class="mx-auto mb-4 flex h-12 w-12 items-center justify-center rounded-full text-lg font-semibold"
						style="background-color: var(--color-foreground); color: var(--color-background);"
					>
						1
					</div>
					<h3
						class="mb-2 text-lg font-semibold"
						style="font-family: var(--font-display);"
					>
						Add to MCP config
					</h3>
					<p
						class="text-sm leading-relaxed"
						style="color: var(--color-muted-foreground);"
					>
						One line in your Claude Desktop or agent config. No
						dependencies to install.
					</p>
				</div>
				<div class="text-center">
					<div
						class="mx-auto mb-4 flex h-12 w-12 items-center justify-center rounded-full text-lg font-semibold"
						style="background-color: var(--color-foreground); color: var(--color-background);"
					>
						2
					</div>
					<h3
						class="mb-2 text-lg font-semibold"
						style="font-family: var(--font-display);"
					>
						Ask for a theme
					</h3>
					<p
						class="text-sm leading-relaxed"
						style="color: var(--color-muted-foreground);"
					>
						The LLM calls theme_search with a name or description.
						Gets back complete design tokens.
					</p>
				</div>
				<div class="text-center">
					<div
						class="mx-auto mb-4 flex h-12 w-12 items-center justify-center rounded-full text-lg font-semibold"
						style="background-color: var(--color-foreground); color: var(--color-background);"
					>
						3
					</div>
					<h3
						class="mb-2 text-lg font-semibold"
						style="font-family: var(--font-display);"
					>
						Generate styled UI
					</h3>
					<p
						class="text-sm leading-relaxed"
						style="color: var(--color-muted-foreground);"
					>
						LLM uses the tokens to generate consistent, beautiful
						interfaces every time.
					</p>
				</div>
			</div>

			<!-- Config example -->
			<div
				class="mx-auto mt-12 max-w-2xl overflow-hidden"
				style="border: 1px solid var(--color-border); border-radius: var(--radius-lg); background-color: var(--color-background);"
			>
				<div
					class="px-4 py-2"
					style="border-bottom: 1px solid var(--color-border);"
				>
					<span
						class="text-xs"
						style="font-family: var(--font-mono); color: var(--color-muted-foreground);"
						>claude_desktop_config.json</span
					>
				</div>
				<pre
					class="overflow-x-auto p-4 text-sm"
					style="font-family: var(--font-mono);"><code
						>{`{
  "mcpServers": {
    "mcp-vibe-ui": {
      "command": "npx",
      "args": ["-y", "mcp-vibe-ui"]
    }
  }
}`}</code
					></pre>
			</div>
		</div>
	</section>

	<!-- Theme Gallery -->
	<section id="themes" class="px-6 py-20">
		<div class="mx-auto max-w-7xl">
			<div class="mb-12 text-center">
				<h2
					class="mb-4 text-3xl tracking-tight md:text-4xl"
					style="font-family: var(--font-display); font-weight: 600;"
				>
					15 distinct themes
				</h2>
				<p
					class="mx-auto max-w-2xl leading-relaxed"
					style="color: var(--color-muted-foreground);"
				>
					Each generated with the same prompt. Click any theme to see
					the full page.
				</p>
			</div>

			<!-- Theme grid -->
			<div class="grid gap-4 sm:grid-cols-2 lg:grid-cols-3">
				{#each themes as theme, i}
					<a
						href="/{theme.slug}"
						class="group relative overflow-hidden transition hover:opacity-95"
						style="border-radius: var(--radius-lg); border: 1px solid var(--color-border);"
					>
						<div class="aspect-video">
							<img
								src={theme.img}
								alt="{theme.name} theme"
								loading="lazy"
								class="h-full w-full object-cover object-top transition-transform duration-500 group-hover:scale-105"
							/>
						</div>
						<div
							class="absolute inset-x-0 bottom-0 p-4"
							style="background: linear-gradient(transparent, oklch(0% 0 0 / 0.8));"
						>
							<span
								class="text-sm font-medium"
								style="color: white; font-family: var(--font-mono);"
								>{theme.slug}</span
							>
						</div>
					</a>
				{/each}
			</div>
		</div>
	</section>

	<!-- What you get -->
	<section
		class="px-6 py-20"
		style="background-color: var(--color-muted);"
	>
		<div class="mx-auto max-w-7xl">
			<h2
				class="mb-12 text-center text-3xl tracking-tight md:text-4xl"
				style="font-family: var(--font-display); font-weight: 600;"
			>
				What each theme includes
			</h2>
			<div class="grid gap-6 md:grid-cols-2 lg:grid-cols-4">
				<div
					class="rounded p-6"
					style="background-color: var(--color-background); border: 1px solid var(--color-border); border-radius: var(--radius-lg);"
				>
					<div class="mb-3 text-2xl">🎨</div>
					<h3
						class="mb-2 font-semibold"
						style="font-family: var(--font-display);"
					>
						Color Tokens
					</h3>
					<p
						class="text-sm"
						style="color: var(--color-muted-foreground);"
					>
						OKLCH colors for background, foreground, primary,
						secondary, accent, muted, and more.
					</p>
				</div>
				<div
					class="rounded p-6"
					style="background-color: var(--color-background); border: 1px solid var(--color-border); border-radius: var(--radius-lg);"
				>
					<div class="mb-3 text-2xl">✏️</div>
					<h3
						class="mb-2 font-semibold"
						style="font-family: var(--font-display);"
					>
						Typography
					</h3>
					<p
						class="text-sm"
						style="color: var(--color-muted-foreground);"
					>
						Font stacks for display, body, and mono. Google Fonts
						links included.
					</p>
				</div>
				<div
					class="rounded p-6"
					style="background-color: var(--color-background); border: 1px solid var(--color-border); border-radius: var(--radius-lg);"
				>
					<div class="mb-3 text-2xl">🧩</div>
					<h3
						class="mb-2 font-semibold"
						style="font-family: var(--font-display);"
					>
						Component Patterns
					</h3>
					<p
						class="text-sm"
						style="color: var(--color-muted-foreground);"
					>
						Tailwind classes for buttons, cards, inputs, navigation,
						and layouts.
					</p>
				</div>
				<div
					class="rounded p-6"
					style="background-color: var(--color-background); border: 1px solid var(--color-border); border-radius: var(--radius-lg);"
				>
					<div class="mb-3 text-2xl">✨</div>
					<h3
						class="mb-2 font-semibold"
						style="font-family: var(--font-display);"
					>
						Effects & Utilities
					</h3>
					<p
						class="text-sm"
						style="color: var(--color-muted-foreground);"
					>
						Shadows, gradients, animations, and theme-specific CSS
						utilities.
					</p>
				</div>
			</div>
		</div>
	</section>

	<!-- Footer -->
	<footer
		class="px-6 py-12"
		style="border-top: 1px solid var(--color-border);"
	>
		<div
			class="mx-auto flex max-w-7xl flex-col items-center justify-between gap-4 md:flex-row"
		>
			<p
				class="text-sm"
				style="color: var(--color-muted-foreground); font-family: var(--font-mono);"
			>
				Built by <a
					href="https://scottspence.com"
					target="_blank"
					rel="noopener"
					class="underline underline-offset-4 transition hover:opacity-70"
					style="color: var(--color-foreground);">Scott Spence</a
				>
			</p>
			<div class="flex gap-6">
				<a
					href="https://github.com/spences10/mcp-vibe-ui"
					target="_blank"
					rel="noopener"
					class="text-sm underline-offset-4 transition hover:underline hover:opacity-70"
					style="color: var(--color-muted-foreground);">GitHub</a
				>
				<a
					href="https://www.npmjs.com/package/mcp-vibe-ui"
					target="_blank"
					rel="noopener"
					class="text-sm underline-offset-4 transition hover:underline hover:opacity-70"
					style="color: var(--color-muted-foreground);">npm</a
				>
			</div>
		</div>
	</footer>
</div>
