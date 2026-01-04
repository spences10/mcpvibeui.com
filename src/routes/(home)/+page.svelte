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
			'MCP server providing design tokens for LLM-powered UI generation with 15 production-ready themes',
		url: 'https://mcpvibeui.com',
		author: { '@type': 'Person', name: 'Scott Spence' },
		offers: { '@type': 'Offer', price: '0', priceCurrency: 'USD' },
	};

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
</script>

<Head {seo_config} />
<SchemaOrg schema={schema_org} />

<div
	class="min-h-screen"
	style="background-color: var(--color-background); color: var(--color-foreground); font-family: var(--font-body);"
>
	<!-- Header -->
	<header
		class="mx-auto flex max-w-5xl items-center justify-between px-6 py-6"
		style="border-bottom: 1px solid var(--color-border);"
	>
		<span
			class="text-xs font-semibold tracking-widest uppercase"
			style="color: var(--color-muted-foreground);">MCP Server</span
		>
		<nav class="flex gap-6 text-sm">
			<a
				href="https://github.com/spences10/mcp-vibe-ui"
				target="_blank"
				rel="noopener"
				class="underline-offset-4 hover:underline"
				style="color: var(--color-muted-foreground);">GitHub</a
			>
			<a
				href="https://www.npmjs.com/package/mcp-vibe-ui"
				target="_blank"
				rel="noopener"
				class="underline-offset-4 hover:underline"
				style="color: var(--color-muted-foreground);">npm</a
			>
		</nav>
	</header>

	<!-- Hero -->
	<section class="mx-auto max-w-4xl px-6 py-20">
		<h1
			class="mb-8 text-5xl leading-tight tracking-tight md:text-6xl"
			style="font-family: var(--font-display); font-weight: 600;"
		>
			Same prompt.<br />15 themes.
		</h1>
		<p
			class="mb-8 max-w-2xl text-xl leading-relaxed"
			style="color: var(--color-muted-foreground);"
		>
			Every page in the gallery below was generated with this prompt:
		</p>

		<div
			class="mb-10 p-6"
			style="background-color: var(--color-muted); border-radius: var(--radius-lg); font-family: var(--font-mono);"
		>
			<p class="text-lg">
				create a <span style="color: var(--color-primary);"
					>{'{theme}'}</span
				> landing page for cat dating app use mcp-vibe-ui
			</p>
		</div>

		<p
			class="mb-10 max-w-2xl leading-relaxed"
			style="color: var(--color-muted-foreground);"
		>
			mcp-vibe-ui is an MCP server. When an LLM calls <code
				style="font-family: var(--font-mono);">theme_search</code
			>, it gets back Tailwind v4 CSS tokens, component patterns, and
			font specs for that theme. The LLM uses these to generate
			consistently styled UI.
		</p>

		<div class="flex flex-wrap items-center gap-4">
			<a
				href="#themes"
				class="px-6 py-3 text-sm font-semibold transition hover:opacity-90"
				style="background-color: var(--color-primary); color: var(--color-primary-foreground); border-radius: var(--radius-sm);"
			>
				See the results
			</a>
			<a
				href="https://github.com/spences10/mcp-vibe-ui"
				target="_blank"
				rel="noopener"
				class="px-6 py-3 text-sm font-semibold transition hover:opacity-80"
				style="border: 1px solid var(--color-border); border-radius: var(--radius-sm);"
			>
				GitHub
			</a>
		</div>

		<!-- Install -->
		<div class="mt-12">
			<p
				class="mb-3 text-xs font-semibold tracking-widest uppercase"
				style="color: var(--color-muted-foreground);"
			>
				Add to your MCP config
			</p>
			<div
				class="overflow-hidden"
				style="border: 1px solid var(--color-border); border-radius: var(--radius-lg);"
			>
				<div
					class="px-4 py-2"
					style="border-bottom: 1px solid var(--color-border); background-color: var(--color-muted);"
				>
					<span
						class="text-xs"
						style="font-family: var(--font-mono); color: var(--color-muted-foreground);"
						>claude_desktop_config.json</span
					>
				</div>
				<pre
					class="p-4 text-sm"
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
	<section
		id="themes"
		class="mx-auto max-w-6xl px-6 py-16"
		style="border-top: 1px solid var(--color-border);"
	>
		<div class="mb-12 max-w-2xl">
			<h2
				class="mb-4 text-3xl tracking-tight"
				style="font-family: var(--font-display); font-weight: 600;"
			>
				The results
			</h2>
			<p
				class="leading-relaxed"
				style="color: var(--color-muted-foreground);"
			>
				Each page was generated with the same prompt. The only
				difference is the theme name. Click any to see the full page.
			</p>
		</div>

		<div class="grid gap-4 sm:grid-cols-2 lg:grid-cols-3">
			{#each themes as theme}
				<a
					href="/{theme.slug}"
					class="group overflow-hidden transition hover:opacity-95"
					style="border: 1px solid var(--color-border); border-radius: var(--radius-lg);"
				>
					<div class="aspect-video overflow-hidden">
						<img
							src={theme.img}
							alt="{theme.name} theme preview"
							loading="lazy"
							class="h-full w-full object-cover object-top transition-transform duration-500 group-hover:scale-105"
						/>
					</div>
					<div class="p-4">
						<p class="text-sm font-semibold">{theme.name}</p>
					</div>
				</a>
			{/each}
		</div>
	</section>

	<!-- Footer -->
	<footer
		class="mx-auto max-w-5xl px-6 py-8"
		style="border-top: 1px solid var(--color-border);"
	>
		<p
			class="text-center text-xs tracking-wide"
			style="color: var(--color-muted-foreground); font-family: var(--font-mono);"
		>
			<a
				href="https://scottspence.com"
				target="_blank"
				rel="noopener"
				class="underline-offset-4 hover:underline"
				style="color: var(--color-foreground);">Scott Spence</a
			>
			<span class="mx-2">·</span>
			<a
				href="https://github.com/spences10/mcp-vibe-ui"
				target="_blank"
				rel="noopener"
				class="underline-offset-4 hover:underline">GitHub</a
			>
			<span class="mx-2">·</span>
			<a
				href="https://www.npmjs.com/package/mcp-vibe-ui"
				target="_blank"
				rel="noopener"
				class="underline-offset-4 hover:underline">npm</a
			>
		</p>
	</footer>
</div>
