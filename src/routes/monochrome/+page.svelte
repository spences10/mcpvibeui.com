<script lang="ts">
	let email = $state('');
</script>

<div class="bg-background text-foreground font-body min-h-screen">
	<!-- Header -->
	<header class="border-border border-b">
		<div
			class="mx-auto flex max-w-6xl items-center justify-between px-6 py-4"
		>
			<div class="flex items-center gap-2">
				<span class="text-2xl">~(=^..^)</span>
				<span
					class="font-display text-xl font-semibold tracking-tight"
				>
					PurrMatch
				</span>
			</div>
			<nav class="hidden items-center gap-8 md:flex">
				<a
					href="#features"
					class="text-muted-foreground hover:text-foreground transition-colors"
				>
					Features
				</a>
				<a
					href="#how"
					class="text-muted-foreground hover:text-foreground transition-colors"
				>
					How It Works
				</a>
				<a
					href="#testimonials"
					class="text-muted-foreground hover:text-foreground transition-colors"
				>
					Stories
				</a>
			</nav>
			<button
				class="border-foreground hover:bg-foreground hover:text-background border-2 bg-transparent px-4 py-2 text-sm font-medium transition-colors"
			>
				Sign In
			</button>
		</div>
	</header>

	<!-- Hero -->
	<section class="px-6 py-24 text-center md:py-32">
		<div class="mx-auto max-w-3xl">
			<p
				class="text-muted-foreground mb-4 font-mono text-sm tracking-widest uppercase"
			>
				Find your feline soulmate
			</p>
			<h1
				class="font-display mb-6 text-5xl font-bold tracking-tight md:text-6xl lg:text-7xl"
			>
				Where Cats Find<br />Their Purrfect Match
			</h1>
			<p class="text-muted-foreground mx-auto mb-10 max-w-xl text-lg">
				The premier dating platform for discerning cats and their
				devoted humans. Swipe right on destiny.
			</p>
			<div
				class="flex flex-col items-center justify-center gap-4 sm:flex-row"
			>
				<button
					class="bg-foreground text-background hover:bg-foreground/90 w-full px-8 py-3 font-medium transition-colors sm:w-auto"
				>
					Get Started Free
				</button>
				<button
					class="border-foreground hover:bg-foreground hover:text-background w-full border-2 bg-transparent px-8 py-3 font-medium transition-colors sm:w-auto"
				>
					Watch Demo
				</button>
			</div>
		</div>
	</section>

	<!-- Stats -->
	<section class="border-border bg-muted border-y py-12">
		<div
			class="mx-auto grid max-w-4xl grid-cols-2 gap-8 px-6 md:grid-cols-4"
		>
			<div class="text-center">
				<p class="font-display text-3xl font-bold md:text-4xl">
					50K+
				</p>
				<p class="text-muted-foreground mt-1 text-sm">Happy Cats</p>
			</div>
			<div class="text-center">
				<p class="font-display text-3xl font-bold md:text-4xl">12K</p>
				<p class="text-muted-foreground mt-1 text-sm">Matches Made</p>
			</div>
			<div class="text-center">
				<p class="font-display text-3xl font-bold md:text-4xl">98%</p>
				<p class="text-muted-foreground mt-1 text-sm">Satisfaction</p>
			</div>
			<div class="text-center">
				<p class="font-display text-3xl font-bold md:text-4xl">
					24/7
				</p>
				<p class="text-muted-foreground mt-1 text-sm">Nap Support</p>
			</div>
		</div>
	</section>

	<!-- Features -->
	<section id="features" class="px-6 py-24">
		<div class="mx-auto max-w-6xl">
			<div class="mb-16 text-center">
				<p
					class="text-muted-foreground mb-3 font-mono text-sm tracking-widest uppercase"
				>
					Features
				</p>
				<h2 class="font-display text-3xl font-bold md:text-4xl">
					Built for Cats, by Cat Lovers
				</h2>
			</div>
			<div class="grid gap-8 md:grid-cols-3">
				<div class="bg-muted rounded p-8">
					<div
						class="bg-foreground text-background mb-4 flex h-12 w-12 items-center justify-center rounded text-xl"
					>
						^..^
					</div>
					<h3 class="font-display mb-2 text-lg font-semibold">
						Whisker Recognition
					</h3>
					<p class="text-muted-foreground">
						Advanced AI that matches cats based on whisker patterns,
						tail fluffiness, and preferred napping positions.
					</p>
				</div>
				<div class="bg-muted rounded p-8">
					<div
						class="bg-foreground text-background mb-4 flex h-12 w-12 items-center justify-center rounded text-xl"
					>
						*~*
					</div>
					<h3 class="font-display mb-2 text-lg font-semibold">
						Treat Compatibility
					</h3>
					<p class="text-muted-foreground">
						Our algorithm considers treat preferences, from salmon
						pate to chicken crunchies.
					</p>
				</div>
				<div class="bg-muted rounded p-8">
					<div
						class="bg-foreground text-background mb-4 flex h-12 w-12 items-center justify-center rounded text-xl"
					>
						=^.^=
					</div>
					<h3 class="font-display mb-2 text-lg font-semibold">
						Territory Mapping
					</h3>
					<p class="text-muted-foreground">
						Find cats in your area who share your interest in window
						watching and bird TV.
					</p>
				</div>
			</div>
		</div>
	</section>

	<!-- How It Works -->
	<section
		id="how"
		class="border-border bg-muted border-y px-6 py-24"
	>
		<div class="mx-auto max-w-4xl">
			<div class="mb-16 text-center">
				<p
					class="text-muted-foreground mb-3 font-mono text-sm tracking-widest uppercase"
				>
					How It Works
				</p>
				<h2 class="font-display text-3xl font-bold md:text-4xl">
					Three Steps to Love
				</h2>
			</div>
			<div class="space-y-12">
				<div class="flex items-start gap-6">
					<div
						class="border-foreground flex h-10 w-10 shrink-0 items-center justify-center rounded-full border-2 font-mono text-sm font-bold"
					>
						01
					</div>
					<div>
						<h3 class="font-display mb-2 text-lg font-semibold">
							Create Your Paw-file
						</h3>
						<p class="text-muted-foreground">
							Upload your best zoomie action shots, nap selfies, and
							that one photo where you knocked something off the
							counter.
						</p>
					</div>
				</div>
				<div class="flex items-start gap-6">
					<div
						class="border-foreground flex h-10 w-10 shrink-0 items-center justify-center rounded-full border-2 font-mono text-sm font-bold"
					>
						02
					</div>
					<div>
						<h3 class="font-display mb-2 text-lg font-semibold">
							Swipe & Scratch
						</h3>
						<p class="text-muted-foreground">
							Browse profiles of eligible cats. Swipe right if you'd
							share your cardboard box, left if they seem like a
							vacuum lover.
						</p>
					</div>
				</div>
				<div class="flex items-start gap-6">
					<div
						class="border-foreground flex h-10 w-10 shrink-0 items-center justify-center rounded-full border-2 font-mono text-sm font-bold"
					>
						03
					</div>
					<div>
						<h3 class="font-display mb-2 text-lg font-semibold">
							Meet & Meow
						</h3>
						<p class="text-muted-foreground">
							Arrange a playdate at neutral territory. We recommend
							somewhere with plenty of hiding spots and cardboard
							boxes.
						</p>
					</div>
				</div>
			</div>
		</div>
	</section>

	<!-- Testimonials -->
	<section id="testimonials" class="px-6 py-24">
		<div class="mx-auto max-w-6xl">
			<div class="mb-16 text-center">
				<p
					class="text-muted-foreground mb-3 font-mono text-sm tracking-widest uppercase"
				>
					Success Stories
				</p>
				<h2 class="font-display text-3xl font-bold md:text-4xl">
					Happy Tails
				</h2>
			</div>
			<div class="grid gap-8 md:grid-cols-2">
				<div class="border-border rounded border p-8">
					<p class="text-muted-foreground mb-6 text-lg italic">
						"I was skeptical at first, but then I met Whiskers. We
						bonded over our mutual hatred of closed doors and love of
						3am zoomies."
					</p>
					<div class="flex items-center gap-4">
						<div
							class="bg-muted flex h-12 w-12 items-center justify-center rounded-full font-mono text-lg"
						>
							MC
						</div>
						<div>
							<p class="font-semibold">Mr. Cuddles</p>
							<p class="text-muted-foreground text-sm">
								Tabby, 4 years old
							</p>
						</div>
					</div>
				</div>
				<div class="border-border rounded border p-8">
					<p class="text-muted-foreground mb-6 text-lg italic">
						"Finally, an app that understands that personality means
						more than fluff. Found my soulmate who also believes 5am
						is breakfast time."
					</p>
					<div class="flex items-center gap-4">
						<div
							class="bg-muted flex h-12 w-12 items-center justify-center rounded-full font-mono text-lg"
						>
							PM
						</div>
						<div>
							<p class="font-semibold">Princess Mittens</p>
							<p class="text-muted-foreground text-sm">
								Persian, 3 years old
							</p>
						</div>
					</div>
				</div>
			</div>
		</div>
	</section>

	<!-- CTA -->
	<section
		class="border-border bg-foreground text-background border-t px-6 py-24"
	>
		<div class="mx-auto max-w-2xl text-center">
			<h2 class="font-display mb-4 text-3xl font-bold md:text-4xl">
				Ready to Find Your Match?
			</h2>
			<p class="text-background/70 mb-8">
				Join thousands of cats who've found their purrfect companion.
				Your soulmate is just a swipe away.
			</p>
			<form
				class="flex flex-col gap-4 sm:flex-row sm:justify-center"
				onsubmit={(e) => e.preventDefault()}
			>
				<input
					type="email"
					bind:value={email}
					placeholder="Enter your email"
					class="border-background/30 text-background placeholder:text-background/50 focus:border-background rounded border-2 bg-transparent px-4 py-3 focus:outline-none sm:w-64"
				/>
				<button
					type="submit"
					class="bg-background text-foreground hover:bg-background/90 rounded px-6 py-3 font-medium transition-colors"
				>
					Get Early Access
				</button>
			</form>
		</div>
	</section>

	<!-- Footer -->
	<footer class="border-border border-t px-6 py-12">
		<div class="mx-auto max-w-6xl">
			<div
				class="flex flex-col items-center justify-between gap-6 md:flex-row"
			>
				<div class="flex items-center gap-2">
					<span class="text-xl">~(=^..^)</span>
					<span class="font-display font-semibold">PurrMatch</span>
				</div>
				<nav class="text-muted-foreground flex gap-6 text-sm">
					<a href="#" class="hover:text-foreground">Privacy</a>
					<a href="#" class="hover:text-foreground">Terms</a>
					<a href="#" class="hover:text-foreground">Contact</a>
				</nav>
				<p class="text-muted-foreground text-sm">
					&copy; 2025 PurrMatch. All rights reserved.
				</p>
			</div>
		</div>
	</footer>
</div>
