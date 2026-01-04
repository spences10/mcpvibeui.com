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

	let current_index = $state(
		Math.floor(Math.random() * themes.length),
	);
	let is_transitioning = $state(false);

	// Generate theme class name
	const get_theme_class = (slug: string) => `theme-${slug}`;

	// Switch theme with opacity fade for smoother font transitions
	const switch_theme = () => {
		if (is_transitioning) return;
		is_transitioning = true;
		// Wait for fade out, then switch theme
		setTimeout(() => {
			current_index = (current_index + 1) % themes.length;
			// Wait a frame for theme to apply, then fade back in
			requestAnimationFrame(() => {
				setTimeout(() => {
					is_transitioning = false;
				}, 50);
			});
		}, 300);
	};

	const seo_config: SeoConfig = {
		title:
			'mcp-vibe-ui — Design Tokens for AI-Generated UI | MCP Server',
		description:
			'Stop getting ugly AI-generated interfaces. mcp-vibe-ui is an MCP server that gives Claude, ChatGPT, and other LLMs access to complete design systems with Tailwind v4 CSS.',
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
	class="min-h-screen {get_theme_class(
		themes[current_index].slug,
	)} transition-opacity duration-300 ease-in-out"
	class:opacity-0={is_transitioning}
	style="background-color: var(--color-background); color: var(--color-foreground); font-family: var(--font-body);"
