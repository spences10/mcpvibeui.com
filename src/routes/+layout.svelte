<script lang="ts">
	import { page } from '$app/state';
	import favicon from '$lib/assets/favicon.svg';
	import '@fontsource/inter/400.css';
	import '@fontsource/inter/500.css';
	import '@fontsource/inter/600.css';
	import '@fontsource/inter/700.css';
	import '@fontsource/jetbrains-mono/400.css';
	import '@fontsource/jetbrains-mono/500.css';
	import { fly } from 'svelte/transition';
	import './layout.css';

	let { children } = $props();

	let show_back = $state(false);
	let is_theme_page = $derived(page.url.pathname !== '/');
	let theme_name = $derived(page.url.pathname.slice(1));

	$effect(() => {
		if (is_theme_page) {
			const timeout = setTimeout(() => {
				show_back = true;
			}, 1500);
			return () => clearTimeout(timeout);
		} else {
			show_back = false;
		}
	});
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>
{@render children()}

{#if is_theme_page && show_back}
	<div
		class="fixed right-6 bottom-6 z-50 flex max-w-sm flex-col gap-3 rounded-lg p-4 shadow-2xl"
		style="background-color: #18181b; color: #fafafa; font-family: 'Inter', sans-serif; border: 1px solid #3f3f46;"
		transition:fly={{ y: 20, duration: 300 }}
	>
		<p class="text-base leading-relaxed" style="color: #a1a1aa;">
			This is the <strong style="color: #fafafa;">{theme_name}</strong
			>
			theme, generated with the prompt
			<span
				style="color: #a855f7; font-family: 'Victor Mono', monospace; font-size: 14px;"
				>"create a {theme_name} landing page for a cat dating app"</span
			>. It's an example page and is not functional.
		</p>
		<a
			href="/"
			class="flex items-center justify-center gap-2 rounded px-4 py-2 text-sm font-medium transition hover:opacity-90"
			style="background-color: #a855f7; color: #18181b;"
		>
			<svg
				xmlns="http://www.w3.org/2000/svg"
				width="16"
				height="16"
				viewBox="0 0 24 24"
				fill="none"
				stroke="currentColor"
				stroke-width="2"
				stroke-linecap="round"
				stroke-linejoin="round"
			>
				<path d="m12 19-7-7 7-7" />
				<path d="M19 12H5" />
			</svg>
			Back to all themes
		</a>
	</div>
{/if}
