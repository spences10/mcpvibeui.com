<script lang="ts">
	const features = [
		{
			title: 'PURRFECT MATCHES',
			desc: 'AI-powered whisker recognition',
			icon: '🐱',
		},
		{
			title: 'MEOW MESSAGING',
			desc: 'Real-time cat chat',
			icon: '💬',
		},
		{
			title: 'TREATS & DATES',
			desc: 'Find local cat cafes',
			icon: '🍪',
		},
	];

	const testimonials = [
		{
			name: 'Mr. Whiskers',
			quote: 'Found my soulmate in 3 purrs!',
			avatar: '😺',
		},
		{
			name: 'Princess Fluff',
			quote: 'Finally, a dating app that gets me.',
			avatar: '😻',
		},
		{
			name: 'Sir Meowington',
			quote: '10/10 would swipe right again.',
			avatar: '🐈',
		},
	];
</script>

<div class="bg-background text-foreground min-h-screen">
	<!-- NAV -->
	<nav class="border-foreground bg-accent border-b-4 p-4">
		<div class="mx-auto flex max-w-6xl items-center justify-between">
			<div class="flex items-center gap-2 text-2xl font-bold">
				<span class="-rotate-3 text-4xl">🐾</span>
				<span
					class="font-(family-name:--font-display) tracking-tight"
				>
					PAWMATCH
				</span>
			</div>
			<div class="flex gap-4">
				<a href="#features" class="font-bold hover:underline">
					FEATURES
				</a>
				<a href="#testimonials" class="font-bold hover:underline">
					REVIEWS
				</a>
			</div>
		</div>
	</nav>

	<!-- HERO -->
	<section
		class="border-foreground bg-secondary relative overflow-hidden border-b-4 px-4 py-20"
	>
		<div class="mx-auto max-w-6xl">
			<div class="grid gap-8 md:grid-cols-2 md:items-center">
				<div>
					<h1
						class="mb-6 font-(family-name:--font-display) text-5xl leading-none font-black md:text-7xl"
					>
						FIND YOUR
						<span
							class="bg-primary text-primary-foreground block rotate-1 px-2"
						>
							PURRFECT
						</span>
						MATCH
					</h1>
					<p class="mb-8 max-w-md text-xl font-medium">
						The brutally honest dating app for cats. No games. No
						hairballs. Just love.
					</p>
					<div class="flex flex-wrap gap-4">
						<button
							class="border-foreground bg-primary text-primary-foreground border-4 px-8 py-4 text-lg font-bold shadow-[8px_8px_0_0_#000] transition-all hover:translate-x-1 hover:translate-y-1 hover:shadow-[4px_4px_0_0_#000]"
						>
							GET STARTED FREE
						</button>
						<button
							class="border-foreground bg-background border-4 px-8 py-4 text-lg font-bold shadow-[8px_8px_0_0_#000] transition-all hover:translate-x-1 hover:translate-y-1 hover:shadow-[4px_4px_0_0_#000]"
						>
							LEARN MORE
						</button>
					</div>
				</div>
				<div class="relative flex justify-center">
					<div
						class="border-foreground bg-warning relative rotate-2 border-4 p-8 shadow-[12px_12px_0_0_#000]"
						style="animation: float 3s ease-in-out infinite;"
					>
						<span class="text-9xl">😻</span>
						<div
							class="border-foreground bg-primary text-primary-foreground absolute -top-4 -right-4 rotate-12 border-4 px-3 py-1 text-sm font-bold"
						>
							ONLINE
						</div>
					</div>
					<div
						class="border-foreground bg-accent absolute -bottom-4 -left-4 -rotate-3 border-4 p-4 shadow-[8px_8px_0_0_#000]"
					>
						<span class="text-4xl">💕</span>
					</div>
				</div>
			</div>
		</div>
	</section>

	<!-- STATS -->
	<section class="border-foreground bg-muted border-b-4">
		<div class="mx-auto grid max-w-6xl grid-cols-2 md:grid-cols-4">
			{#each [{ num: '10K+', label: 'HAPPY CATS' }, { num: '500+', label: 'MATCHES/DAY' }, { num: '99%', label: 'PURR RATE' }, { num: '24/7', label: 'NAP SUPPORT' }] as stat, i}
				<div
					class="border-foreground border-r-4 p-6 text-center last:border-r-0 {i %
						2 ===
					0
						? 'bg-accent'
						: 'bg-warning'}"
				>
					<div
						class="font-(family-name:--font-display) text-4xl font-black"
					>
						{stat.num}
					</div>
					<div class="text-sm font-bold">{stat.label}</div>
				</div>
			{/each}
		</div>
	</section>

	<!-- FEATURES -->
	<section
		id="features"
		class="border-foreground bg-background border-b-4 px-4 py-20"
	>
		<div class="mx-auto max-w-6xl">
			<h2
				class="mb-12 text-center font-(family-name:--font-display) text-4xl font-black md:text-5xl"
			>
				WHY PAWMATCH<span class="text-primary inline-block rotate-3">
					?
				</span>
			</h2>
			<div class="grid gap-6 md:grid-cols-3">
				{#each features as feature, i}
					<div
						class="border-foreground border-4 p-6 shadow-[8px_8px_0_0_#000] transition-all hover:-translate-x-1 hover:-translate-y-1 hover:shadow-[12px_12px_0_0_#000] {i ===
						0
							? 'bg-primary text-primary-foreground rotate-1'
							: i === 1
								? 'bg-secondary text-secondary-foreground -rotate-1'
								: 'bg-accent text-accent-foreground rotate-1'}"
					>
						<span class="mb-4 block text-5xl">{feature.icon}</span>
						<h3
							class="mb-2 font-(family-name:--font-display) text-2xl font-black"
						>
							{feature.title}
						</h3>
						<p class="font-medium">{feature.desc}</p>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- TESTIMONIALS -->
	<section
		id="testimonials"
		class="border-foreground bg-warning border-b-4 px-4 py-20"
	>
		<div class="mx-auto max-w-6xl">
			<h2
				class="mb-12 text-center font-(family-name:--font-display) text-4xl font-black"
			>
				WHAT CATS SAY
			</h2>
			<div class="grid gap-6 md:grid-cols-3">
				{#each testimonials as t, i}
					<div
						class="border-foreground bg-background border-4 p-6 shadow-[8px_8px_0_0_#000] {i ===
						1
							? '-rotate-1'
							: 'rotate-1'}"
					>
						<span class="mb-4 block text-6xl">{t.avatar}</span>
						<p class="mb-4 text-lg font-medium">"{t.quote}"</p>
						<p class="font-(family-name:--font-display) font-bold">
							- {t.name}
						</p>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- CTA -->
	<section
		class="border-foreground bg-primary text-primary-foreground border-b-4 px-4 py-20"
	>
		<div class="mx-auto max-w-3xl text-center">
			<h2
				class="mb-6 font-(family-name:--font-display) text-4xl font-black md:text-6xl"
			>
				READY TO FIND LOVE?
			</h2>
			<p class="mb-8 text-xl">
				Join thousands of cats finding their purrfect match every day.
			</p>
			<button
				class="border-foreground bg-background text-foreground border-4 px-10 py-5 text-xl font-bold shadow-[8px_8px_0_0_#000] transition-all hover:translate-x-1 hover:translate-y-1 hover:shadow-[4px_4px_0_0_#000]"
			>
				START MATCHING NOW
			</button>
		</div>
	</section>

	<!-- FOOTER -->
	<footer class="bg-foreground text-background p-8">
		<div
			class="mx-auto flex max-w-6xl flex-col items-center justify-between gap-4 md:flex-row"
		>
			<div class="flex items-center gap-2 text-xl font-bold">
				<span>🐾</span>
				<span class="font-(family-name:--font-display)">PAWMATCH</span
				>
			</div>
			<div class="flex gap-6">
				<a href="#" class="hover:underline">PRIVACY</a>
				<a href="#" class="hover:underline">TERMS</a>
				<a href="#" class="hover:underline">CONTACT</a>
			</div>
			<p class="font-mono text-sm">2025 PAWMATCH INC.</p>
		</div>
	</footer>
</div>
