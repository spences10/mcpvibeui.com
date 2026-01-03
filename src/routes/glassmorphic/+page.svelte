<script lang="ts">
	let email = $state('');
</script>

<div
	class="relative min-h-screen overflow-hidden bg-linear-to-br from-purple-400 via-pink-300 to-orange-200"
>
	<!-- Floating orbs background -->
	<div class="pointer-events-none absolute inset-0 overflow-hidden">
		<div
			class="absolute top-20 left-20 h-72 w-72 animate-[float_6s_ease-in-out_infinite] rounded-full bg-pink-300/40 blur-3xl"
		></div>
		<div
			class="absolute top-40 right-32 h-96 w-96 animate-[float_8s_ease-in-out_infinite_1s] rounded-full bg-purple-300/40 blur-3xl"
		></div>
		<div
			class="absolute bottom-20 left-1/3 h-80 w-80 animate-[float_7s_ease-in-out_infinite_0.5s] rounded-full bg-orange-200/40 blur-3xl"
		></div>
	</div>

	<!-- Nav -->
	<nav
		class="relative z-10 flex items-center justify-between px-8 py-6"
	>
		<div class="flex items-center gap-2">
			<span class="text-3xl">🐱</span>
			<span class="text-foreground text-2xl font-bold">PurrMatch</span
			>
		</div>
		<div class="hidden items-center gap-8 md:flex">
			<a
				href="#features"
				class="text-foreground/80 hover:text-foreground transition-colors"
				>Features</a
			>
			<a
				href="#how"
				class="text-foreground/80 hover:text-foreground transition-colors"
				>How it Works</a
			>
			<a
				href="#pricing"
				class="text-foreground/80 hover:text-foreground transition-colors"
				>Pricing</a
			>
		</div>
		<button
			class="text-foreground rounded-lg border border-white/30 bg-white/20 px-6 py-2 backdrop-blur-md transition-all hover:bg-white/30"
		>
			Sign In
		</button>
	</nav>

	<!-- Hero -->
	<section class="relative z-10 mx-auto max-w-6xl px-8 pt-16 pb-24">
		<div class="grid items-center gap-12 md:grid-cols-2">
			<div>
				<h1
					class="text-foreground mb-6 text-5xl leading-tight font-bold md:text-6xl"
				>
					Find Your Cat's
					<span
						class="bg-linear-to-r from-purple-600 to-pink-500 bg-clip-text text-transparent"
					>
						Purrfect Match
					</span>
				</h1>
				<p class="text-muted-foreground mb-8 text-lg">
					The premier dating app for cats. Help your feline friend
					find companionship, playmates, or their soulmate.
				</p>
				<div class="flex flex-wrap gap-4">
					<button
						class="bg-primary text-primary-foreground animate-[pulse-glow_2s_ease-in-out_infinite] rounded-lg px-8 py-4 font-semibold shadow-lg transition-all hover:opacity-90"
					>
						Get Started Free
					</button>
					<button
						class="text-foreground rounded-lg border border-white/30 bg-white/20 px-8 py-4 font-semibold backdrop-blur-md transition-all hover:bg-white/30"
					>
						Watch Demo
					</button>
				</div>
			</div>

			<!-- Glass card with cat profiles -->
			<div
				class="rounded-2xl border border-white/25 bg-white/15 p-6 shadow-[0_8px_32px_rgba(31,38,135,0.15)] backdrop-blur-xl"
			>
				<div class="mb-4 flex items-center gap-3">
					<div class="h-3 w-3 rounded-full bg-red-400"></div>
					<div class="h-3 w-3 rounded-full bg-yellow-400"></div>
					<div class="h-3 w-3 rounded-full bg-green-400"></div>
				</div>
				<div class="space-y-4">
					<div
						class="flex cursor-pointer items-center gap-4 rounded-xl border border-white/20 bg-white/20 p-4 backdrop-blur-md transition-all hover:bg-white/30"
					>
						<div
							class="flex h-16 w-16 items-center justify-center rounded-full bg-linear-to-br from-orange-300 to-orange-400 text-2xl"
						>
							🐈
						</div>
						<div class="flex-1">
							<div class="text-foreground font-semibold">
								Whiskers
							</div>
							<div class="text-muted-foreground text-sm">
								3 years old - Tabby
							</div>
						</div>
						<span class="text-2xl text-pink-500">💕</span>
					</div>
					<div
						class="flex cursor-pointer items-center gap-4 rounded-xl border border-white/20 bg-white/20 p-4 backdrop-blur-md transition-all hover:bg-white/30"
					>
						<div
							class="flex h-16 w-16 items-center justify-center rounded-full bg-linear-to-br from-gray-300 to-gray-400 text-2xl"
						>
							🐱
						</div>
						<div class="flex-1">
							<div class="text-foreground font-semibold">Luna</div>
							<div class="text-muted-foreground text-sm">
								2 years old - Persian
							</div>
						</div>
						<span class="text-2xl text-pink-500">💕</span>
					</div>
					<div
						class="flex cursor-pointer items-center gap-4 rounded-xl border border-white/20 bg-white/20 p-4 backdrop-blur-md transition-all hover:bg-white/30"
					>
						<div
							class="flex h-16 w-16 items-center justify-center rounded-full bg-linear-to-br from-amber-200 to-amber-300 text-2xl"
						>
							😺
						</div>
						<div class="flex-1">
							<div class="text-foreground font-semibold">Mochi</div>
							<div class="text-muted-foreground text-sm">
								1 year old - Siamese
							</div>
						</div>
						<span class="text-2xl text-pink-500">💕</span>
					</div>
				</div>
			</div>
		</div>
	</section>

	<!-- Features -->
	<section
		id="features"
		class="relative z-10 mx-auto max-w-6xl px-8 py-20"
	>
		<h2
			class="text-foreground mb-4 text-center text-3xl font-bold md:text-4xl"
		>
			Why Cats Love Us
		</h2>
		<p
			class="text-muted-foreground mx-auto mb-12 max-w-2xl text-center"
		>
			Designed by cat lovers, for cat lovers. Features your feline
			will actually use.
		</p>

		<div class="grid gap-6 md:grid-cols-3">
			<div
				class="rounded-2xl border border-white/25 bg-white/15 p-8 shadow-[0_8px_32px_rgba(31,38,135,0.15)] backdrop-blur-xl transition-all hover:bg-white/20"
			>
				<div
					class="mb-4 flex h-14 w-14 items-center justify-center rounded-xl bg-purple-500/20 text-3xl"
				>
					🎯
				</div>
				<h3 class="text-foreground mb-2 text-xl font-semibold">
					Smart Matching
				</h3>
				<p class="text-muted-foreground">
					AI-powered algorithm that considers personality, breed
					compatibility, and play styles.
				</p>
			</div>

			<div
				class="rounded-2xl border border-white/25 bg-white/15 p-8 shadow-[0_8px_32px_rgba(31,38,135,0.15)] backdrop-blur-xl transition-all hover:bg-white/20"
			>
				<div
					class="mb-4 flex h-14 w-14 items-center justify-center rounded-xl bg-pink-500/20 text-3xl"
				>
					📍
				</div>
				<h3 class="text-foreground mb-2 text-xl font-semibold">
					Local Meetups
				</h3>
				<p class="text-muted-foreground">
					Find cats in your neighborhood for supervised playdates and
					socialization.
				</p>
			</div>

			<div
				class="rounded-2xl border border-white/25 bg-white/15 p-8 shadow-[0_8px_32px_rgba(31,38,135,0.15)] backdrop-blur-xl transition-all hover:bg-white/20"
			>
				<div
					class="mb-4 flex h-14 w-14 items-center justify-center rounded-xl bg-orange-500/20 text-3xl"
				>
					🛡️
				</div>
				<h3 class="text-foreground mb-2 text-xl font-semibold">
					Verified Profiles
				</h3>
				<p class="text-muted-foreground">
					All cats are vet-verified for health and vaccination status.
					Safety first!
				</p>
			</div>
		</div>
	</section>

	<!-- Stats -->
	<section class="relative z-10 mx-auto max-w-6xl px-8 py-16">
		<div
			class="rounded-3xl border border-white/20 bg-white/10 p-8 backdrop-blur-xl md:p-12"
		>
			<div class="grid grid-cols-2 gap-8 text-center md:grid-cols-4">
				<div>
					<div class="text-foreground text-4xl font-bold md:text-5xl">
						50K+
					</div>
					<div class="text-muted-foreground mt-1">Happy Cats</div>
				</div>
				<div>
					<div class="text-foreground text-4xl font-bold md:text-5xl">
						12K+
					</div>
					<div class="text-muted-foreground mt-1">Matches Made</div>
				</div>
				<div>
					<div class="text-foreground text-4xl font-bold md:text-5xl">
						98%
					</div>
					<div class="text-muted-foreground mt-1">Satisfaction</div>
				</div>
				<div>
					<div class="text-foreground text-4xl font-bold md:text-5xl">
						24/7
					</div>
					<div class="text-muted-foreground mt-1">Support</div>
				</div>
			</div>
		</div>
	</section>

	<!-- CTA -->
	<section
		class="relative z-10 mx-auto max-w-4xl px-8 py-20 text-center"
	>
		<h2 class="text-foreground mb-4 text-3xl font-bold md:text-4xl">
			Ready to Find Love?
		</h2>
		<p class="text-muted-foreground mb-8">
			Join thousands of cats already finding their perfect companions.
		</p>

		<div
			class="mx-auto max-w-md rounded-2xl border border-white/25 bg-white/15 p-8 shadow-[0_8px_32px_rgba(31,38,135,0.15)] backdrop-blur-xl"
		>
			<form
				class="flex flex-col gap-4"
				onsubmit={(e) => e.preventDefault()}
			>
				<input
					type="email"
					placeholder="Enter your email"
					bind:value={email}
					class="text-foreground placeholder:text-muted-foreground focus:ring-primary/50 rounded-lg border border-white/30 bg-white/30 px-4 py-3 backdrop-blur-md focus:ring-2 focus:outline-none"
				/>
				<button
					type="submit"
					class="bg-primary text-primary-foreground rounded-lg px-6 py-3 font-semibold transition-all hover:opacity-90"
				>
					Start Matching
				</button>
			</form>
			<p class="text-muted-foreground mt-4 text-sm">
				Free to join. No credit card required.
			</p>
		</div>
	</section>

	<!-- Footer -->
	<footer class="relative z-10 border-t border-white/20 px-8 py-8">
		<div
			class="mx-auto flex max-w-6xl flex-col items-center justify-between gap-4 md:flex-row"
		>
			<div class="flex items-center gap-2">
				<span class="text-2xl">🐱</span>
				<span class="text-foreground font-bold">PurrMatch</span>
			</div>
			<p class="text-muted-foreground text-sm">
				Made with 💕 for cats everywhere
			</p>
		</div>
	</footer>
</div>
