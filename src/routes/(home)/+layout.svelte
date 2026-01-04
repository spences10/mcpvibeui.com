<script lang="ts">
	import '@fontsource/playfair-display/400.css';
	import '@fontsource/playfair-display/600.css';
	import '@fontsource/playfair-display/700.css';
	import '@fontsource/source-sans-pro/300.css';
	import '@fontsource/source-sans-pro/400.css';
	import '@fontsource/source-sans-pro/600.css';
	import '@fontsource/victor-mono/400.css';
	import '@fontsource/victor-mono/500.css';

	let { children } = $props();
</script>

<div class="home-theme">
	{@render children()}
</div>

<style>
	.home-theme {
		--color-background: oklch(99% 0.01 240);
		--color-foreground: oklch(20% 0.03 240);
		--color-muted: oklch(96% 0.02 240);
		--color-muted-foreground: oklch(32% 0.02 240);
		--color-border: oklch(93% 0.02 240);
		--color-primary: oklch(45% 0.05 250);
		--color-primary-foreground: oklch(96% 0.01 250);
		--color-secondary: oklch(55% 0.07 30);
		--color-secondary-foreground: oklch(98% 0.01 30);
		--color-accent: oklch(68% 0.09 120);
		--color-accent-foreground: oklch(14% 0.02 120);
		--font-display:
			'Playfair Display', Georgia, 'Times New Roman', serif;
		--font-body:
			'Source Sans Pro', 'Helvetica Neue', Arial, sans-serif;
		--font-mono:
			'Victor Mono', 'SF Mono', Monaco, Consolas, monospace;
		--radius-sm: 0.25rem;
		--radius-md: 0.25rem;
		--radius-lg: 0.5rem;
	}
</style>
