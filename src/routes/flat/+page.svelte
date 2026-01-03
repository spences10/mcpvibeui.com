<script lang="ts">
	const features = [
		{
			icon: '🐱',
			title: 'Purrfect Matches',
			desc: 'AI-powered matching based on personality, breed preferences, and lifestyle'
		},
		{
			icon: '📍',
			title: 'Local Kitties',
			desc: 'Find feline friends in your neighborhood for playdates'
		},
		{
			icon: '💬',
			title: 'Cat Chat',
			desc: 'Message other cat parents and arrange meetups'
		},
		{
			icon: '📸',
			title: 'Photo Albums',
			desc: 'Share unlimited photos of your adorable fur babies'
		}
	];

	const testimonials = [
		{
			name: 'Whiskers & Luna',
			text: 'Found my cat her best friend! They nap together every day now.',
			avatar: '😺'
		},
		{
			name: 'Mr. Fluffington',
			text: 'Finally a dating app that understands cats are the priority.',
			avatar: '😸'
		},
		{
			name: 'Shadow & Mittens',
			text: 'Our cats fell in love at first sniff. Wedding bells soon!',
			avatar: '😻'
		}
	];
</script>

<div class="min-h-screen">
	<!-- Nav -->
	<nav class="flex items-center justify-between px-6 py-4 bg-base-100">
		<div class="flex items-center gap-2">
			<span class="text-3xl">😻</span>
			<span class="font-[family-name:var(--font-display)] text-xl font-bold text-primary"
				>PurrMeet</span
			>
		</div>
		<div class="flex items-center gap-4">
			<a href="#features" class="text-base-content/70 hover:text-primary transition-colors"
				>Features</a
			>
			<a href="#testimonials" class="text-base-content/70 hover:text-primary transition-colors"
				>Stories</a
			>
			<button
				class="bg-primary text-primary-content px-4 py-2 rounded-[var(--radius-field)] font-semibold hover:opacity-90 transition-opacity"
			>
				Get Started
			</button>
		</div>
	</nav>

	<!-- Hero -->
	<section class="px-6 py-20 text-center bg-base-200">
		<div class="max-w-3xl mx-auto">
			<h1
				class="font-[family-name:var(--font-display)] text-5xl md:text-6xl font-bold text-base-content mb-6"
			>
				Find Your Cat's <span class="text-primary">Soulmate</span>
			</h1>
			<p class="text-xl text-base-content/70 mb-8 max-w-xl mx-auto">
				The #1 dating app for cats and their humans. Swipe right on love, friendship, and endless
				cuddle puddles.
			</p>
			<div class="flex flex-col sm:flex-row gap-4 justify-center">
				<button
					class="bg-primary text-primary-content px-8 py-3 rounded-[var(--radius-field)] font-semibold text-lg hover:opacity-90 transition-opacity"
				>
					Download Free
				</button>
				<button
					class="bg-base-300 text-base-content px-8 py-3 rounded-[var(--radius-field)] font-semibold text-lg hover:bg-base-300/80 transition-colors"
				>
					Learn More
				</button>
			</div>
			<p class="mt-6 text-sm text-base-content/50">
				Join 50,000+ happy cats and their humans
			</p>
		</div>

		<!-- Hero illustration -->
		<div class="mt-16 flex justify-center gap-8 text-8xl">
			<span class="animate-bounce" style="animation-delay: 0ms;">🐱</span>
			<span class="text-6xl self-center text-secondary">💕</span>
			<span class="animate-bounce" style="animation-delay: 200ms;">😺</span>
		</div>
	</section>

	<!-- Features -->
	<section id="features" class="px-6 py-20 bg-base-100">
		<div class="max-w-5xl mx-auto">
			<h2
				class="font-[family-name:var(--font-display)] text-3xl md:text-4xl font-bold text-center mb-4"
			>
				Why Cats Love Us
			</h2>
			<p class="text-center text-base-content/60 mb-12 max-w-xl mx-auto">
				Everything your feline friend needs to find their purrfect match
			</p>

			<div class="grid md:grid-cols-2 lg:grid-cols-4 gap-6">
				{#each features as feature}
					<div class="bg-base-200 p-6 rounded-[var(--radius-box)]">
						<div class="text-4xl mb-4">{feature.icon}</div>
						<h3 class="font-[family-name:var(--font-display)] font-semibold text-lg mb-2">
							{feature.title}
						</h3>
						<p class="text-base-content/60 text-sm">{feature.desc}</p>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- Stats -->
	<section class="px-6 py-16 bg-primary text-primary-content">
		<div class="max-w-4xl mx-auto grid grid-cols-2 md:grid-cols-4 gap-8 text-center">
			<div>
				<div class="font-[family-name:var(--font-display)] text-4xl font-bold">50K+</div>
				<div class="text-primary-content/70 text-sm mt-1">Happy Cats</div>
			</div>
			<div>
				<div class="font-[family-name:var(--font-display)] text-4xl font-bold">12K</div>
				<div class="text-primary-content/70 text-sm mt-1">Matches Made</div>
			</div>
			<div>
				<div class="font-[family-name:var(--font-display)] text-4xl font-bold">98%</div>
				<div class="text-primary-content/70 text-sm mt-1">Purr Rate</div>
			</div>
			<div>
				<div class="font-[family-name:var(--font-display)] text-4xl font-bold">4.9</div>
				<div class="text-primary-content/70 text-sm mt-1">App Rating</div>
			</div>
		</div>
	</section>

	<!-- Testimonials -->
	<section id="testimonials" class="px-6 py-20 bg-base-200">
		<div class="max-w-5xl mx-auto">
			<h2
				class="font-[family-name:var(--font-display)] text-3xl md:text-4xl font-bold text-center mb-12"
			>
				Love Stories
			</h2>

			<div class="grid md:grid-cols-3 gap-6">
				{#each testimonials as t}
					<div class="bg-base-100 p-6 rounded-[var(--radius-box)]">
						<div class="text-5xl mb-4">{t.avatar}</div>
						<p class="text-base-content/70 mb-4 italic">"{t.text}"</p>
						<p class="font-semibold text-sm">{t.name}</p>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- CTA -->
	<section class="px-6 py-20 bg-base-100 text-center">
		<div class="max-w-2xl mx-auto">
			<h2
				class="font-[family-name:var(--font-display)] text-3xl md:text-4xl font-bold mb-4"
			>
				Ready to Find Love?
			</h2>
			<p class="text-base-content/60 mb-8">
				Download PurrMeet today and give your cat the social life they deserve.
			</p>
			<div class="flex flex-col sm:flex-row gap-4 justify-center">
				<button
					class="bg-neutral text-neutral-content px-6 py-3 rounded-[var(--radius-field)] font-semibold flex items-center justify-center gap-2"
				>
					<span>🍎</span> App Store
				</button>
				<button
					class="bg-neutral text-neutral-content px-6 py-3 rounded-[var(--radius-field)] font-semibold flex items-center justify-center gap-2"
				>
					<span>▶️</span> Google Play
				</button>
			</div>
		</div>
	</section>

	<!-- Footer -->
	<footer class="px-6 py-8 bg-base-300">
		<div class="max-w-5xl mx-auto flex flex-col md:flex-row justify-between items-center gap-4">
			<div class="flex items-center gap-2">
				<span class="text-2xl">😻</span>
				<span class="font-[family-name:var(--font-display)] font-bold text-primary">PurrMeet</span>
			</div>
			<div class="flex gap-6 text-sm text-base-content/60">
				<a href="#" class="hover:text-primary transition-colors">Privacy</a>
				<a href="#" class="hover:text-primary transition-colors">Terms</a>
				<a href="#" class="hover:text-primary transition-colors">Contact</a>
			</div>
			<p class="text-sm text-base-content/50">Made with 💕 for cats everywhere</p>
		</div>
	</footer>
</div>
