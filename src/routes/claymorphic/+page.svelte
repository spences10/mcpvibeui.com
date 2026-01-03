<script lang="ts">
	let email = $state('');
</script>

<div class="min-h-screen bg-base-200 font-body">
	<!-- Nav -->
	<nav class="flex items-center justify-between px-8 py-6">
		<div class="flex items-center gap-2">
			<span class="text-4xl">🐱</span>
			<span class="font-display text-2xl font-bold text-base-content">PurrMatch</span>
		</div>
		<div class="flex gap-4">
			<button class="clay-sm px-6 py-3 font-medium text-base-content cursor-pointer">Log In</button>
			<button class="clay-btn px-6 py-3 font-medium text-primary-content cursor-pointer">Sign Up</button>
		</div>
	</nav>

	<!-- Hero -->
	<section class="px-8 py-20">
		<div class="mx-auto max-w-6xl flex flex-col lg:flex-row items-center gap-12">
			<div class="flex-1 space-y-8">
				<h1 class="font-display text-5xl lg:text-6xl font-bold text-base-content leading-tight">
					Find Your Cat's<br />
					<span class="text-primary">Purrfect Match</span>
				</h1>
				<p class="text-xl text-base-content/70 max-w-lg">
					The first dating app designed for cats. Help your feline find friendship, love, or just a playdate buddy.
				</p>
				<div class="flex flex-col sm:flex-row gap-4">
					<input
						bind:value={email}
						type="email"
						placeholder="Enter your email"
						class="clay-sm px-6 py-4 text-base-content placeholder:text-base-content/50 outline-none flex-1 max-w-sm"
					/>
					<button class="clay-btn px-8 py-4 font-semibold text-primary-content cursor-pointer">
						Get Started Free
					</button>
				</div>
				<p class="text-sm text-base-content/50">Join 50,000+ happy cat parents. No credit card required.</p>
			</div>
			<div class="flex-1 flex justify-center">
				<div class="clay p-8 relative">
					<div class="w-72 h-80 bg-base-300 rounded-2xl flex items-center justify-center text-8xl">
						😻
					</div>
					<div class="absolute -bottom-4 -right-4 clay-accent px-4 py-2 text-accent-content font-medium">
						98% Match!
					</div>
				</div>
			</div>
		</div>
	</section>

	<!-- Features -->
	<section class="px-8 py-20 bg-base-100">
		<div class="mx-auto max-w-6xl">
			<h2 class="font-display text-4xl font-bold text-center text-base-content mb-16">
				Why Cats Love Us
			</h2>
			<div class="grid md:grid-cols-3 gap-8">
				<div class="clay p-8 space-y-4">
					<div class="clay-secondary w-16 h-16 flex items-center justify-center text-3xl">🐾</div>
					<h3 class="font-display text-xl font-semibold text-base-content">Personality Matching</h3>
					<p class="text-base-content/70">Our AI analyzes your cat's personality to find compatible companions.</p>
				</div>
				<div class="clay p-8 space-y-4">
					<div class="clay-accent w-16 h-16 flex items-center justify-center text-3xl">📍</div>
					<h3 class="font-display text-xl font-semibold text-base-content">Local Connections</h3>
					<p class="text-base-content/70">Find feline friends in your neighborhood for easy meetups.</p>
				</div>
				<div class="clay p-8 space-y-4">
					<div class="clay-btn w-16 h-16 flex items-center justify-center text-3xl">💬</div>
					<h3 class="font-display text-xl font-semibold text-base-content">Safe Chat</h3>
					<p class="text-base-content/70">Message other cat parents in our moderated, pet-friendly environment.</p>
				</div>
			</div>
		</div>
	</section>

	<!-- How It Works -->
	<section class="px-8 py-20">
		<div class="mx-auto max-w-6xl">
			<h2 class="font-display text-4xl font-bold text-center text-base-content mb-16">
				How It Works
			</h2>
			<div class="grid md:grid-cols-4 gap-6">
				{#each [
					{ num: '1', icon: '📸', title: 'Create Profile', desc: 'Upload cute pics of your cat' },
					{ num: '2', icon: '🎯', title: 'Set Preferences', desc: 'Tell us what your cat likes' },
					{ num: '3', icon: '💕', title: 'Get Matches', desc: 'Swipe through compatible cats' },
					{ num: '4', icon: '🎉', title: 'Meet Up!', desc: 'Arrange playdates nearby' }
				] as step}
					<div class="clay-sm p-6 text-center space-y-3">
						<div class="clay-secondary w-12 h-12 mx-auto flex items-center justify-center font-display font-bold text-secondary-content">
							{step.num}
						</div>
						<span class="text-4xl block">{step.icon}</span>
						<h3 class="font-display font-semibold text-base-content">{step.title}</h3>
						<p class="text-sm text-base-content/70">{step.desc}</p>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- Testimonials -->
	<section class="px-8 py-20 bg-base-100">
		<div class="mx-auto max-w-6xl">
			<h2 class="font-display text-4xl font-bold text-center text-base-content mb-16">
				Happy Tails
			</h2>
			<div class="grid md:grid-cols-3 gap-8">
				{#each [
					{ name: 'Whiskers & Mittens', quote: 'They became best friends on their first playdate!', avatar: '🐈' },
					{ name: 'Sir Fluffington', quote: 'Finally found a cat who matches my energy level.', avatar: '🐈‍⬛' },
					{ name: 'Luna & Oliver', quote: 'Now they have sleepovers every weekend!', avatar: '😸' }
				] as testimonial}
					<div class="clay p-8 space-y-4">
						<div class="flex items-center gap-4">
							<div class="clay-sm w-14 h-14 flex items-center justify-center text-2xl">
								{testimonial.avatar}
							</div>
							<span class="font-display font-semibold text-base-content">{testimonial.name}</span>
						</div>
						<p class="text-base-content/70 italic">"{testimonial.quote}"</p>
						<div class="text-accent">★★★★★</div>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- CTA -->
	<section class="px-8 py-20">
		<div class="mx-auto max-w-3xl text-center">
			<div class="clay p-12 space-y-6">
				<span class="text-6xl">😺</span>
				<h2 class="font-display text-4xl font-bold text-base-content">
					Ready to Find Love?
				</h2>
				<p class="text-xl text-base-content/70">
					Your cat's soulmate is just a swipe away.
				</p>
				<button class="clay-btn px-10 py-4 font-semibold text-lg text-primary-content cursor-pointer">
					Download Free App
				</button>
				<div class="flex justify-center gap-8 pt-4">
					<div class="clay-sm px-4 py-2 text-sm text-base-content">🍎 App Store</div>
					<div class="clay-sm px-4 py-2 text-sm text-base-content">🤖 Play Store</div>
				</div>
			</div>
		</div>
	</section>

	<!-- Footer -->
	<footer class="px-8 py-12 bg-base-300">
		<div class="mx-auto max-w-6xl flex flex-col md:flex-row justify-between items-center gap-6">
			<div class="flex items-center gap-2">
				<span class="text-2xl">🐱</span>
				<span class="font-display font-bold text-base-content">PurrMatch</span>
			</div>
			<div class="flex gap-8 text-base-content/70">
				<a href="#" class="hover:text-base-content">About</a>
				<a href="#" class="hover:text-base-content">Privacy</a>
				<a href="#" class="hover:text-base-content">Terms</a>
				<a href="#" class="hover:text-base-content">Contact</a>
			</div>
			<p class="text-sm text-base-content/50">© 2026 PurrMatch. Made with 💕 for cats.</p>
		</div>
	</footer>
</div>
