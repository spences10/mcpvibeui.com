<script lang="ts">
	let email = $state('');
</script>

<div class="bg-base-200 font-body min-h-screen">
	<!-- Nav -->
	<nav class="flex items-center justify-between px-8 py-6">
		<div class="flex items-center gap-2">
			<span class="text-4xl">🐱</span>
			<span class="font-display text-base-content text-2xl font-bold">
				PurrMatch
			</span>
		</div>
		<div class="flex gap-4">
			<button
				class="clay-sm text-base-content cursor-pointer px-6 py-3 font-medium"
			>
				Log In
			</button>
			<button
				class="clay-btn text-primary-content cursor-pointer px-6 py-3 font-medium"
			>
				Sign Up
			</button>
		</div>
	</nav>

	<!-- Hero -->
	<section class="px-8 py-20">
		<div
			class="mx-auto flex max-w-6xl flex-col items-center gap-12 lg:flex-row"
		>
			<div class="flex-1 space-y-8">
				<h1
					class="font-display text-base-content text-5xl leading-tight font-bold lg:text-6xl"
				>
					Find Your Cat's<br />
					<span class="text-primary">Purrfect Match</span>
				</h1>
				<p class="text-base-content/70 max-w-lg text-xl">
					The first dating app designed for cats. Help your feline
					find friendship, love, or just a playdate buddy.
				</p>
				<div class="flex flex-col gap-4 sm:flex-row">
					<input
						bind:value={email}
						type="email"
						placeholder="Enter your email"
						class="clay-sm text-base-content placeholder:text-base-content/50 max-w-sm flex-1 px-6 py-4 outline-none"
					/>
					<button
						class="clay-btn text-primary-content cursor-pointer px-8 py-4 font-semibold"
					>
						Get Started Free
					</button>
				</div>
				<p class="text-base-content/50 text-sm">
					Join 50,000+ happy cat parents. No credit card required.
				</p>
			</div>
			<div class="flex flex-1 justify-center">
				<div class="clay relative p-8">
					<div
						class="bg-base-300 flex h-80 w-72 items-center justify-center rounded-2xl text-8xl"
					>
						😻
					</div>
					<div
						class="clay-accent text-accent-content absolute -right-4 -bottom-4 px-4 py-2 font-medium"
					>
						98% Match!
					</div>
				</div>
			</div>
		</div>
	</section>

	<!-- Features -->
	<section class="bg-base-100 px-8 py-20">
		<div class="mx-auto max-w-6xl">
			<h2
				class="font-display text-base-content mb-16 text-center text-4xl font-bold"
			>
				Why Cats Love Us
			</h2>
			<div class="grid gap-8 md:grid-cols-3">
				<div class="clay space-y-4 p-8">
					<div
						class="clay-secondary flex h-16 w-16 items-center justify-center text-3xl"
					>
						🐾
					</div>
					<h3
						class="font-display text-base-content text-xl font-semibold"
					>
						Personality Matching
					</h3>
					<p class="text-base-content/70">
						Our AI analyzes your cat's personality to find compatible
						companions.
					</p>
				</div>
				<div class="clay space-y-4 p-8">
					<div
						class="clay-accent flex h-16 w-16 items-center justify-center text-3xl"
					>
						📍
					</div>
					<h3
						class="font-display text-base-content text-xl font-semibold"
					>
						Local Connections
					</h3>
					<p class="text-base-content/70">
						Find feline friends in your neighborhood for easy meetups.
					</p>
				</div>
				<div class="clay space-y-4 p-8">
					<div
						class="clay-btn flex h-16 w-16 items-center justify-center text-3xl"
					>
						💬
					</div>
					<h3
						class="font-display text-base-content text-xl font-semibold"
					>
						Safe Chat
					</h3>
					<p class="text-base-content/70">
						Message other cat parents in our moderated, pet-friendly
						environment.
					</p>
				</div>
			</div>
		</div>
	</section>

	<!-- How It Works -->
	<section class="px-8 py-20">
		<div class="mx-auto max-w-6xl">
			<h2
				class="font-display text-base-content mb-16 text-center text-4xl font-bold"
			>
				How It Works
			</h2>
			<div class="grid gap-6 md:grid-cols-4">
				{#each [{ num: '1', icon: '📸', title: 'Create Profile', desc: 'Upload cute pics of your cat' }, { num: '2', icon: '🎯', title: 'Set Preferences', desc: 'Tell us what your cat likes' }, { num: '3', icon: '💕', title: 'Get Matches', desc: 'Swipe through compatible cats' }, { num: '4', icon: '🎉', title: 'Meet Up!', desc: 'Arrange playdates nearby' }] as step}
					<div class="clay-sm space-y-3 p-6 text-center">
						<div
							class="clay-secondary font-display text-secondary-content mx-auto flex h-12 w-12 items-center justify-center font-bold"
						>
							{step.num}
						</div>
						<span class="block text-4xl">{step.icon}</span>
						<h3 class="font-display text-base-content font-semibold">
							{step.title}
						</h3>
						<p class="text-base-content/70 text-sm">{step.desc}</p>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- Testimonials -->
	<section class="bg-base-100 px-8 py-20">
		<div class="mx-auto max-w-6xl">
			<h2
				class="font-display text-base-content mb-16 text-center text-4xl font-bold"
			>
				Happy Tails
			</h2>
			<div class="grid gap-8 md:grid-cols-3">
				{#each [{ name: 'Whiskers & Mittens', quote: 'They became best friends on their first playdate!', avatar: '🐈' }, { name: 'Sir Fluffington', quote: 'Finally found a cat who matches my energy level.', avatar: '🐈‍⬛' }, { name: 'Luna & Oliver', quote: 'Now they have sleepovers every weekend!', avatar: '😸' }] as testimonial}
					<div class="clay space-y-4 p-8">
						<div class="flex items-center gap-4">
							<div
								class="clay-sm flex h-14 w-14 items-center justify-center text-2xl"
							>
								{testimonial.avatar}
							</div>
							<span
								class="font-display text-base-content font-semibold"
								>{testimonial.name}</span
							>
						</div>
						<p class="text-base-content/70 italic">
							"{testimonial.quote}"
						</p>
						<div class="text-accent">★★★★★</div>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- CTA -->
	<section class="px-8 py-20">
		<div class="mx-auto max-w-3xl text-center">
			<div class="clay space-y-6 p-12">
				<span class="text-6xl">😺</span>
				<h2 class="font-display text-base-content text-4xl font-bold">
					Ready to Find Love?
				</h2>
				<p class="text-base-content/70 text-xl">
					Your cat's soulmate is just a swipe away.
				</p>
				<button
					class="clay-btn text-primary-content cursor-pointer px-10 py-4 text-lg font-semibold"
				>
					Download Free App
				</button>
				<div class="flex justify-center gap-8 pt-4">
					<div class="clay-sm text-base-content px-4 py-2 text-sm">
						🍎 App Store
					</div>
					<div class="clay-sm text-base-content px-4 py-2 text-sm">
						🤖 Play Store
					</div>
				</div>
			</div>
		</div>
	</section>

	<!-- Footer -->
	<footer class="bg-base-300 px-8 py-12">
		<div
			class="mx-auto flex max-w-6xl flex-col items-center justify-between gap-6 md:flex-row"
		>
			<div class="flex items-center gap-2">
				<span class="text-2xl">🐱</span>
				<span class="font-display text-base-content font-bold"
					>PurrMatch</span
				>
			</div>
			<div class="text-base-content/70 flex gap-8">
				<a href="#" class="hover:text-base-content">About</a>
				<a href="#" class="hover:text-base-content">Privacy</a>
				<a href="#" class="hover:text-base-content">Terms</a>
				<a href="#" class="hover:text-base-content">Contact</a>
			</div>
			<p class="text-base-content/50 text-sm">
				© 2026 PurrMatch. Made with 💕 for cats.
			</p>
		</div>
	</footer>
</div>
