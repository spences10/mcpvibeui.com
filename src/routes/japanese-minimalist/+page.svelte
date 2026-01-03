<script lang="ts">
	let email = $state('');
</script>

<div class="bg-background text-foreground min-h-screen">
	<!-- Navigation -->
	<nav
		class="bg-background/95 border-border fixed top-0 z-50 w-full border-b backdrop-blur-sm"
	>
		<div
			class="mx-auto flex max-w-6xl items-center justify-between px-6 py-4"
		>
			<div
				class="font-(family-name:--font-display) text-xl font-medium tracking-wide"
			>
				<span class="text-primary">neko</span>match
			</div>
			<div
				class="text-muted-foreground flex gap-8 font-(family-name:--font-display) text-sm"
			>
				<a
					href="#about"
					class="hover:text-foreground transition-colors">About</a
				>
				<a
					href="#features"
					class="hover:text-foreground transition-colors">Features</a
				>
				<a
					href="#join"
					class="hover:text-foreground transition-colors">Join</a
				>
			</div>
		</div>
	</nav>

	<!-- Hero Section -->
	<section
		class="flex min-h-screen items-center justify-center px-6 pt-20"
	>
		<div class="mx-auto max-w-4xl text-center">
			<!-- Minimal cat illustration -->
			<div class="mb-12 animate-[float_4s_ease-in-out_infinite]">
				<svg
					class="text-foreground/80 mx-auto h-32 w-32"
					viewBox="0 0 100 100"
					fill="none"
					stroke="currentColor"
					stroke-width="1.5"
				>
					<!-- Cat face outline -->
					<ellipse cx="50" cy="55" rx="30" ry="25" />
					<!-- Left ear -->
					<path d="M25 40 L20 20 L35 35" />
					<!-- Right ear -->
					<path d="M75 40 L80 20 L65 35" />
					<!-- Eyes -->
					<circle cx="40" cy="50" r="3" fill="currentColor" />
					<circle cx="60" cy="50" r="3" fill="currentColor" />
					<!-- Nose -->
					<path d="M50 58 L47 62 L53 62 Z" fill="currentColor" />
					<!-- Whiskers -->
					<line x1="30" y1="58" x2="15" y2="55" />
					<line x1="30" y1="62" x2="15" y2="65" />
					<line x1="70" y1="58" x2="85" y2="55" />
					<line x1="70" y1="62" x2="85" y2="65" />
				</svg>
			</div>

			<p
				class="text-muted-foreground mb-6 font-(family-name:--font-display) text-sm tracking-[0.3em] uppercase"
			>
				find your cat's perfect companion
			</p>

			<h1
				class="mb-8 font-(family-name:--font-display) text-5xl font-light tracking-tight md:text-7xl"
			>
				Where cats find
				<span class="text-primary block font-medium">harmony</span>
			</h1>

			<p
				class="text-muted-foreground mx-auto mb-12 max-w-xl text-lg leading-relaxed"
			>
				A mindful approach to feline friendship. Connect your cat with
				compatible companions through thoughtful matching.
			</p>

			<a
				href="#join"
				class="border-foreground/20 hover:bg-foreground hover:text-background inline-block border px-8 py-3 font-(family-name:--font-display) text-sm tracking-wide transition-all duration-300"
			>
				Begin the journey
			</a>
		</div>
	</section>

	<!-- About Section -->
	<section id="about" class="px-6 py-32">
		<div class="mx-auto max-w-4xl">
			<div class="grid items-center gap-16 md:grid-cols-2">
				<div>
					<p
						class="text-muted-foreground mb-4 font-(family-name:--font-display) text-xs tracking-[0.2em] uppercase"
					>
						Philosophy
					</p>
					<h2
						class="mb-6 font-(family-name:--font-display) text-3xl font-light"
					>
						Balance in companionship
					</h2>
					<p class="text-muted-foreground mb-6 leading-relaxed">
						Just as nature finds equilibrium, we believe every cat
						deserves a companion that complements their unique spirit.
					</p>
					<p class="text-muted-foreground leading-relaxed">
						Our matching considers temperament, energy, and the subtle
						nuances that create lasting feline friendships.
					</p>
				</div>
				<div
					class="bg-muted flex items-center justify-center rounded-lg p-12"
				>
					<svg
						class="text-foreground/30 h-48 w-48"
						viewBox="0 0 100 100"
						fill="none"
						stroke="currentColor"
						stroke-width="0.75"
					>
						<!-- Enso circle -->
						<path
							d="M50 10 A40 40 0 1 1 45 10"
							stroke-linecap="round"
						/>
						<!-- Small cat silhouette -->
						<ellipse cx="50" cy="55" rx="12" ry="10" />
						<path d="M42 50 L40 42 L46 48" />
						<path d="M58 50 L60 42 L54 48" />
					</svg>
				</div>
			</div>
		</div>
	</section>

	<!-- Features Section -->
	<section id="features" class="bg-muted/50 px-6 py-32">
		<div class="mx-auto max-w-4xl">
			<div class="mb-20 text-center">
				<p
					class="text-muted-foreground mb-4 font-(family-name:--font-display) text-xs tracking-[0.2em] uppercase"
				>
					The way
				</p>
				<h2
					class="font-(family-name:--font-display) text-3xl font-light"
				>
					Simple. Intentional. Effective.
				</h2>
			</div>

			<div class="grid gap-12 md:grid-cols-3">
				<div class="text-center">
					<div
						class="border-border mx-auto mb-6 flex h-16 w-16 items-center justify-center rounded border"
					>
						<span
							class="text-primary font-(family-name:--font-display) text-2xl"
							>1</span
						>
					</div>
					<h3
						class="mb-3 font-(family-name:--font-display) font-medium"
					>
						Create profile
					</h3>
					<p class="text-muted-foreground text-sm leading-relaxed">
						Share your cat's personality, preferences, and photos
					</p>
				</div>

				<div class="text-center">
					<div
						class="border-border mx-auto mb-6 flex h-16 w-16 items-center justify-center rounded border"
					>
						<span
							class="text-primary font-(family-name:--font-display) text-2xl"
							>2</span
						>
					</div>
					<h3
						class="mb-3 font-(family-name:--font-display) font-medium"
					>
						Discover matches
					</h3>
					<p class="text-muted-foreground text-sm leading-relaxed">
						Our algorithm finds cats with compatible energies
					</p>
				</div>

				<div class="text-center">
					<div
						class="border-border mx-auto mb-6 flex h-16 w-16 items-center justify-center rounded border"
					>
						<span
							class="text-primary font-(family-name:--font-display) text-2xl"
							>3</span
						>
					</div>
					<h3
						class="mb-3 font-(family-name:--font-display) font-medium"
					>
						Connect
					</h3>
					<p class="text-muted-foreground text-sm leading-relaxed">
						Arrange playdates and watch friendships bloom
					</p>
				</div>
			</div>
		</div>
	</section>

	<!-- Testimonial -->
	<section class="px-6 py-32">
		<div class="mx-auto max-w-2xl text-center">
			<svg
				class="text-muted-foreground/50 mx-auto mb-8 h-8 w-8"
				viewBox="0 0 24 24"
				fill="currentColor"
			>
				<path
					d="M4.583 17.321C3.553 16.227 3 15 3 13.011c0-3.5 2.457-6.637 6.03-8.188l.893 1.378c-3.335 1.804-3.987 4.145-4.247 5.621.537-.278 1.24-.375 1.929-.311 1.804.167 3.226 1.648 3.226 3.489a3.5 3.5 0 01-3.5 3.5c-1.073 0-2.099-.49-2.748-1.179zm10 0C13.553 16.227 13 15 13 13.011c0-3.5 2.457-6.637 6.03-8.188l.893 1.378c-3.335 1.804-3.987 4.145-4.247 5.621.537-.278 1.24-.375 1.929-.311 1.804.167 3.226 1.648 3.226 3.489a3.5 3.5 0 01-3.5 3.5c-1.073 0-2.099-.49-2.748-1.179z"
				/>
			</svg>
			<p class="text-foreground/80 mb-8 text-xl leading-relaxed">
				Mochi was so lonely. Through nekomatch, she found Sakura. Now
				they groom each other every evening.
			</p>
			<p
				class="text-muted-foreground font-(family-name:--font-display) text-sm"
			>
				Yuki T. — Tokyo
			</p>
		</div>
	</section>

	<!-- Join Section -->
	<section id="join" class="bg-muted/30 px-6 py-32">
		<div class="mx-auto max-w-md text-center">
			<p
				class="text-muted-foreground mb-4 font-(family-name:--font-display) text-xs tracking-[0.2em] uppercase"
			>
				Join waitlist
			</p>
			<h2
				class="mb-6 font-(family-name:--font-display) text-3xl font-light"
			>
				Be among the first
			</h2>
			<p class="text-muted-foreground mb-10">
				We're launching soon. Enter your email for early access.
			</p>

			<form
				class="flex flex-col gap-3 sm:flex-row"
				onsubmit={(e) => e.preventDefault()}
			>
				<input
					type="email"
					bind:value={email}
					placeholder="your@email.com"
					class="bg-background border-border focus:border-foreground/40 flex-1 border px-4 py-3 text-sm transition-colors focus:outline-none"
				/>
				<button
					type="submit"
					class="bg-foreground text-background hover:bg-foreground/90 px-6 py-3 font-(family-name:--font-display) text-sm tracking-wide transition-colors"
				>
					Notify me
				</button>
			</form>
		</div>
	</section>

	<!-- Footer -->
	<footer class="border-border border-t px-6 py-16">
		<div
			class="mx-auto flex max-w-4xl flex-col items-center justify-between gap-6 md:flex-row"
		>
			<div class="font-(family-name:--font-display) text-lg">
				<span class="text-primary">neko</span>match
			</div>
			<div class="text-muted-foreground flex gap-8 text-sm">
				<a href="#" class="hover:text-foreground transition-colors">
					Privacy
				</a>
				<a href="#" class="hover:text-foreground transition-colors">
					Terms
				</a>
				<a href="#" class="hover:text-foreground transition-colors">
					Contact
				</a>
			</div>
			<p class="text-muted-foreground text-xs">
				Made with care for cats everywhere
			</p>
		</div>
	</footer>
</div>
