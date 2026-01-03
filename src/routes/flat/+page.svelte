<script lang="ts">
	const features = [
		{
			icon: '🐱',
			title: 'Purrfect Matches',
			desc: 'AI-powered matching based on personality, breed preferences, and lifestyle',
		},
		{
			icon: '📍',
			title: 'Local Kitties',
			desc: 'Find feline friends in your neighborhood for playdates',
		},
		{
			icon: '💬',
			title: 'Cat Chat',
			desc: 'Message other cat parents and arrange meetups',
		},
		{
			icon: '📸',
			title: 'Photo Albums',
			desc: 'Share unlimited photos of your adorable fur babies',
		},
	];

	const testimonials = [
		{
			name: 'Whiskers & Luna',
			text: 'Found my cat her best friend! They nap together every day now.',
			avatar: '😺',
		},
		{
			name: 'Mr. Fluffington',
			text: 'Finally a dating app that understands cats are the priority.',
			avatar: '😸',
		},
		{
			name: 'Shadow & Mittens',
			text: 'Our cats fell in love at first sniff. Wedding bells soon!',
			avatar: '😻',
		},
	];
</script>

<div class="min-h-screen">
	<!-- Nav -->
	<nav
		class="bg-base-100 flex items-center justify-between px-6 py-4"
	>
		<div class="flex items-center gap-2">
			<span class="text-3xl">😻</span>
			<span class="text-primary font-display text-xl font-bold"
				>PurrMeet</span
			>
		</div>
		<div class="flex items-center gap-4">
			<a
				href="#features"
				class="text-base-content/70 hover:text-primary transition-colors"
				>Features</a
			>
			<a
				href="#testimonials"
				class="text-base-content/70 hover:text-primary transition-colors"
				>Stories</a
			>
			<button
				class="bg-primary text-primary-content rounded-(--radius-field) px-4 py-2 font-semibold transition-opacity hover:opacity-90"
			>
				Get Started
			</button>
		</div>
	</nav>

	<!-- Hero -->
	<section class="bg-base-200 px-6 py-20 text-center">
		<div class="mx-auto max-w-3xl">
			<h1
				class="text-base-content font-display mb-6 text-5xl font-bold md:text-6xl"
			>
				Find Your Cat's <span class="text-primary">Soulmate</span>
			</h1>
			<p class="text-base-content/70 mx-auto mb-8 max-w-xl text-xl">
				The #1 dating app for cats and their humans. Swipe right on
				love, friendship, and endless cuddle puddles.
			</p>
			<div class="flex flex-col justify-center gap-4 sm:flex-row">
				<button
					class="bg-primary text-primary-content rounded-(--radius-field) px-8 py-3 text-lg font-semibold transition-opacity hover:opacity-90"
				>
					Download Free
				</button>
				<button
					class="bg-base-300 text-base-content hover:bg-base-300/80 rounded-(--radius-field) px-8 py-3 text-lg font-semibold transition-colors"
				>
					Learn More
				</button>
			</div>
			<p class="text-base-content/50 mt-6 text-sm">
				Join 50,000+ happy cats and their humans
			</p>
		</div>

		<!-- Hero illustration -->
		<div class="mt-16 flex justify-center gap-8 text-8xl">
			<span class="animate-bounce" style="animation-delay: 0ms;"
				>🐱</span
			>
			<span class="text-secondary self-center text-6xl">💕</span>
			<span class="animate-bounce" style="animation-delay: 200ms;"
				>😺</span
			>
		</div>
	</section>

	<!-- Features -->
	<section id="features" class="bg-base-100 px-6 py-20">
		<div class="mx-auto max-w-5xl">
			<h2
				class="font-display mb-4 text-center text-3xl font-bold md:text-4xl"
			>
				Why Cats Love Us
			</h2>
			<p
				class="text-base-content/60 mx-auto mb-12 max-w-xl text-center"
			>
				Everything your feline friend needs to find their purrfect
				match
			</p>

			<div class="grid gap-6 md:grid-cols-2 lg:grid-cols-4">
				{#each features as feature}
					<div class="bg-base-200 rounded-(--radius-box) p-6">
						<div class="mb-4 text-4xl">{feature.icon}</div>
						<h3 class="font-display mb-2 text-lg font-semibold">
							{feature.title}
						</h3>
						<p class="text-base-content/60 text-sm">{feature.desc}</p>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- Stats -->
	<section class="bg-primary text-primary-content px-6 py-16">
		<div
			class="mx-auto grid max-w-4xl grid-cols-2 gap-8 text-center md:grid-cols-4"
		>
			<div>
				<div class="font-display text-4xl font-bold">50K+</div>
				<div class="text-primary-content/70 mt-1 text-sm">
					Happy Cats
				</div>
			</div>
			<div>
				<div class="font-display text-4xl font-bold">12K</div>
				<div class="text-primary-content/70 mt-1 text-sm">
					Matches Made
				</div>
			</div>
			<div>
				<div class="font-display text-4xl font-bold">98%</div>
				<div class="text-primary-content/70 mt-1 text-sm">
					Purr Rate
				</div>
			</div>
			<div>
				<div class="font-display text-4xl font-bold">4.9</div>
				<div class="text-primary-content/70 mt-1 text-sm">
					App Rating
				</div>
			</div>
		</div>
	</section>

	<!-- Testimonials -->
	<section id="testimonials" class="bg-base-200 px-6 py-20">
		<div class="mx-auto max-w-5xl">
			<h2
				class="font-display mb-12 text-center text-3xl font-bold md:text-4xl"
			>
				Love Stories
			</h2>

			<div class="grid gap-6 md:grid-cols-3">
				{#each testimonials as t}
					<div class="bg-base-100 rounded-(--radius-box) p-6">
						<div class="mb-4 text-5xl">{t.avatar}</div>
						<p class="text-base-content/70 mb-4 italic">"{t.text}"</p>
						<p class="text-sm font-semibold">{t.name}</p>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- CTA -->
	<section class="bg-base-100 px-6 py-20 text-center">
		<div class="mx-auto max-w-2xl">
			<h2 class="font-display mb-4 text-3xl font-bold md:text-4xl">
				Ready to Find Love?
			</h2>
			<p class="text-base-content/60 mb-8">
				Download PurrMeet today and give your cat the social life they
				deserve.
			</p>
			<div class="flex flex-col justify-center gap-4 sm:flex-row">
				<button
					class="bg-neutral text-neutral-content flex items-center justify-center gap-2 rounded-(--radius-field) px-6 py-3 font-semibold"
				>
					<span>🍎</span> App Store
				</button>
				<button
					class="bg-neutral text-neutral-content flex items-center justify-center gap-2 rounded-(--radius-field) px-6 py-3 font-semibold"
				>
					<span>▶️</span> Google Play
				</button>
			</div>
		</div>
	</section>

	<!-- Footer -->
	<footer class="bg-base-300 px-6 py-8">
		<div
			class="mx-auto flex max-w-5xl flex-col items-center justify-between gap-4 md:flex-row"
		>
			<div class="flex items-center gap-2">
				<span class="text-2xl">😻</span>
				<span class="text-primary font-display font-bold"
					>PurrMeet</span
				>
			</div>
			<div class="text-base-content/60 flex gap-6 text-sm">
				<a href="#" class="hover:text-primary transition-colors"
					>Privacy</a
				>
				<a href="#" class="hover:text-primary transition-colors"
					>Terms</a
				>
				<a href="#" class="hover:text-primary transition-colors"
					>Contact</a
				>
			</div>
			<p class="text-base-content/50 text-sm">
				Made with 💕 for cats everywhere
			</p>
		</div>
	</footer>
</div>
