<script lang="ts">
	let email = $state('');
</script>

<svelte:head>
	<title>PurrConnect | Find Your Cat's Soulmate</title>
</svelte:head>

<div
	class="bg-background text-foreground relative min-h-screen overflow-hidden"
>
	<!-- Scanlines overlay -->
	<div
		class="pointer-events-none fixed inset-0 z-50 bg-[repeating-linear-gradient(0deg,transparent_0px,rgba(255,0,128,0.03)_1px,rgba(255,0,128,0.03)_2px,transparent_3px)]"
	></div>

	<!-- Grid background -->
	<div
		class="fixed inset-0 opacity-20"
		style="background-image:
			repeating-linear-gradient(90deg, transparent, transparent 79px, rgba(255,0,128,0.3) 79px, rgba(255,0,128,0.3) 81px),
			repeating-linear-gradient(0deg, transparent, transparent 79px, rgba(0,255,255,0.2) 79px, rgba(0,255,255,0.2) 81px)"
	></div>

	<!-- Navigation -->
	<nav
		class="relative z-40 flex items-center justify-between px-8 py-6"
	>
		<div
			class="text-primary font-[Orbitron] text-2xl font-bold"
			style="animation: neon-flicker 3s ease-in-out infinite"
		>
			PURRCONNECT
		</div>
		<div class="flex gap-6 font-[Share_Tech_Mono] text-sm">
			<a
				href="#features"
				class="text-muted-foreground hover:text-primary transition-colors"
			>
				FEATURES
			</a>
			<a
				href="#how"
				class="text-muted-foreground hover:text-primary transition-colors"
			>
				HOW IT WORKS
			</a>
			<a
				href="#testimonials"
				class="text-muted-foreground hover:text-primary transition-colors"
			>
				TESTIMONIALS
			</a>
		</div>
		<button
			class="border-primary bg-primary/10 text-primary hover:bg-primary hover:text-primary-foreground rounded border px-6 py-2 font-[Share_Tech_Mono] text-sm transition-all hover:shadow-[0_0_30px_var(--color-primary)]"
		>
			SIGN IN
		</button>
	</nav>

	<!-- Hero Section -->
	<section
		class="relative z-10 flex min-h-[80vh] flex-col items-center justify-center px-8 text-center"
	>
		<!-- Floating cat silhouette -->
		<div
			class="absolute top-1/4 left-1/4 text-8xl opacity-20"
			style="animation: float 4s ease-in-out infinite"
		>
			🐱
		</div>
		<div
			class="absolute right-1/4 bottom-1/4 text-8xl opacity-20"
			style="animation: float 4s ease-in-out infinite 1s"
		>
			😻
		</div>

		<p
			class="text-accent mb-4 font-[Share_Tech_Mono] text-sm tracking-[0.3em] uppercase"
		>
			// THE FUTURE OF FELINE ROMANCE
		</p>

		<h1
			class="mb-6 font-[Orbitron] text-6xl leading-tight font-black uppercase md:text-8xl"
			style="text-shadow: 0 0 40px var(--color-primary), 0 0 80px var(--color-secondary)"
		>
			<span class="text-primary">PURR</span><span
				class="text-secondary">CONNECT</span
			>
		</h1>

		<p
			class="text-muted-foreground mb-8 max-w-2xl font-[Share_Tech_Mono] text-xl"
		>
			Where whiskers meet destiny. Advanced AI matching for cats
			seeking companionship in the digital age.
		</p>

		<!-- CTA Form -->
		<div class="flex flex-col items-center gap-4 sm:flex-row">
			<input
				type="email"
				placeholder="enter_your_email.cat"
				bind:value={email}
				class="border-primary/50 bg-muted text-foreground placeholder:text-muted-foreground focus:border-primary w-80 rounded border px-6 py-4 font-[Source_Code_Pro] focus:shadow-[0_0_20px_var(--color-primary)] focus:outline-none"
			/>
			<button
				class="bg-primary text-primary-foreground rounded px-8 py-4 font-[Orbitron] font-bold uppercase transition-all hover:shadow-[0_0_40px_var(--color-primary)]"
				style="animation: pulse-glow 2s ease-in-out infinite"
			>
				JOIN WAITLIST
			</button>
		</div>

		<p
			class="text-muted-foreground mt-6 font-[Share_Tech_Mono] text-sm"
		>
			<span class="text-success">●</span> 50,000+ cats already waiting
		</p>
	</section>

	<!-- Features Section -->
	<section id="features" class="relative z-10 px-8 py-24">
		<h2
			class="text-foreground mb-16 text-center font-[Orbitron] text-4xl font-bold uppercase"
		>
			<span class="text-accent">[</span> FEATURES
			<span class="text-accent">]</span>
		</h2>

		<div class="mx-auto grid max-w-6xl gap-8 md:grid-cols-3">
			<!-- Feature 1 -->
			<div
				class="border-primary/30 bg-muted hover:border-primary rounded border p-8 transition-all hover:shadow-[0_0_30px_rgba(255,0,128,0.2)]"
			>
				<div class="mb-4 text-5xl">🧬</div>
				<h3
					class="text-primary mb-3 font-[Orbitron] text-xl font-bold"
				>
					AI PAWSONALITY MATCH
				</h3>
				<p
					class="text-muted-foreground font-[Share_Tech_Mono] text-sm"
				>
					Our neural network analyzes 47 meow patterns and 128 purr
					frequencies to find the purrfect match.
				</p>
			</div>

			<!-- Feature 2 -->
			<div
				class="border-secondary/30 bg-muted hover:border-secondary rounded border p-8 transition-all hover:shadow-[0_0_30px_rgba(138,43,226,0.2)]"
			>
				<div class="mb-4 text-5xl">📡</div>
				<h3
					class="text-secondary mb-3 font-[Orbitron] text-xl font-bold"
				>
					QUANTUM WHISKER SYNC
				</h3>
				<p
					class="text-muted-foreground font-[Share_Tech_Mono] text-sm"
				>
					Entangled whisker technology ensures your cats vibe on the
					same cosmic frequency.
				</p>
			</div>

			<!-- Feature 3 -->
			<div
				class="border-accent/30 bg-muted hover:border-accent rounded border p-8 transition-all hover:shadow-[0_0_30px_rgba(0,255,255,0.2)]"
			>
				<div class="mb-4 text-5xl">🛸</div>
				<h3
					class="text-accent mb-3 font-[Orbitron] text-xl font-bold"
				>
					HOLOGRAPHIC DATES
				</h3>
				<p
					class="text-muted-foreground font-[Share_Tech_Mono] text-sm"
				>
					Virtual reality playdates let cats meet without leaving
					their favorite sunspot.
				</p>
			</div>
		</div>
	</section>

	<!-- How It Works -->
	<section id="how" class="relative z-10 px-8 py-24">
		<h2
			class="text-foreground mb-16 text-center font-[Orbitron] text-4xl font-bold uppercase"
		>
			<span class="text-primary">&lt;</span> PROTOCOL
			<span class="text-primary">/&gt;</span>
		</h2>

		<div class="mx-auto flex max-w-4xl flex-col gap-8">
			{#each [{ step: '01', title: 'UPLOAD PROFILE', desc: 'Scan your cat with our proprietary PhotonPaw™ technology' }, { step: '02', title: 'AI ANALYSIS', desc: 'Our algorithms decode their unique feline signature' }, { step: '03', title: 'MATCH PROTOCOL', desc: 'Receive quantum-certified compatible companions' }, { step: '04', title: 'INITIATE CONTACT', desc: 'Begin secure meow-to-meow communication' }] as item}
				<div
					class="border-border bg-muted/50 hover:border-primary/50 hover:bg-muted flex items-center gap-6 rounded border p-6 transition-all"
				>
					<div
						class="border-primary bg-primary/10 text-primary flex h-16 w-16 items-center justify-center rounded border font-[Orbitron] text-2xl font-bold"
					>
						{item.step}
					</div>
					<div>
						<h3
							class="text-foreground font-[Orbitron] text-lg font-bold"
						>
							{item.title}
						</h3>
						<p
							class="text-muted-foreground font-[Share_Tech_Mono] text-sm"
						>
							{item.desc}
						</p>
					</div>
				</div>
			{/each}
		</div>
	</section>

	<!-- Testimonials -->
	<section id="testimonials" class="relative z-10 px-8 py-24">
		<h2
			class="text-foreground mb-16 text-center font-[Orbitron] text-4xl font-bold uppercase"
		>
			<span class="text-secondary">/*</span> TRANSMISSIONS
			<span class="text-secondary">*/</span>
		</h2>

		<div class="mx-auto grid max-w-5xl gap-8 md:grid-cols-2">
			{#each [{ name: 'WHISKERS_9000', location: 'Neo Tokyo', quote: 'Found my soulmate across the datastream. Our frequencies are perfectly synchronized.' }, { name: 'CYBER_MITTENS', location: 'Los Angeles 2049', quote: 'The holographic dates are incredible. We chase laser pointers through virtual space.' }, { name: 'COMMANDER_FLOOF', location: 'Orbital Station 7', quote: 'Even in zero gravity, PurrConnect found me love. 10/10 would meow again.' }, { name: 'NEON_PAWS', location: 'Sector 9', quote: 'The AI understood my complex personality. I am no longer a solo glitch in the matrix.' }] as testimonial}
				<div
					class="border-border bg-background/50 hover:border-secondary/50 rounded border p-6 backdrop-blur-sm transition-all"
				>
					<p
						class="text-muted-foreground mb-4 font-[Share_Tech_Mono]"
					>
						"{testimonial.quote}"
					</p>
					<div class="flex items-center gap-2">
						<span class="text-2xl">😺</span>
						<div>
							<p
								class="text-primary font-[Orbitron] text-sm font-bold"
							>
								{testimonial.name}
							</p>
							<p
								class="text-muted-foreground font-[Source_Code_Pro] text-xs"
							>
								{testimonial.location}
							</p>
						</div>
					</div>
				</div>
			{/each}
		</div>
	</section>

	<!-- CTA Section -->
	<section class="relative z-10 px-8 py-24 text-center">
		<div
			class="border-primary/50 bg-muted mx-auto max-w-3xl rounded border p-12"
			style="box-shadow: 0 0 60px rgba(255,0,128,0.2), inset 0 0 60px rgba(255,0,128,0.05)"
		>
			<h2
				class="text-foreground mb-4 font-[Orbitron] text-4xl font-bold uppercase"
			>
				READY TO <span class="text-primary">CONNECT</span>?
			</h2>
			<p class="text-muted-foreground mb-8 font-[Share_Tech_Mono]">
				Join the future of feline matchmaking. Your cat's destiny
				awaits in the digital realm.
			</p>
			<button
				class="from-primary to-secondary rounded bg-gradient-to-r px-12 py-4 font-[Orbitron] text-lg font-bold text-white uppercase transition-all hover:shadow-[0_0_50px_var(--color-primary)]"
			>
				ACTIVATE PROTOCOL
			</button>
		</div>
	</section>

	<!-- Footer -->
	<footer class="border-border relative z-10 border-t px-8 py-12">
		<div
			class="mx-auto flex max-w-6xl flex-col items-center justify-between gap-6 md:flex-row"
		>
			<div class="text-primary font-[Orbitron] text-xl font-bold">
				PURRCONNECT
			</div>
			<div
				class="text-muted-foreground flex gap-6 font-[Source_Code_Pro] text-xs"
			>
				<span>TERMS.exe</span>
				<span>PRIVACY.cfg</span>
				<span>SUPPORT.sys</span>
			</div>
			<p class="text-muted-foreground font-[Share_Tech_Mono] text-xs">
				© 2049 PURRCONNECT INDUSTRIES. ALL RIGHTS RESERVED.
			</p>
		</div>
	</footer>
</div>
