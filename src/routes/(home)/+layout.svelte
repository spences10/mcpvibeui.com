<script lang="ts">
	// Theme CSS
	import '$lib/themes/all-themes.css';

	// === SHARED FONTS (used by multiple themes) ===
	// Inter - glassmorphic, neumorphic, monochrome, typographic
	import '@fontsource/inter/300.css';
	import '@fontsource/inter/400.css';
	import '@fontsource/inter/500.css';
	import '@fontsource/inter/600.css';
	import '@fontsource/inter/700.css';
	// Fira Code - glassmorphic, wireframe
	import '@fontsource/fira-code/300.css';
	import '@fontsource/fira-code/400.css';
	import '@fontsource/fira-code/500.css';
	import '@fontsource/fira-code/600.css';
	import '@fontsource/fira-code/700.css';
	// JetBrains Mono - claymorphic, industrial, typographic
	import '@fontsource/jetbrains-mono/300.css';
	import '@fontsource/jetbrains-mono/400.css';
	import '@fontsource/jetbrains-mono/500.css';
	import '@fontsource/jetbrains-mono/600.css';
	import '@fontsource/jetbrains-mono/700.css';
	// IBM Plex Mono - editorial, monochrome, wireframe
	import '@fontsource/ibm-plex-mono/300.css';
	import '@fontsource/ibm-plex-mono/400.css';
	import '@fontsource/ibm-plex-mono/500.css';
	import '@fontsource/ibm-plex-mono/600.css';
	import '@fontsource/ibm-plex-mono/700.css';
	// Source Sans Pro - editorial, organic-flow
	import '@fontsource/source-sans-pro/300.css';
	import '@fontsource/source-sans-pro/400.css';
	import '@fontsource/source-sans-pro/600.css';
	import '@fontsource/source-sans-pro/700.css';
	// Source Code Pro - organic-flow, retro-futurism
	import '@fontsource/source-code-pro/300.css';
	import '@fontsource/source-code-pro/400.css';
	import '@fontsource/source-code-pro/500.css';
	import '@fontsource/source-code-pro/600.css';
	import '@fontsource/source-code-pro/700.css';
	// Orbitron - cyberpunk, retro-futurism
	import '@fontsource/orbitron/400.css';
	import '@fontsource/orbitron/500.css';
	import '@fontsource/orbitron/600.css';
	import '@fontsource/orbitron/700.css';
	import '@fontsource/orbitron/800.css';
	import '@fontsource/orbitron/900.css';
	// === THEME-SPECIFIC FONTS ===
	// Cyberpunk - Exo 2
	import '@fontsource/exo-2/300.css';
	import '@fontsource/exo-2/400.css';
	import '@fontsource/exo-2/500.css';
	import '@fontsource/exo-2/600.css';
	// Neu-Brutalist - Space Grotesk, Space Mono
	import '@fontsource/space-grotesk/300.css';
	import '@fontsource/space-grotesk/400.css';
	import '@fontsource/space-grotesk/500.css';
	import '@fontsource/space-grotesk/600.css';
	import '@fontsource/space-grotesk/700.css';
	import '@fontsource/space-mono/400.css';
	import '@fontsource/space-mono/700.css';
	// Claymorphic - Poppins, Quicksand
	import '@fontsource/poppins/300.css';
	import '@fontsource/poppins/400.css';
	import '@fontsource/poppins/500.css';
	import '@fontsource/poppins/600.css';
	import '@fontsource/poppins/700.css';
	import '@fontsource/quicksand/300.css';
	import '@fontsource/quicksand/400.css';
	import '@fontsource/quicksand/500.css';
	import '@fontsource/quicksand/600.css';
	import '@fontsource/quicksand/700.css';
	// Editorial - Playfair Display
	import '@fontsource/playfair-display/400.css';
	import '@fontsource/playfair-display/500.css';
	import '@fontsource/playfair-display/600.css';
	import '@fontsource/playfair-display/700.css';
	import '@fontsource/playfair-display/800.css';
	import '@fontsource/playfair-display/900.css';
	// Flat - Open Sans, Lato, Roboto Mono
	import '@fontsource/lato/300.css';
	import '@fontsource/lato/400.css';
	import '@fontsource/lato/700.css';
	import '@fontsource/lato/900.css';
	import '@fontsource/open-sans/300.css';
	import '@fontsource/open-sans/400.css';
	import '@fontsource/open-sans/500.css';
	import '@fontsource/open-sans/600.css';
	import '@fontsource/open-sans/700.css';
	import '@fontsource/open-sans/800.css';
	import '@fontsource/roboto-mono/300.css';
	import '@fontsource/roboto-mono/400.css';
	import '@fontsource/roboto-mono/500.css';
	import '@fontsource/roboto-mono/600.css';
	import '@fontsource/roboto-mono/700.css';
	// Industrial - Bebas Neue
	import '@fontsource/bebas-neue/400.css';

	// Japanese Minimalist - Noto Sans JP, Source Serif Pro, Noto Sans Mono
	import '@fontsource/noto-sans-jp/300.css';
	import '@fontsource/noto-sans-jp/400.css';
	import '@fontsource/noto-sans-jp/500.css';
	import '@fontsource/noto-sans-jp/700.css';
	import '@fontsource/noto-sans-jp/900.css';
	import '@fontsource/noto-sans-mono/300.css';
	import '@fontsource/noto-sans-mono/400.css';
	import '@fontsource/noto-sans-mono/500.css';
	import '@fontsource/noto-sans-mono/600.css';
	import '@fontsource/noto-sans-mono/700.css';
	import '@fontsource/source-serif-pro/300.css';
	import '@fontsource/source-serif-pro/400.css';
	import '@fontsource/source-serif-pro/600.css';
	import '@fontsource/source-serif-pro/700.css';
	// Organic Flow - Comfortaa
	import '@fontsource/comfortaa/300.css';
	import '@fontsource/comfortaa/400.css';
	import '@fontsource/comfortaa/500.css';
	import '@fontsource/comfortaa/600.css';
	import '@fontsource/comfortaa/700.css';
	// Pixel Art - Press Start 2P, VT323
	import '@fontsource/press-start-2p/400.css';
	import '@fontsource/vt323/400.css';
	// Retro Futurism - Share Tech Mono
	import '@fontsource/share-tech-mono/400.css';

	let { children } = $props();
</script>

{@render children()}