>
	<!-- Nav -->
	<nav
		class="fixed top-0 right-0 left-0 z-50 backdrop-blur-md transition-colors duration-500"
		style="background-color: color-mix(in oklch, var(--color-background) 80%, transparent); border-bottom: 1px solid var(--color-border);"
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
					class="btn-primary px-4 py-2 text-sm font-medium transition-all"
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
						MCP Server
					</p>
					<h1
						class="mb-6 text-4xl leading-[1.1] tracking-tight md:text-5xl lg:text-6xl"
						style="font-family: var(--font-display); font-weight: 600;"
					>
						AI-generated UI that doesn't look like trash
					</h1>
					<p
						class="mb-8 max-w-lg text-lg leading-relaxed"
						style="color: var(--color-muted-foreground);"
					>
						<strong style="color: var(--color-foreground);"
							>mcp-vibe-ui</strong
						>
						is an
						<a
							href="https://modelcontextprotocol.io"
							target="_blank"
							rel="noopener"
							class="underline underline-offset-2"
							style="color: var(--color-foreground);">MCP server</a
						>
						that gives LLMs access to complete design systems. When Claude
						or Cursor generates UI, it pulls real Tailwind v4 tokens, component
						patterns, and effects instead of guessing.
					</p>

					<!-- Quick install -->
					<div
						class="mb-6 overflow-hidden"
						style="border: var(--theme-border-width, 1px) solid var(--color-border); border-radius: var(--radius-md); background-color: var(--color-muted); box-shadow: var(--theme-shadow);"
					>
						<div
							class="px-3 py-1.5 text-xs"
							style="border-bottom: var(--theme-border-width, 1px) solid var(--color-border); color: var(--color-muted-foreground);"
						>
							Add to Claude Desktop / Cursor
						</div>
						<pre
							class="overflow-x-auto p-3 text-sm"
							style="font-family: var(--font-mono);"><code
								>{`"mcp-vibe-ui": { "command": "npx", "args": ["-y", "mcp-vibe-ui"] }`}</code
							></pre>
					</div>

					<div class="flex flex-wrap gap-3">
						<a
							href="#how-it-works"
							class="btn-primary px-6 py-3 text-sm font-semibold transition-all"
						>
							See how it works
						</a>
						<a
							href="https://github.com/spences10/mcp-vibe-ui"
							target="_blank"
							rel="noopener"
							class="btn-secondary px-6 py-3 text-sm font-semibold transition-all"
						>
							GitHub
						</a>
					</div>
				</div>

				<!-- Right: Live Preview -->
				<div class="relative">
					<!-- Proof label -->
					<div
						class="mb-3 text-center text-sm font-medium"
						style="color: var(--color-muted-foreground);"
					>
						Every page below was AI-generated. Same prompt. Different
						theme.
					</div>

					<div
						class="relative overflow-hidden"
						style="border-radius: var(--radius-lg); border: var(--theme-border-width, 1px) solid var(--color-border); box-shadow: var(--theme-shadow, 0 25px 50px -12px rgba(0,0,0,0.15));"
					>
						<!-- Browser chrome -->
						<div
							class="flex items-center gap-2 px-4 py-3"
							style="background-color: var(--color-muted); border-bottom: var(--theme-border-width, 1px) solid var(--color-border);"
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
								class="ml-4 flex-1 px-3 py-1 text-xs"
								style="background-color: var(--color-background); color: var(--color-muted-foreground); font-family: var(--font-mono); border-radius: var(--radius-sm);"
							>
								localhost:5173
							</div>
						</div>

						<!-- Theme preview -->
						<button
							type="button"
							class="relative block aspect-video w-full cursor-pointer"
							onclick={switch_theme}
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
							class="absolute right-4 bottom-4 left-4 flex items-center justify-between px-4 py-2 backdrop-blur-md"
							style="background-color: oklch(0% 0 0 / 0.7); border-radius: var(--radius-sm);"
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
						class="mt-4 p-4"
						style="background-color: var(--color-muted); border: var(--theme-border-width, 1px) solid var(--color-border); border-radius: var(--radius-lg);"
					>
						<div class="flex items-center justify-between">
							<p
								class="text-xs tracking-wider uppercase"
								style="color: var(--color-muted-foreground);"
							>
								The exact prompt used
							</p>
							<span
								class="px-2 py-0.5 text-xs"
								style="background-color: var(--color-primary); color: var(--color-primary-foreground); border-radius: var(--radius-sm);"
								>one-shot</span
							>
						</div>
						<p
							class="mt-2 text-sm"
							style="font-family: var(--font-mono); color: var(--color-foreground);"
						>
							create a <span style="color: var(--color-primary);"
								>{themes[current_index].slug}</span
							> landing page for a cat dating app
						</p>
					</div>
				</div>
			</div>
		</div>
	</section>

	<!-- Proof section -->
	<section class="px-6 py-16">
		<div class="mx-auto max-w-3xl text-center">
			<p
				class="text-xl leading-relaxed md:text-2xl"
				style="color: var(--color-foreground);"
			>
				Every theme on this site was generated with the
				<strong style="color: var(--color-primary);"
					>exact same prompt</strong
				>. One-shot. No follow-ups. Each was a fresh Claude Code
				session — the only thing that changed was the theme name.
			</p>
		</div>
	</section>

	<!-- Theme Gallery -->
	<section id="themes" class="px-6 pb-20">
		<div class="mx-auto max-w-7xl">
			<div class="mb-12 text-center">
				<h2
					class="mb-4 text-3xl tracking-tight md:text-4xl"
					style="font-family: var(--font-display); font-weight: 600;"
				>
					15 themes, zero follow-up prompts
				</h2>
				<p
					class="mx-auto max-w-2xl leading-relaxed"
					style="color: var(--color-muted-foreground);"
				>
					Each page below was generated in a fresh Claude Code session
					with the same prompt. Click to see the full result.
				</p>
			</div>

			<!-- Theme grid -->
			<div class="grid gap-4 sm:grid-cols-2 lg:grid-cols-3">
				{#each themes as theme, i}
					<a
						href="/{theme.slug}"
						class="group relative overflow-hidden transition hover:opacity-95"
						style="border-radius: var(--radius-lg); border: var(--theme-border-width, 1px) solid var(--color-border); box-shadow: var(--theme-shadow);"
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

	<!-- How it works -->
	<section
		id="how-it-works"
		class="px-6 py-20"
		style="background-color: var(--color-muted);"
	>
		<div class="mx-auto max-w-7xl">
			<div class="mb-12 text-center">
				<h2
					class="mb-4 text-3xl tracking-tight md:text-4xl"
					style="font-family: var(--font-display); font-weight: 600;"
				>
					How it works
				</h2>
				<p
					class="mx-auto max-w-2xl"
					style="color: var(--color-muted-foreground);"
				>
					MCP (Model Context Protocol) lets LLMs call external tools.
					When you ask for themed UI, the LLM calls
					<code
						style="font-family: var(--font-mono); background-color: var(--color-background); padding: 0.125rem 0.375rem; border-radius: 0.25rem;"
						>theme_search</code
					> and gets back everything it needs.
				</p>
			</div>

			<!-- Two column: steps + code -->
			<div class="grid gap-8 lg:grid-cols-2">
				<!-- Steps -->
				<div class="space-y-6">
					<div
						class="flex gap-4 p-4"
						style="background-color: var(--color-background); border: var(--theme-border-width, 1px) solid var(--color-border); border-radius: var(--radius-lg); box-shadow: var(--theme-shadow);"
					>
						<div
							class="flex h-8 w-8 shrink-0 items-center justify-center text-sm font-semibold"
							style="background-color: var(--color-foreground); color: var(--color-background); border-radius: var(--radius-sm);"
						>
							1
						</div>
						<div>
							<h3
								class="mb-1 font-semibold"
								style="font-family: var(--font-display);"
							>
								You prompt for themed UI
							</h3>
							<p
								class="text-sm"
								style="color: var(--color-muted-foreground);"
							>
								"Create a cyberpunk login form" or "build me a
								glassmorphic dashboard"
							</p>
						</div>
					</div>

					<div
						class="flex gap-4 p-4"
						style="background-color: var(--color-background); border: var(--theme-border-width, 1px) solid var(--color-border); border-radius: var(--radius-lg); box-shadow: var(--theme-shadow);"
					>
						<div
							class="flex h-8 w-8 shrink-0 items-center justify-center text-sm font-semibold"
							style="background-color: var(--color-foreground); color: var(--color-background); border-radius: var(--radius-sm);"
						>
							2
						</div>
						<div>
							<h3
								class="mb-1 font-semibold"
								style="font-family: var(--font-display);"
							>
								LLM calls theme_search
							</h3>
							<p
								class="text-sm"
								style="color: var(--color-muted-foreground);"
							>
								Matches by name ("cyberpunk") or intent ("dark
								futuristic neon"). Returns the full design system.
							</p>
						</div>
					</div>

					<div
						class="flex gap-4 p-4"
						style="background-color: var(--color-background); border: var(--theme-border-width, 1px) solid var(--color-border); border-radius: var(--radius-lg); box-shadow: var(--theme-shadow);"
					>
						<div
							class="flex h-8 w-8 shrink-0 items-center justify-center text-sm font-semibold"
							style="background-color: var(--color-foreground); color: var(--color-background); border-radius: var(--radius-sm);"
						>
							3
						</div>
						<div>
							<h3
								class="mb-1 font-semibold"
								style="font-family: var(--font-display);"
							>
								LLM generates with real tokens
							</h3>
							<p
								class="text-sm"
								style="color: var(--color-muted-foreground);"
							>
								Uses the CSS variables, patterns, and effects. No more
								guessing colors or inventing class names.
							</p>
						</div>
					</div>
				</div>

				<!-- Code example -->
				<div
					class="overflow-hidden"
					style="border: var(--theme-border-width, 1px) solid var(--color-border); border-radius: var(--radius-lg); background-color: var(--color-background); box-shadow: var(--theme-shadow);"
				>
					<div
						class="px-4 py-2"
						style="border-bottom: var(--theme-border-width, 1px) solid var(--color-border);"
					>
						<span
							class="text-xs"
							style="font-family: var(--font-mono); color: var(--color-muted-foreground);"
							>theme_search("cyberpunk") returns:</span
						>
					</div>
					<pre
						class="overflow-x-auto p-4 text-xs leading-relaxed"
						style="font-family: var(--font-mono);"><code
							>{`{
  "id": "cyberpunk",
  "css": "@theme {
    --color-background: oklch(12% 0.03 300);
    --color-primary: oklch(65% 0.28 330);
    --font-display: 'Orbitron', monospace;
    ...
  }",
  "patterns": {
    "surface": "bg-background text-foreground",
    "card": "bg-muted rounded-lg border",
    "glow": "shadow-[0_0_20px_var(--color-primary)]"
  },
  "fonts": [
    { "package": "@fontsource/orbitron", ... }
  ],
  "extended": {
    "effects": { "neonGlow": "..." },
    "animations": { "pulse": "..." }
  }
}`}</code
						></pre>
				</div>
			</div>

			<!-- Installation -->
			<div class="mt-12">
				<h3
					class="mb-4 text-center text-lg font-semibold"
					style="font-family: var(--font-display);"
				>
					Installation
				</h3>
				<div
					class="mx-auto max-w-2xl overflow-hidden"
					style="border: var(--theme-border-width, 1px) solid var(--color-border); border-radius: var(--radius-lg); background-color: var(--color-background); box-shadow: var(--theme-shadow);"
				>
					<div
						class="px-4 py-2"
						style="border-bottom: var(--theme-border-width, 1px) solid var(--color-border);"
					>
						<span
							class="text-xs"
							style="font-family: var(--font-mono); color: var(--color-muted-foreground);"
							>claude_desktop_config.json / .cursor/mcp.json</span
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
				<p
					class="mt-3 text-center text-sm"
					style="color: var(--color-muted-foreground);"
				>
					That's it. No npm install. npx downloads and runs it on
					demand.
				</p>
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
					class="p-6"
					style="background-color: var(--color-background); border: var(--theme-border-width, 1px) solid var(--color-border); border-radius: var(--radius-lg); box-shadow: var(--theme-shadow);"
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
					class="p-6"
					style="background-color: var(--color-background); border: var(--theme-border-width, 1px) solid var(--color-border); border-radius: var(--radius-lg); box-shadow: var(--theme-shadow);"
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
					class="p-6"
					style="background-color: var(--color-background); border: var(--theme-border-width, 1px) solid var(--color-border); border-radius: var(--radius-lg); box-shadow: var(--theme-shadow);"
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
					class="p-6"
					style="background-color: var(--color-background); border: var(--theme-border-width, 1px) solid var(--color-border); border-radius: var(--radius-lg); box-shadow: var(--theme-shadow);"
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
		style="border-top: var(--theme-border-width, 1px) solid var(--color-border);"
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
