<script lang="ts">
	let email = $state('');
</script>

<svelte:head>
	<title>PurrMatch - Find Your Cat's Purrfect Partner</title>
</svelte:head>

<div class="bg-background text-foreground min-h-screen">
	<!-- Hero Section -->
	<header class="relative overflow-hidden">
		<!-- Decorative blobs -->
		<div
			class="bg-primary/20 absolute -top-20 -left-20 h-72 w-72 animate-[sway_8s_ease-in-out_infinite] rounded-[60%_40%_30%_70%/60%_30%_70%_40%] blur-3xl"
		></div>
		<div
			class="bg-secondary/20 absolute top-40 -right-20 h-96 w-96 animate-[sway_10s_ease-in-out_infinite_reverse] rounded-[30%_60%_70%_40%/50%_60%_30%_60%] blur-3xl"
		></div>

		<nav
			class="relative z-10 mx-auto flex max-w-6xl items-center justify-between px-6 py-6"
		>
			<div
				class="text-primary font-(family-name:--font-display) text-2xl font-bold"
			>
				PurrMatch
			</div>
			<div class="flex items-center gap-6">
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
				<button
					class="bg-primary text-primary-foreground rounded-full px-6 py-2 font-semibold transition-all hover:scale-[1.02] hover:shadow-[0_8px_30px_rgba(34,197,94,0.3)] active:scale-[0.98]"
				>
					Sign Up
				</button>
			</div>
		</nav>

		<div
			class="relative z-10 mx-auto grid max-w-6xl items-center gap-12 px-6 py-20 md:grid-cols-2"
		>
			<div
				class="animate-[grow_0.6s_cubic-bezier(0.25,0.46,0.45,0.94)]"
			>
				<h1
					class="mb-6 font-(family-name:--font-display) text-5xl font-bold md:text-6xl"
				>
					Find Your Cat's <span class="text-primary">Purrfect</span> Partner
				</h1>
				<p class="text-muted-foreground mb-8 text-xl leading-relaxed">
					The premier dating app for cats. Connect your feline friend
					with compatible companions for playdates, friendship, or
					finding their soulmate.
				</p>
				<div class="flex flex-wrap gap-4">
					<button
						class="bg-primary text-primary-foreground rounded-full px-8 py-4 text-lg font-semibold transition-all hover:scale-[1.02] hover:shadow-[0_8px_30px_rgba(34,197,94,0.3)] active:scale-[0.98]"
					>
						Get Started Free
					</button>
					<button
						class="bg-muted text-foreground hover:bg-border rounded-full px-8 py-4 text-lg font-semibold transition-all hover:scale-[1.02] active:scale-[0.98]"
					>
						Learn More
					</button>
				</div>
			</div>
			<div class="relative animate-[float_6s_ease-in-out_infinite]">
				<div
					class="bg-muted rounded-[60%_40%_30%_70%/60%_30%_70%_40%] p-8 shadow-[0_8px_30px_rgba(34,197,94,0.3)]"
				>
					<div class="text-center">
						<div class="mb-4 text-8xl">🐱❤️🐱</div>
						<p
							class="text-muted-foreground font-(family-name:--font-display) text-xl"
						>
							50,000+ Happy Matches
						</p>
					</div>
				</div>
			</div>
		</div>
	</header>

	<!-- Features Section -->
	<section id="features" class="bg-muted py-24">
		<div class="mx-auto max-w-6xl px-6">
			<h2
				class="mb-4 text-center font-(family-name:--font-display) text-4xl font-bold"
			>
				Why Cats Love PurrMatch
			</h2>
			<p
				class="text-muted-foreground mx-auto mb-16 max-w-2xl text-center"
			>
				Built by cat lovers, for cats. Every feature designed with
				feline happiness in mind.
			</p>

			<div class="grid gap-8 md:grid-cols-3">
				<div
					class="bg-background rounded-2xl p-8 shadow-[0_4px_20px_rgba(34,197,94,0.2)] transition-all hover:scale-[1.02] hover:shadow-[0_8px_30px_rgba(34,197,94,0.3)]"
				>
					<div class="mb-6 text-5xl">🎯</div>
					<h3
						class="mb-3 font-(family-name:--font-display) text-xl font-bold"
					>
						Purrsonality Matching
					</h3>
					<p class="text-muted-foreground">
						Our AI analyzes your cat's unique traits to find
						compatible companions based on temperament, energy level,
						and play style.
					</p>
				</div>

				<div
					class="bg-background rounded-2xl p-8 shadow-[0_4px_20px_rgba(34,197,94,0.2)] transition-all hover:scale-[1.02] hover:shadow-[0_8px_30px_rgba(34,197,94,0.3)]"
				>
					<div class="mb-6 text-5xl">📍</div>
					<h3
						class="mb-3 font-(family-name:--font-display) text-xl font-bold"
					>
						Local Connections
					</h3>
					<p class="text-muted-foreground">
						Find feline friends in your neighborhood. Arrange safe
						playdates at local cat cafes or parks with our meetup
						feature.
					</p>
				</div>

				<div
					class="bg-background rounded-2xl p-8 shadow-[0_4px_20px_rgba(34,197,94,0.2)] transition-all hover:scale-[1.02] hover:shadow-[0_8px_30px_rgba(34,197,94,0.3)]"
				>
					<div class="mb-6 text-5xl">🛡️</div>
					<h3
						class="mb-3 font-(family-name:--font-display) text-xl font-bold"
					>
						Verified Profiles
					</h3>
					<p class="text-muted-foreground">
						Every cat profile is verified by their human. Health
						records, vaccination status, and temperament assessments
						included.
					</p>
				</div>
			</div>
		</div>
	</section>

	<!-- How It Works -->
	<section id="how" class="py-24">
		<div class="mx-auto max-w-6xl px-6">
			<h2
				class="mb-16 text-center font-(family-name:--font-display) text-4xl font-bold"
			>
				How It Works
			</h2>

			<div class="grid gap-8 md:grid-cols-4">
				<div class="text-center">
					<div
						class="bg-primary/20 mx-auto mb-6 flex h-20 w-20 items-center justify-center rounded-full"
					>
						<span class="text-primary text-3xl font-bold">1</span>
					</div>
					<h3
						class="mb-2 font-(family-name:--font-display) font-bold"
					>
						Create Profile
					</h3>
					<p class="text-muted-foreground text-sm">
						Share your cat's photos, personality traits, and
						preferences
					</p>
				</div>

				<div class="text-center">
					<div
						class="bg-secondary/20 mx-auto mb-6 flex h-20 w-20 items-center justify-center rounded-full"
					>
						<span class="text-secondary text-3xl font-bold">2</span>
					</div>
					<h3
						class="mb-2 font-(family-name:--font-display) font-bold"
					>
						Get Matches
					</h3>
					<p class="text-muted-foreground text-sm">
						Our algorithm finds the most compatible feline companions
					</p>
				</div>

				<div class="text-center">
					<div
						class="bg-accent/20 mx-auto mb-6 flex h-20 w-20 items-center justify-center rounded-full"
					>
						<span class="text-accent-foreground text-3xl font-bold"
							>3</span
						>
					</div>
					<h3
						class="mb-2 font-(family-name:--font-display) font-bold"
					>
						Chat & Connect
					</h3>
					<p class="text-muted-foreground text-sm">
						Message other cat parents to plan the purrfect meetup
					</p>
				</div>

				<div class="text-center">
					<div
						class="bg-success/20 mx-auto mb-6 flex h-20 w-20 items-center justify-center rounded-full"
					>
						<span class="text-success text-3xl font-bold">4</span>
					</div>
					<h3
						class="mb-2 font-(family-name:--font-display) font-bold"
					>
						Playdate!
					</h3>
					<p class="text-muted-foreground text-sm">
						Watch your cats form new friendships and memories
					</p>
				</div>
			</div>
		</div>
	</section>

	<!-- Testimonials -->
	<section class="bg-muted py-24">
		<div class="mx-auto max-w-6xl px-6">
			<h2
				class="mb-16 text-center font-(family-name:--font-display) text-4xl font-bold"
			>
				Success Stories
			</h2>

			<div class="grid gap-8 md:grid-cols-2">
				<div
					class="bg-background rounded-2xl p-8 shadow-[0_4px_20px_rgba(34,197,94,0.2)]"
				>
					<div class="mb-6 flex items-center gap-4">
						<div class="text-5xl">🐱</div>
						<div>
							<h4 class="font-(family-name:--font-display) font-bold">
								Whiskers & Mittens
							</h4>
							<p class="text-muted-foreground text-sm">
								Matched 6 months ago
							</p>
						</div>
					</div>
					<p class="text-muted-foreground italic">
						"Whiskers was so lonely after we moved. PurrMatch helped
						him find Mittens, and now they're inseparable! They have
						weekly playdates and even nap together."
					</p>
					<p class="mt-4 font-semibold">— Sarah M., Cat Mom</p>
				</div>

				<div
					class="bg-background rounded-2xl p-8 shadow-[0_4px_20px_rgba(34,197,94,0.2)]"
				>
					<div class="mb-6 flex items-center gap-4">
						<div class="text-5xl">😺</div>
						<div>
							<h4 class="font-(family-name:--font-display) font-bold">
								Luna & Oliver
							</h4>
							<p class="text-muted-foreground text-sm">
								Matched 1 year ago
							</p>
						</div>
					</div>
					<p class="text-muted-foreground italic">
						"I never thought my shy Luna would find a friend. Oliver's
						calm personality was the perfect match. Now they're the
						best of friends!"
					</p>
					<p class="mt-4 font-semibold">— Mike T., Proud Cat Dad</p>
				</div>
			</div>
		</div>
	</section>

	<!-- CTA Section -->
	<section class="relative overflow-hidden py-24">
		<div
			class="from-primary/10 via-secondary/10 to-accent/10 absolute inset-0 bg-linear-to-br"
		></div>
		<div class="relative z-10 mx-auto max-w-3xl px-6 text-center">
			<h2
				class="mb-6 font-(family-name:--font-display) text-4xl font-bold"
			>
				Ready to Find Your Cat's Match?
			</h2>
			<p class="text-muted-foreground mb-8 text-xl">
				Join thousands of happy cats who found their purrfect
				companions through PurrMatch.
			</p>

			<form
				class="mx-auto flex max-w-md flex-col justify-center gap-4 sm:flex-row"
			>
				<input
					type="email"
					bind:value={email}
					placeholder="Enter your email"
					class="bg-background border-border focus:ring-primary flex-1 rounded-full border px-6 py-4 focus:ring-2 focus:outline-none"
				/>
				<button
					type="submit"
					class="bg-primary text-primary-foreground rounded-full px-8 py-4 font-semibold transition-all hover:scale-[1.02] hover:shadow-[0_8px_30px_rgba(34,197,94,0.3)] active:scale-[0.98]"
				>
					Get Started
				</button>
			</form>

			<p class="text-muted-foreground mt-4 text-sm">
				Free forever. No credit card required.
			</p>
		</div>
	</section>

	<!-- Footer -->
	<footer class="bg-foreground text-background py-12">
		<div class="mx-auto max-w-6xl px-6">
			<div class="grid gap-8 md:grid-cols-4">
				<div>
					<div
						class="mb-4 font-(family-name:--font-display) text-2xl font-bold"
					>
						PurrMatch
					</div>
					<p class="text-background/70">
						Connecting cats, one playdate at a time.
					</p>
				</div>
				<div>
					<h4 class="mb-4 font-bold">Product</h4>
					<ul class="text-background/70 space-y-2">
						<li>
							<a
								href="#features"
								class="hover:text-background transition-colors"
								>Features</a
							>
						</li>
						<li>
							<a
								href="#how"
								class="hover:text-background transition-colors"
								>How It Works</a
							>
						</li>
						<li>
							<a
								href="#"
								class="hover:text-background transition-colors"
								>Pricing</a
							>
						</li>
					</ul>
				</div>
				<div>
					<h4 class="mb-4 font-bold">Company</h4>
					<ul class="text-background/70 space-y-2">
						<li>
							<a
								href="#"
								class="hover:text-background transition-colors"
								>About</a
							>
						</li>
						<li>
							<a
								href="#"
								class="hover:text-background transition-colors"
								>Blog</a
							>
						</li>
						<li>
							<a
								href="#"
								class="hover:text-background transition-colors"
								>Careers</a
							>
						</li>
					</ul>
				</div>
				<div>
					<h4 class="mb-4 font-bold">Legal</h4>
					<ul class="text-background/70 space-y-2">
						<li>
							<a
								href="#"
								class="hover:text-background transition-colors"
								>Privacy</a
							>
						</li>
						<li>
							<a
								href="#"
								class="hover:text-background transition-colors"
								>Terms</a
							>
						</li>
					</ul>
				</div>
			</div>
			<div
				class="border-background/20 text-background/70 mt-12 border-t pt-8 text-center"
			>
				<p>
					&copy; 2025 PurrMatch. Made with 🐱 for cats everywhere.
				</p>
			</div>
		</div>
	</footer>
</div>
