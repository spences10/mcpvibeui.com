<script lang="ts">
	let email = $state('');
</script>

<div class="relative min-h-screen overflow-hidden">
	<!-- Background grid -->
	<div class="cyber-grid fixed inset-0"></div>

	<!-- Floating neon shapes -->
	<div
		class="bg-primary/20 glow-primary absolute -top-20 -left-20 h-40 w-40 animate-pulse rounded-full blur-3xl"
	></div>
	<div
		class="bg-secondary/20 glow-secondary absolute top-1/2 -right-20 h-60 w-60 animate-pulse rounded-full blur-3xl"
	></div>
	<div
		class="bg-accent/20 glow-accent absolute -bottom-20 left-1/3 h-40 w-40 animate-pulse rounded-full blur-3xl"
	></div>

	<!-- Main content -->
	<div class="relative z-10">
		<!-- Nav -->
		<nav
			class="border-primary/20 flex items-center justify-between border-b px-6 py-4"
		>
			<div class="flex items-center gap-2">
				<span class="text-3xl">🐱</span>
				<span
					class="text-glow-primary text-primary font-display text-xl font-bold"
				>
					NEKO.LINK
				</span>
			</div>
			<div class="flex gap-4">
				<button
					class="bg-base-200 hover:bg-base-300 rounded-(--radius-field) px-4 py-2 transition"
					>Login</button
				>
				<button
					class="glow-primary bg-primary text-primary-content rounded-(--radius-field) px-4 py-2 font-semibold transition hover:brightness-110"
					>Sign Up</button
				>
			</div>
		</nav>

		<!-- Hero -->
		<section class="scanlines relative px-6 py-24 text-center">
			<h1
				class="text-glow-primary text-primary font-display mb-6 text-5xl font-black tracking-wider md:text-7xl"
			>
				FIND YOUR<br />
				<span class="text-glow-secondary text-secondary"
					>PURRFECT</span
				> MATCH
			</h1>
			<p class="text-base-content/80 mx-auto mb-10 max-w-xl text-lg">
				The future of feline connections is here. Neural-linked
				matching algorithms find your cat's soulmate in the neon-lit
				streets of tomorrow.
			</p>

			<!-- Email signup -->
			<div
				class="bg-base-200/80 border-primary/30 glow-primary mx-auto flex max-w-md flex-col gap-3 rounded-(--radius-box) border p-4 backdrop-blur sm:flex-row"
			>
				<input
					type="email"
					bind:value={email}
					placeholder="Enter your email..."
					class="bg-base-300 text-base-content placeholder:text-base-content/50 focus:ring-primary flex-1 rounded-(--radius-field) border-none px-4 py-3 outline-none focus:ring-2"
				/>
				<button
					class="glow-secondary bg-secondary text-secondary-content rounded-(--radius-field) px-6 py-3 font-semibold transition hover:brightness-110"
				>
					JOIN WAITLIST
				</button>
			</div>

			<p class="text-base-content/50 mt-4 text-sm">
				🔒 Your data is encrypted with quantum protocols
			</p>
		</section>

		<!-- Features -->
		<section class="px-6 py-16">
			<h2
				class="text-glow-accent text-accent font-display mb-12 text-center text-3xl font-bold"
			>
				[ FEATURES ]
			</h2>
			<div class="mx-auto grid max-w-5xl gap-6 md:grid-cols-3">
				<div
					class="bg-base-200/60 border-primary/20 hover:border-primary/50 hover:glow-primary rounded-(--radius-box) border p-6 backdrop-blur transition"
				>
					<div class="mb-4 text-4xl">🧠</div>
					<h3
						class="text-primary font-display mb-2 text-lg font-bold"
					>
						NEURAL MATCHING
					</h3>
					<p class="text-base-content/70 text-sm">
						AI analyzes 10,000+ behavioral patterns to find compatible
						cats in your megacity sector.
					</p>
				</div>
				<div
					class="bg-base-200/60 border-secondary/20 hover:border-secondary/50 hover:glow-secondary rounded-(--radius-box) border p-6 backdrop-blur transition"
				>
					<div class="mb-4 text-4xl">🌐</div>
					<h3
						class="text-secondary font-display mb-2 text-lg font-bold"
					>
						HOLO-PROFILES
					</h3>
					<p class="text-base-content/70 text-sm">
						3D holographic cat profiles let you see potential matches
						in augmented reality before meeting.
					</p>
				</div>
				<div
					class="bg-base-200/60 border-accent/20 hover:border-accent/50 hover:glow-accent rounded-(--radius-box) border p-6 backdrop-blur transition"
				>
					<div class="mb-4 text-4xl">🔐</div>
					<h3 class="text-accent font-display mb-2 text-lg font-bold">
						SECURE MEETS
					</h3>
					<p class="text-base-content/70 text-sm">
						Verified safe zones and drone-monitored meetups protect
						your precious fluffball.
					</p>
				</div>
			</div>
		</section>

		<!-- Stats -->
		<section
			class="border-primary/20 bg-base-200/40 border-y px-6 py-16"
		>
			<div
				class="mx-auto grid max-w-4xl grid-cols-2 gap-8 md:grid-cols-4"
			>
				<div class="text-center">
					<div
						class="text-glow-primary text-primary font-display text-4xl font-black"
					>
						2.4M
					</div>
					<div class="text-base-content/60 text-sm">CATS ONLINE</div>
				</div>
				<div class="text-center">
					<div
						class="text-glow-secondary text-secondary font-display text-4xl font-black"
					>
						847K
					</div>
					<div class="text-base-content/60 text-sm">MATCHES MADE</div>
				</div>
				<div class="text-center">
					<div
						class="text-glow-accent text-accent font-display text-4xl font-black"
					>
						99.7%
					</div>
					<div class="text-base-content/60 text-sm">
						COMPATIBILITY
					</div>
				</div>
				<div class="text-center">
					<div
						class="text-glow-primary text-primary font-display text-4xl font-black"
					>
						24/7
					</div>
					<div class="text-base-content/60 text-sm">UPTIME</div>
				</div>
			</div>
		</section>

		<!-- CTA -->
		<section class="px-6 py-24 text-center">
			<h2
				class="text-glow-secondary text-secondary font-display mb-6 text-4xl font-bold"
			>
				READY TO CONNECT?
			</h2>
			<p class="text-base-content/70 mx-auto mb-8 max-w-lg">
				Join the revolution. Let your cat find love in the digital
				underground.
			</p>
			<button
				class="glow-primary bg-primary text-primary-content font-display rounded-(--radius-field) px-8 py-4 text-lg font-bold transition hover:brightness-110"
			>
				DOWNLOAD BETA
			</button>
		</section>

		<!-- Footer -->
		<footer
			class="border-primary/20 text-base-content/50 border-t px-6 py-8 text-center text-sm"
		>
			<div class="mb-4 flex justify-center gap-6">
				<a href="#" class="hover:text-primary transition">Terms</a>
				<a href="#" class="hover:text-primary transition">Privacy</a>
				<a href="#" class="hover:text-primary transition">Support</a>
			</div>
			<p>© 2077 NEKO.LINK — All rights reserved in this timeline</p>
		</footer>
	</div>
</div>
