<script lang="ts">
	let email = $state('');
</script>

<div
	class="min-h-screen bg-[linear-gradient(#ccc_1px,transparent_1px),linear-gradient(90deg,#ccc_1px,transparent_1px)] bg-size-[20px_20px]"
>
	<!-- Nav -->
	<nav
		class="border-border flex items-center justify-between border-b p-6"
	>
		<div class="font-(family-name:--font-display) text-xl">
			[ PurrMatch ]
		</div>
		<div class="flex gap-6">
			<a href="#features" class="hover:underline">Features</a>
			<a href="#how" class="hover:underline">How it Works</a>
			<a href="#pricing" class="hover:underline">Pricing</a>
		</div>
		<button
			class="border-foreground hover:bg-foreground/5 border px-4 py-2"
		>
			Sign In
		</button>
	</nav>

	<!-- Hero -->
	<section
		class="border-border flex flex-col items-center border-b px-6 py-24 text-center"
	>
		<div
			class="border-foreground/40 mb-8 flex h-32 w-32 items-center justify-center rounded-full border-2 border-dashed"
		>
			<span class="text-4xl">🐱</span>
		</div>
		<h1 class="mb-4 font-(family-name:--font-display) text-5xl">
			Find Your Cat's Purr-fect Match
		</h1>
		<p class="text-muted-foreground mb-8 max-w-md">
			The premier dating app for cats. Swipe, match, and let your
			feline find their soulmate.
		</p>
		<div class="flex gap-4">
			<button
				class="bg-primary text-primary-foreground rounded-sm px-6 py-3 hover:brightness-110"
			>
				Get Started
			</button>
			<button
				class="border-foreground hover:bg-foreground/5 rounded-sm border px-6 py-3"
			>
				Learn More
			</button>
		</div>
	</section>

	<!-- Features -->
	<section id="features" class="border-border border-b px-6 py-20">
		<h2
			class="mb-12 text-center font-(family-name:--font-display) text-3xl"
		>
			[ Features ]
		</h2>
		<div
			class="mx-auto grid max-w-5xl grid-cols-1 gap-8 md:grid-cols-3"
		>
			<div class="border-border border p-6">
				<div
					class="border-foreground/40 mb-4 flex h-16 w-16 items-center justify-center border border-dashed"
				>
					<span class="text-2xl">📸</span>
				</div>
				<h3 class="mb-2 font-bold">Photo Profiles</h3>
				<p class="text-muted-foreground text-sm">
					Showcase your cat's best angles with up to 6 photos
				</p>
			</div>
			<div class="border-border border p-6">
				<div
					class="border-foreground/40 mb-4 flex h-16 w-16 items-center justify-center border border-dashed"
				>
					<span class="text-2xl">💬</span>
				</div>
				<h3 class="mb-2 font-bold">Meow Messaging</h3>
				<p class="text-muted-foreground text-sm">
					Chat with matches using our cat-friendly interface
				</p>
			</div>
			<div class="border-border border p-6">
				<div
					class="border-foreground/40 mb-4 flex h-16 w-16 items-center justify-center border border-dashed"
				>
					<span class="text-2xl">📍</span>
				</div>
				<h3 class="mb-2 font-bold">Local Matches</h3>
				<p class="text-muted-foreground text-sm">
					Find cats in your neighborhood for easy meetups
				</p>
			</div>
		</div>
	</section>

	<!-- How it Works -->
	<section id="how" class="border-border border-b px-6 py-20">
		<h2
			class="mb-12 text-center font-(family-name:--font-display) text-3xl"
		>
			[ How It Works ]
		</h2>
		<div
			class="mx-auto flex max-w-4xl flex-col items-center justify-center gap-8 md:flex-row"
		>
			<div class="text-center">
				<div
					class="border-foreground mx-auto mb-4 flex h-20 w-20 items-center justify-center rounded-full border-2"
				>
					<span class="text-2xl font-bold">1</span>
				</div>
				<p class="font-bold">Create Profile</p>
			</div>
			<div
				class="border-foreground/40 hidden w-16 border-t border-dashed md:block"
			></div>
			<div class="text-center">
				<div
					class="border-foreground mx-auto mb-4 flex h-20 w-20 items-center justify-center rounded-full border-2"
				>
					<span class="text-2xl font-bold">2</span>
				</div>
				<p class="font-bold">Swipe & Match</p>
			</div>
			<div
				class="border-foreground/40 hidden w-16 border-t border-dashed md:block"
			></div>
			<div class="text-center">
				<div
					class="border-foreground mx-auto mb-4 flex h-20 w-20 items-center justify-center rounded-full border-2"
				>
					<span class="text-2xl font-bold">3</span>
				</div>
				<p class="font-bold">Meet & Greet</p>
			</div>
		</div>
	</section>

	<!-- Testimonials -->
	<section class="border-border border-b px-6 py-20">
		<h2
			class="mb-12 text-center font-(family-name:--font-display) text-3xl"
		>
			[ Success Stories ]
		</h2>
		<div
			class="mx-auto grid max-w-4xl grid-cols-1 gap-8 md:grid-cols-2"
		>
			<div class="border-border border p-6">
				<div class="mb-4 flex items-center gap-4">
					<div
						class="border-foreground/40 h-12 w-12 rounded-full border border-dashed"
					></div>
					<div>
						<p class="font-bold">Whiskers & Luna</p>
						<p class="text-muted-foreground text-sm">
							Matched 6 months ago
						</p>
					</div>
				</div>
				<p class="text-muted-foreground italic">
					"We're now happily napping together every day!"
				</p>
			</div>
			<div class="border-border border p-6">
				<div class="mb-4 flex items-center gap-4">
					<div
						class="border-foreground/40 h-12 w-12 rounded-full border border-dashed"
					></div>
					<div>
						<p class="font-bold">Mr. Fluffkins & Bella</p>
						<p class="text-muted-foreground text-sm">
							Matched 1 year ago
						</p>
					</div>
				</div>
				<p class="text-muted-foreground italic">
					"Found my soulmate. 10/10 would swipe right again."
				</p>
			</div>
		</div>
	</section>

	<!-- CTA -->
	<section class="border-border border-b px-6 py-20">
		<div class="mx-auto max-w-xl text-center">
			<h2 class="mb-4 font-(family-name:--font-display) text-3xl">
				Ready to Find Love?
			</h2>
			<p class="text-muted-foreground mb-8">
				Join thousands of cats finding their perfect match
			</p>
			<div class="flex justify-center gap-4">
				<input
					type="email"
					bind:value={email}
					placeholder="whiskers@email.com"
					class="border-border w-64 border bg-transparent px-4 py-3 focus:outline-2 focus:outline-dashed"
				/>
				<button
					class="bg-primary text-primary-foreground px-6 py-3 hover:brightness-110"
				>
					Sign Up
				</button>
			</div>
		</div>
	</section>

	<!-- Footer -->
	<footer class="px-6 py-12">
		<div
			class="mx-auto flex max-w-5xl flex-col items-center justify-between gap-8 md:flex-row"
		>
			<div class="font-(family-name:--font-display)">
				[ PurrMatch ]
			</div>
			<div class="text-muted-foreground flex gap-8 text-sm">
				<a href="#" class="hover:underline">Privacy</a>
				<a href="#" class="hover:underline">Terms</a>
				<a href="#" class="hover:underline">Contact</a>
			</div>
			<p class="text-muted-foreground text-sm">© 2026 PurrMatch</p>
		</div>
	</footer>
</div>
