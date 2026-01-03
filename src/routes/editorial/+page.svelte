<script lang="ts">
	let email = $state('');
</script>

<svelte:head>
	<title>Purrfect Match | Where Cats Find Love</title>
</svelte:head>

<div class="min-h-screen">
	<!-- Header -->
	<header class="border-base-300 border-b">
		<nav
			class="mx-auto flex max-w-6xl items-center justify-between px-6 py-4"
		>
			<div class="font-display text-2xl font-semibold tracking-tight">
				Purrfect Match
			</div>
			<div class="flex items-center gap-8 text-sm">
				<a
					href="#stories"
					class="hover:text-primary transition-colors">Stories</a
				>
				<a href="#how" class="hover:text-primary transition-colors"
					>How It Works</a
				>
				<a
					href="#testimonials"
					class="hover:text-primary transition-colors">Testimonials</a
				>
				<button
					class="bg-primary text-primary-content rounded-(--radius-field) px-4 py-2 font-medium transition-opacity hover:opacity-90"
				>
					Join Waitlist
				</button>
			</div>
		</nav>
	</header>

	<!-- Hero -->
	<section
		class="mx-auto grid max-w-6xl grid-cols-12 gap-8 px-6 py-20"
	>
		<div class="col-span-7">
			<p
				class="text-secondary mb-4 text-sm tracking-[0.2em] uppercase"
			>
				The New Standard in Feline Companionship
			</p>
			<h1 class="font-display mb-6 text-6xl leading-[1.1]">
				Every Cat Deserves<br />
				<em class="italic">a Soulmate</em>
			</h1>
			<p
				class="text-base-content/70 mb-8 max-w-xl text-lg leading-relaxed"
			>
				Purrfect Match connects discerning cats with compatible
				companions through our proprietary personality assessment.
				Because finding the right friend shouldn't be left to chance.
			</p>
			<div class="flex gap-4">
				<input
					type="email"
					bind:value={email}
					placeholder="Enter your email"
					class="border-base-300 bg-base-100 focus:border-primary w-64 rounded-(--radius-field) border px-4 py-3 focus:outline-none"
				/>
				<button
					class="bg-neutral text-neutral-content rounded-(--radius-field) px-6 py-3 font-medium transition-opacity hover:opacity-90"
				>
					Get Early Access
				</button>
			</div>
		</div>
		<div class="col-span-5 flex items-center justify-center">
			<div
				class="bg-base-200 border-base-300 flex h-96 w-80 items-center justify-center rounded-(--radius-box) border"
			>
				<span class="text-8xl">🐱</span>
			</div>
		</div>
	</section>

	<!-- Stats Bar -->
	<section class="border-base-300 bg-base-200 border-y">
		<div class="mx-auto grid max-w-6xl grid-cols-4 gap-8 px-6 py-8">
			<div class="text-center">
				<div class="font-display text-4xl font-semibold">12,847</div>
				<div class="text-base-content/60 mt-1 text-sm">
					Cats Matched
				</div>
			</div>
			<div class="text-center">
				<div class="font-display text-4xl font-semibold">94%</div>
				<div class="text-base-content/60 mt-1 text-sm">
					Compatibility Rate
				</div>
			</div>
			<div class="text-center">
				<div class="font-display text-4xl font-semibold">47</div>
				<div class="text-base-content/60 mt-1 text-sm">Countries</div>
			</div>
			<div class="text-center">
				<div class="font-display text-4xl font-semibold">4.9</div>
				<div class="text-base-content/60 mt-1 text-sm">
					Owner Rating
				</div>
			</div>
		</div>
	</section>

	<!-- Featured Story -->
	<section id="stories" class="mx-auto max-w-6xl px-6 py-20">
		<div class="grid grid-cols-12 gap-12">
			<div class="col-span-5">
				<div
					class="bg-base-200 border-base-300 flex aspect-4/5 w-full items-center justify-center rounded-(--radius-box) border"
				>
					<span class="text-9xl">😻</span>
				</div>
			</div>
			<div class="col-span-7 flex flex-col justify-center">
				<p
					class="text-secondary mb-4 text-sm tracking-[0.2em] uppercase"
				>
					Featured Love Story
				</p>
				<h2 class="font-display mb-6 text-4xl leading-tight">
					"Whiskers and Mittens:<br />A Tale of Two Tails"
				</h2>
				<p class="text-base-content/70 mb-6 leading-relaxed">
					When Whiskers, a refined British Shorthair from Manhattan,
					matched with Mittens, an adventurous tabby from Brooklyn,
					neither expected to find their perfect companion. But our
					algorithm saw what they couldn't—two souls meant to share a
					sunbeam.
				</p>
				<p class="text-base-content/70 mb-8 leading-relaxed">
					"I never thought I'd find a cat who understands my need for
					both quiet contemplation and spontaneous 3 AM zoomies," says
					Whiskers' owner, Sarah. "Purrfect Match understood what we
					were looking for before we did."
				</p>
				<a href="#" class="text-primary font-medium hover:underline"
					>Read their full story →</a
				>
			</div>
		</div>
	</section>

	<!-- How It Works -->
	<section id="how" class="border-base-300 bg-base-200 border-y">
		<div class="mx-auto max-w-6xl px-6 py-20">
			<div class="mb-16 text-center">
				<p
					class="text-secondary mb-4 text-sm tracking-[0.2em] uppercase"
				>
					The Process
				</p>
				<h2 class="font-display text-4xl">
					How Purrfect Match Works
				</h2>
			</div>
			<div class="grid grid-cols-3 gap-12">
				<div>
					<div class="font-display text-base-300 mb-4 text-6xl">
						01
					</div>
					<h3 class="font-display mb-3 text-xl">
						Personality Assessment
					</h3>
					<p class="text-base-content/70 leading-relaxed">
						Complete our comprehensive 47-point feline personality
						quiz. We analyze everything from nap preferences to prey
						drive.
					</p>
				</div>
				<div>
					<div class="font-display text-base-300 mb-4 text-6xl">
						02
					</div>
					<h3 class="font-display mb-3 text-xl">
						Algorithm Matching
					</h3>
					<p class="text-base-content/70 leading-relaxed">
						Our proprietary algorithm considers temperament, energy
						levels, and even preferred window-watching schedules.
					</p>
				</div>
				<div>
					<div class="font-display text-base-300 mb-4 text-6xl">
						03
					</div>
					<h3 class="font-display mb-3 text-xl">
						Supervised Introduction
					</h3>
					<p class="text-base-content/70 leading-relaxed">
						Arrange a chaperoned meetup at one of our partner cat
						cafés. First sniff is always complimentary.
					</p>
				</div>
			</div>
		</div>
	</section>

	<!-- Testimonials -->
	<section id="testimonials" class="mx-auto max-w-6xl px-6 py-20">
		<div class="mb-16 text-center">
			<p
				class="text-secondary mb-4 text-sm tracking-[0.2em] uppercase"
			>
				What Cat Parents Say
			</p>
			<h2 class="font-display text-4xl">Testimonials</h2>
		</div>
		<div class="grid grid-cols-2 gap-8">
			<div class="border-base-300 rounded-(--radius-box) border p-8">
				<p class="mb-6 text-lg leading-relaxed italic">
					"Mr. Fluffington had been an only cat for seven years. I
					thought he'd never accept another feline. Purrfect Match
					found him Princess Whiskerface, and now they groom each
					other daily."
				</p>
				<div class="flex items-center gap-4">
					<div
						class="bg-base-200 flex h-12 w-12 items-center justify-center rounded-full"
					>
						🐈
					</div>
					<div>
						<div class="font-medium">Mr. Fluffington's Human</div>
						<div class="text-base-content/60 text-sm">
							Portland, OR
						</div>
					</div>
				</div>
			</div>
			<div class="border-base-300 rounded-(--radius-box) border p-8">
				<p class="mb-6 text-lg leading-relaxed italic">
					"As a Bengal owner, I knew I needed another high-energy cat.
					The algorithm matched Ziggy with an Abyssinian named Rocket,
					and now my living room is a perpetual circus. Exactly what
					we wanted."
				</p>
				<div class="flex items-center gap-4">
					<div
						class="bg-base-200 flex h-12 w-12 items-center justify-center rounded-full"
					>
						🐆
					</div>
					<div>
						<div class="font-medium">Ziggy & Rocket's Family</div>
						<div class="text-base-content/60 text-sm">Austin, TX</div>
					</div>
				</div>
			</div>
		</div>
	</section>

	<!-- Editorial Quote -->
	<section class="border-base-300 border-y">
		<div class="mx-auto max-w-4xl px-6 py-20 text-center">
			<blockquote
				class="font-display mb-6 text-3xl leading-relaxed italic"
			>
				"In an age of endless swipes and shallow connections, Purrfect
				Match reminds us that meaningful companionship—even for our
				feline friends—requires patience, understanding, and a little
				algorithmic magic."
			</blockquote>
			<cite
				class="text-base-content/60 text-sm tracking-[0.2em] uppercase"
			>
				— The Feline Quarterly
			</cite>
		</div>
	</section>

	<!-- CTA -->
	<section class="mx-auto max-w-6xl px-6 py-20">
		<div
			class="bg-neutral text-neutral-content rounded-(--radius-box) p-16 text-center"
		>
			<h2 class="font-display mb-4 text-4xl">
				Find Your Cat's Perfect Match
			</h2>
			<p class="text-neutral-content/80 mx-auto mb-8 max-w-xl">
				Join 50,000+ cat parents on our waitlist. Early members
				receive lifetime premium access.
			</p>
			<div class="flex justify-center gap-4">
				<input
					type="email"
					placeholder="Enter your email"
					class="bg-neutral-content text-neutral w-64 rounded-(--radius-field) px-4 py-3 focus:outline-none"
				/>
				<button
					class="bg-primary text-primary-content rounded-(--radius-field) px-6 py-3 font-medium transition-opacity hover:opacity-90"
				>
					Join Waitlist
				</button>
			</div>
		</div>
	</section>

	<!-- Footer -->
	<footer class="border-base-300 border-t">
		<div class="mx-auto max-w-6xl px-6 py-12">
			<div class="mb-12 grid grid-cols-4 gap-8">
				<div>
					<div class="font-display mb-4 text-xl font-semibold">
						Purrfect Match
					</div>
					<p class="text-base-content/60 text-sm leading-relaxed">
						Connecting cats with compatible companions since 2024.
					</p>
				</div>
				<div>
					<div class="mb-4 font-medium">Product</div>
					<ul class="text-base-content/60 space-y-2 text-sm">
						<li>
							<a href="#" class="hover:text-primary">How It Works</a>
						</li>
						<li>
							<a href="#" class="hover:text-primary">Pricing</a>
						</li>
						<li>
							<a href="#" class="hover:text-primary"
								>Success Stories</a
							>
						</li>
						<li>
							<a href="#" class="hover:text-primary">Cat Cafés</a>
						</li>
					</ul>
				</div>
				<div>
					<div class="mb-4 font-medium">Company</div>
					<ul class="text-base-content/60 space-y-2 text-sm">
						<li><a href="#" class="hover:text-primary">About</a></li>
						<li><a href="#" class="hover:text-primary">Blog</a></li>
						<li>
							<a href="#" class="hover:text-primary">Careers</a>
						</li>
						<li><a href="#" class="hover:text-primary">Press</a></li>
					</ul>
				</div>
				<div>
					<div class="mb-4 font-medium">Legal</div>
					<ul class="text-base-content/60 space-y-2 text-sm">
						<li>
							<a href="#" class="hover:text-primary">Privacy</a>
						</li>
						<li><a href="#" class="hover:text-primary">Terms</a></li>
						<li>
							<a href="#" class="hover:text-primary">Cat Safety</a>
						</li>
					</ul>
				</div>
			</div>
			<div
				class="border-base-300 text-base-content/60 border-t pt-8 text-center text-sm"
			>
				© 2024 Purrfect Match. All rights reserved. Made with 😺 for
				cats everywhere.
			</div>
		</div>
	</footer>
</div>
