<script lang="ts">
	const features = [
		{
			icon: '🐱',
			title: 'Purrfect Matches',
			description:
				'AI-powered matching finds cats with compatible personalities',
		},
		{
			icon: '💕',
			title: 'Whisker Connections',
			description: 'Connect with feline friends in your neighborhood',
		},
		{
			icon: '🏠',
			title: 'Safe Meetups',
			description: 'Verified profiles and safe meeting locations',
		},
	];

	const testimonials = [
		{
			name: 'Mr. Whiskers',
			quote: 'Found my soulmate! We nap together every day now.',
			avatar: '😺',
		},
		{
			name: 'Princess Fluffington',
			quote: 'Finally, an app that understands feline romance.',
			avatar: '😻',
		},
		{
			name: 'Shadow',
			quote: 'Met the love of my nine lives here!',
			avatar: '🐈‍⬛',
		},
	];
</script>

<div class="bg-background text-foreground min-h-screen">
	<!-- Nav -->
	<nav class="px-6 py-4">
		<div class="mx-auto flex max-w-6xl items-center justify-between">
			<div
				class="flex items-center gap-2 rounded-xl px-4 py-2 shadow-[5px_5px_10px_#d1d9e6,-5px_-5px_10px_#ffffff]"
			>
				<span class="text-2xl">😻</span>
				<span class="text-xl font-semibold">PurrMatch</span>
			</div>
			<div class="flex gap-4">
				<button
					class="rounded-xl px-6 py-2 shadow-[5px_5px_10px_#d1d9e6,-5px_-5px_10px_#ffffff] transition-all hover:shadow-[3px_3px_6px_#d1d9e6,-3px_-3px_6px_#ffffff] active:shadow-[inset_5px_5px_10px_#d1d9e6,inset_-5px_-5px_10px_#ffffff]"
				>
					Login
				</button>
				<button
					class="bg-primary text-primary-foreground rounded-xl px-6 py-2 shadow-[5px_5px_10px_#d1d9e6,-5px_-5px_10px_#ffffff] transition-all hover:shadow-[3px_3px_6px_#d1d9e6,-3px_-3px_6px_#ffffff] active:shadow-[inset_5px_5px_10px_#d1d9e6,inset_-5px_-5px_10px_#ffffff]"
				>
					Sign Up
				</button>
			</div>
		</div>
	</nav>

	<!-- Hero -->
	<section class="px-6 py-20">
		<div class="mx-auto max-w-6xl text-center">
			<div
				class="mb-8 inline-block animate-[float_3s_ease-in-out_infinite] text-8xl"
			>
				😻
			</div>
			<h1 class="mb-6 text-5xl font-bold tracking-tight md:text-6xl">
				Find Your Cat's<br />
				<span class="text-primary">Purrfect Match</span>
			</h1>
			<p
				class="text-muted-foreground mx-auto mb-10 max-w-2xl text-lg"
			>
				The premier dating app for cats. Because every whisker
				deserves love. Join thousands of felines finding
				companionship.
			</p>
			<div class="flex justify-center gap-4">
				<button
					class="bg-primary text-primary-foreground rounded-2xl px-8 py-4 text-lg font-semibold shadow-[8px_8px_16px_#d1d9e6,-8px_-8px_16px_#ffffff] transition-all hover:shadow-[4px_4px_8px_#d1d9e6,-4px_-4px_8px_#ffffff] active:shadow-[inset_5px_5px_10px_#d1d9e6,inset_-5px_-5px_10px_#ffffff]"
				>
					Get Started Free
				</button>
				<button
					class="rounded-2xl px-8 py-4 text-lg font-semibold shadow-[8px_8px_16px_#d1d9e6,-8px_-8px_16px_#ffffff] transition-all hover:shadow-[4px_4px_8px_#d1d9e6,-4px_-4px_8px_#ffffff] active:shadow-[inset_5px_5px_10px_#d1d9e6,inset_-5px_-5px_10px_#ffffff]"
				>
					Learn More
				</button>
			</div>
		</div>
	</section>

	<!-- Features -->
	<section class="px-6 py-20">
		<div class="mx-auto max-w-6xl">
			<h2 class="mb-12 text-center text-3xl font-bold">
				Why Cats Love Us
			</h2>
			<div class="grid gap-8 md:grid-cols-3">
				{#each features as feature}
					<div
						class="bg-background rounded-2xl p-8 shadow-[8px_8px_16px_rgba(0,0,0,0.1),-8px_-8px_16px_rgba(255,255,255,0.8)] transition-all hover:-translate-y-1 hover:shadow-[12px_12px_24px_rgba(0,0,0,0.1),-12px_-12px_24px_rgba(255,255,255,0.8)]"
					>
						<div
							class="mb-4 inline-flex h-16 w-16 items-center justify-center rounded-2xl text-3xl shadow-[inset_4px_4px_8px_rgba(0,0,0,0.1),inset_-4px_-4px_8px_rgba(255,255,255,0.8)]"
						>
							{feature.icon}
						</div>
						<h3 class="mb-2 text-xl font-semibold">
							{feature.title}
						</h3>
						<p class="text-muted-foreground">{feature.description}</p>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- Stats -->
	<section class="px-6 py-20">
		<div class="mx-auto max-w-4xl">
			<div
				class="bg-background grid gap-8 rounded-3xl p-10 shadow-[8px_8px_16px_rgba(0,0,0,0.1),-8px_-8px_16px_rgba(255,255,255,0.8)] md:grid-cols-3"
			>
				<div class="text-center">
					<div class="text-primary text-4xl font-bold">50K+</div>
					<div class="text-muted-foreground">Happy Cats</div>
				</div>
				<div class="text-center">
					<div class="text-secondary text-4xl font-bold">25K+</div>
					<div class="text-muted-foreground">Matches Made</div>
				</div>
				<div class="text-center">
					<div class="text-accent-foreground text-4xl font-bold">
						99%
					</div>
					<div class="text-muted-foreground">Satisfaction</div>
				</div>
			</div>
		</div>
	</section>

	<!-- Testimonials -->
	<section class="px-6 py-20">
		<div class="mx-auto max-w-6xl">
			<h2 class="mb-12 text-center text-3xl font-bold">
				Success Stories
			</h2>
			<div class="grid gap-8 md:grid-cols-3">
				{#each testimonials as testimonial}
					<div
						class="bg-background rounded-2xl p-6 shadow-[8px_8px_16px_rgba(0,0,0,0.1),-8px_-8px_16px_rgba(255,255,255,0.8)]"
					>
						<div class="mb-4 flex items-center gap-3">
							<div
								class="flex h-12 w-12 items-center justify-center rounded-full text-2xl shadow-[inset_4px_4px_8px_rgba(0,0,0,0.1),inset_-4px_-4px_8px_rgba(255,255,255,0.8)]"
							>
								{testimonial.avatar}
							</div>
							<span class="font-semibold">{testimonial.name}</span>
						</div>
						<p class="text-muted-foreground italic">
							"{testimonial.quote}"
						</p>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- CTA -->
	<section class="px-6 py-20">
		<div class="mx-auto max-w-2xl text-center">
			<div
				class="bg-background rounded-3xl p-12 shadow-[8px_8px_16px_rgba(0,0,0,0.1),-8px_-8px_16px_rgba(255,255,255,0.8)]"
			>
				<h2 class="mb-4 text-3xl font-bold">Ready to Find Love?</h2>
				<p class="text-muted-foreground mb-8">
					Join PurrMatch today and let your cat discover their
					purrfect companion.
				</p>
				<div
					class="mx-auto max-w-md rounded-2xl p-2 shadow-[inset_4px_4px_8px_rgba(0,0,0,0.1),inset_-4px_-4px_8px_rgba(255,255,255,0.8)]"
				>
					<div class="flex gap-2">
						<input
							type="email"
							placeholder="Enter your email"
							class="bg-background flex-1 rounded-xl px-4 py-3 shadow-[inset_2px_2px_4px_rgba(0,0,0,0.05),inset_-2px_-2px_4px_rgba(255,255,255,0.5)] outline-none"
						/>
						<button
							class="bg-primary text-primary-foreground rounded-xl px-6 py-3 font-semibold shadow-[5px_5px_10px_#d1d9e6,-5px_-5px_10px_#ffffff] transition-all active:shadow-[inset_5px_5px_10px_#d1d9e6,inset_-5px_-5px_10px_#ffffff]"
						>
							Join
						</button>
					</div>
				</div>
			</div>
		</div>
	</section>

	<!-- Footer -->
	<footer class="px-6 py-10">
		<div
			class="bg-background mx-auto max-w-6xl rounded-2xl p-8 shadow-[8px_8px_16px_rgba(0,0,0,0.1),-8px_-8px_16px_rgba(255,255,255,0.8)]"
		>
			<div
				class="flex flex-col items-center justify-between gap-4 md:flex-row"
			>
				<div class="flex items-center gap-2">
					<span class="text-2xl">😻</span>
					<span class="text-xl font-semibold">PurrMatch</span>
				</div>
				<div class="text-muted-foreground flex gap-6">
					<a href="#about" class="hover:text-foreground">About</a>
					<a href="#privacy" class="hover:text-foreground">Privacy</a>
					<a href="#terms" class="hover:text-foreground">Terms</a>
					<a href="#contact" class="hover:text-foreground">Contact</a>
				</div>
				<p class="text-muted-foreground text-sm">
					2025 PurrMatch. All rights reserved.
				</p>
			</div>
		</div>
	</footer>
</div>
