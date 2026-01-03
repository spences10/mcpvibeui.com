<script lang="ts">
	let email = $state('');
</script>

<svelte:head>
	<title>Purrfect Match | Where Cats Find Love</title>
</svelte:head>

<div class="min-h-screen">
	<!-- Header -->
	<header class="border-b border-base-300">
		<nav class="max-w-6xl mx-auto px-6 py-4 flex items-center justify-between">
			<div class="font-display text-2xl font-semibold tracking-tight">Purrfect Match</div>
			<div class="flex items-center gap-8 text-sm">
				<a href="#stories" class="hover:text-primary transition-colors">Stories</a>
				<a href="#how" class="hover:text-primary transition-colors">How It Works</a>
				<a href="#testimonials" class="hover:text-primary transition-colors">Testimonials</a>
				<button class="bg-primary text-primary-content px-4 py-2 rounded-[var(--radius-field)] font-medium hover:opacity-90 transition-opacity">
					Join Waitlist
				</button>
			</div>
		</nav>
	</header>

	<!-- Hero -->
	<section class="max-w-6xl mx-auto px-6 py-20 grid grid-cols-12 gap-8">
		<div class="col-span-7">
			<p class="text-sm uppercase tracking-[0.2em] text-secondary mb-4">The New Standard in Feline Companionship</p>
			<h1 class="text-6xl font-display leading-[1.1] mb-6">
				Every Cat Deserves<br/>
				<em class="italic">a Soulmate</em>
			</h1>
			<p class="text-lg text-base-content/70 leading-relaxed max-w-xl mb-8">
				Purrfect Match connects discerning cats with compatible companions through our proprietary
				personality assessment. Because finding the right friend shouldn't be left to chance.
			</p>
			<div class="flex gap-4">
				<input
					type="email"
					bind:value={email}
					placeholder="Enter your email"
					class="px-4 py-3 border border-base-300 rounded-[var(--radius-field)] w-64 bg-base-100 focus:outline-none focus:border-primary"
				/>
				<button class="bg-neutral text-neutral-content px-6 py-3 rounded-[var(--radius-field)] font-medium hover:opacity-90 transition-opacity">
					Get Early Access
				</button>
			</div>
		</div>
		<div class="col-span-5 flex items-center justify-center">
			<div class="w-80 h-96 bg-base-200 rounded-[var(--radius-box)] flex items-center justify-center border border-base-300">
				<span class="text-8xl">🐱</span>
			</div>
		</div>
	</section>

	<!-- Stats Bar -->
	<section class="border-y border-base-300 bg-base-200">
		<div class="max-w-6xl mx-auto px-6 py-8 grid grid-cols-4 gap-8">
			<div class="text-center">
				<div class="font-display text-4xl font-semibold">12,847</div>
				<div class="text-sm text-base-content/60 mt-1">Cats Matched</div>
			</div>
			<div class="text-center">
				<div class="font-display text-4xl font-semibold">94%</div>
				<div class="text-sm text-base-content/60 mt-1">Compatibility Rate</div>
			</div>
			<div class="text-center">
				<div class="font-display text-4xl font-semibold">47</div>
				<div class="text-sm text-base-content/60 mt-1">Countries</div>
			</div>
			<div class="text-center">
				<div class="font-display text-4xl font-semibold">4.9</div>
				<div class="text-sm text-base-content/60 mt-1">Owner Rating</div>
			</div>
		</div>
	</section>

	<!-- Featured Story -->
	<section id="stories" class="max-w-6xl mx-auto px-6 py-20">
		<div class="grid grid-cols-12 gap-12">
			<div class="col-span-5">
				<div class="w-full aspect-[4/5] bg-base-200 rounded-[var(--radius-box)] flex items-center justify-center border border-base-300">
					<span class="text-9xl">😻</span>
				</div>
			</div>
			<div class="col-span-7 flex flex-col justify-center">
				<p class="text-sm uppercase tracking-[0.2em] text-secondary mb-4">Featured Love Story</p>
				<h2 class="text-4xl font-display leading-tight mb-6">
					"Whiskers and Mittens:<br/>A Tale of Two Tails"
				</h2>
				<p class="text-base-content/70 leading-relaxed mb-6">
					When Whiskers, a refined British Shorthair from Manhattan, matched with Mittens,
					an adventurous tabby from Brooklyn, neither expected to find their perfect companion.
					But our algorithm saw what they couldn't—two souls meant to share a sunbeam.
				</p>
				<p class="text-base-content/70 leading-relaxed mb-8">
					"I never thought I'd find a cat who understands my need for both quiet contemplation
					and spontaneous 3 AM zoomies," says Whiskers' owner, Sarah. "Purrfect Match understood
					what we were looking for before we did."
				</p>
				<a href="#" class="text-primary font-medium hover:underline">Read their full story →</a>
			</div>
		</div>
	</section>

	<!-- How It Works -->
	<section id="how" class="border-y border-base-300 bg-base-200">
		<div class="max-w-6xl mx-auto px-6 py-20">
			<div class="text-center mb-16">
				<p class="text-sm uppercase tracking-[0.2em] text-secondary mb-4">The Process</p>
				<h2 class="text-4xl font-display">How Purrfect Match Works</h2>
			</div>
			<div class="grid grid-cols-3 gap-12">
				<div>
					<div class="font-display text-6xl text-base-300 mb-4">01</div>
					<h3 class="font-display text-xl mb-3">Personality Assessment</h3>
					<p class="text-base-content/70 leading-relaxed">
						Complete our comprehensive 47-point feline personality quiz. We analyze everything
						from nap preferences to prey drive.
					</p>
				</div>
				<div>
					<div class="font-display text-6xl text-base-300 mb-4">02</div>
					<h3 class="font-display text-xl mb-3">Algorithm Matching</h3>
					<p class="text-base-content/70 leading-relaxed">
						Our proprietary algorithm considers temperament, energy levels, and even preferred
						window-watching schedules.
					</p>
				</div>
				<div>
					<div class="font-display text-6xl text-base-300 mb-4">03</div>
					<h3 class="font-display text-xl mb-3">Supervised Introduction</h3>
					<p class="text-base-content/70 leading-relaxed">
						Arrange a chaperoned meetup at one of our partner cat cafés. First sniff is
						always complimentary.
					</p>
				</div>
			</div>
		</div>
	</section>

	<!-- Testimonials -->
	<section id="testimonials" class="max-w-6xl mx-auto px-6 py-20">
		<div class="text-center mb-16">
			<p class="text-sm uppercase tracking-[0.2em] text-secondary mb-4">What Cat Parents Say</p>
			<h2 class="text-4xl font-display">Testimonials</h2>
		</div>
		<div class="grid grid-cols-2 gap-8">
			<div class="p-8 border border-base-300 rounded-[var(--radius-box)]">
				<p class="text-lg leading-relaxed mb-6 italic">
					"Mr. Fluffington had been an only cat for seven years. I thought he'd never accept
					another feline. Purrfect Match found him Princess Whiskerface, and now they groom
					each other daily."
				</p>
				<div class="flex items-center gap-4">
					<div class="w-12 h-12 bg-base-200 rounded-full flex items-center justify-center">🐈</div>
					<div>
						<div class="font-medium">Mr. Fluffington's Human</div>
						<div class="text-sm text-base-content/60">Portland, OR</div>
					</div>
				</div>
			</div>
			<div class="p-8 border border-base-300 rounded-[var(--radius-box)]">
				<p class="text-lg leading-relaxed mb-6 italic">
					"As a Bengal owner, I knew I needed another high-energy cat. The algorithm matched
					Ziggy with an Abyssinian named Rocket, and now my living room is a perpetual circus.
					Exactly what we wanted."
				</p>
				<div class="flex items-center gap-4">
					<div class="w-12 h-12 bg-base-200 rounded-full flex items-center justify-center">🐆</div>
					<div>
						<div class="font-medium">Ziggy & Rocket's Family</div>
						<div class="text-sm text-base-content/60">Austin, TX</div>
					</div>
				</div>
			</div>
		</div>
	</section>

	<!-- Editorial Quote -->
	<section class="border-y border-base-300">
		<div class="max-w-4xl mx-auto px-6 py-20 text-center">
			<blockquote class="font-display text-3xl leading-relaxed italic mb-6">
				"In an age of endless swipes and shallow connections, Purrfect Match reminds us that
				meaningful companionship—even for our feline friends—requires patience, understanding,
				and a little algorithmic magic."
			</blockquote>
			<cite class="text-sm uppercase tracking-[0.2em] text-base-content/60">
				— The Feline Quarterly
			</cite>
		</div>
	</section>

	<!-- CTA -->
	<section class="max-w-6xl mx-auto px-6 py-20">
		<div class="bg-neutral text-neutral-content rounded-[var(--radius-box)] p-16 text-center">
			<h2 class="font-display text-4xl mb-4">Find Your Cat's Perfect Match</h2>
			<p class="text-neutral-content/80 mb-8 max-w-xl mx-auto">
				Join 50,000+ cat parents on our waitlist. Early members receive lifetime premium access.
			</p>
			<div class="flex justify-center gap-4">
				<input
					type="email"
					placeholder="Enter your email"
					class="px-4 py-3 rounded-[var(--radius-field)] w-64 bg-neutral-content text-neutral focus:outline-none"
				/>
				<button class="bg-primary text-primary-content px-6 py-3 rounded-[var(--radius-field)] font-medium hover:opacity-90 transition-opacity">
					Join Waitlist
				</button>
			</div>
		</div>
	</section>

	<!-- Footer -->
	<footer class="border-t border-base-300">
		<div class="max-w-6xl mx-auto px-6 py-12">
			<div class="grid grid-cols-4 gap-8 mb-12">
				<div>
					<div class="font-display text-xl font-semibold mb-4">Purrfect Match</div>
					<p class="text-sm text-base-content/60 leading-relaxed">
						Connecting cats with compatible companions since 2024.
					</p>
				</div>
				<div>
					<div class="font-medium mb-4">Product</div>
					<ul class="space-y-2 text-sm text-base-content/60">
						<li><a href="#" class="hover:text-primary">How It Works</a></li>
						<li><a href="#" class="hover:text-primary">Pricing</a></li>
						<li><a href="#" class="hover:text-primary">Success Stories</a></li>
						<li><a href="#" class="hover:text-primary">Cat Cafés</a></li>
					</ul>
				</div>
				<div>
					<div class="font-medium mb-4">Company</div>
					<ul class="space-y-2 text-sm text-base-content/60">
						<li><a href="#" class="hover:text-primary">About</a></li>
						<li><a href="#" class="hover:text-primary">Blog</a></li>
						<li><a href="#" class="hover:text-primary">Careers</a></li>
						<li><a href="#" class="hover:text-primary">Press</a></li>
					</ul>
				</div>
				<div>
					<div class="font-medium mb-4">Legal</div>
					<ul class="space-y-2 text-sm text-base-content/60">
						<li><a href="#" class="hover:text-primary">Privacy</a></li>
						<li><a href="#" class="hover:text-primary">Terms</a></li>
						<li><a href="#" class="hover:text-primary">Cat Safety</a></li>
					</ul>
				</div>
			</div>
			<div class="border-t border-base-300 pt-8 text-sm text-base-content/60 text-center">
				© 2024 Purrfect Match. All rights reserved. Made with 😺 for cats everywhere.
			</div>
		</div>
	</footer>
</div>
