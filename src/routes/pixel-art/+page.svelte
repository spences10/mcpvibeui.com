<script lang="ts">
	let email = $state('');
</script>

<div class="bg-background text-foreground font-body min-h-screen">
	<!-- Header -->
	<header class="border-foreground bg-muted border-b-4">
		<div
			class="mx-auto flex max-w-6xl items-center justify-between px-4 py-4"
		>
			<div class="flex items-center gap-3">
				<div class="text-3xl">
					<span class="[image-rendering:pixelated]">
						<!-- Pixel cat icon -->
						<svg
							width="32"
							height="32"
							viewBox="0 0 16 16"
							class="inline-block"
						>
							<rect
								x="4"
								y="2"
								width="2"
								height="2"
								fill="currentColor"
							/>
							<rect
								x="10"
								y="2"
								width="2"
								height="2"
								fill="currentColor"
							/>
							<rect
								x="3"
								y="4"
								width="10"
								height="8"
								fill="currentColor"
							/>
							<rect x="5" y="6" width="2" height="2" fill="white" />
							<rect x="9" y="6" width="2" height="2" fill="white" />
							<rect x="7" y="9" width="2" height="1" fill="#FF6B9D" />
							<rect x="6" y="10" width="1" height="1" fill="white" />
							<rect x="9" y="10" width="1" height="1" fill="white" />
						</svg>
					</span>
				</div>
				<h1 class="font-display text-primary text-xs sm:text-sm">
					PURRFECT MATCH
				</h1>
			</div>
			<nav class="hidden gap-6 text-xl md:flex">
				<a
					href="#features"
					class="hover:text-primary transition-colors">Features</a
				>
				<a href="#how" class="hover:text-primary transition-colors">
					How It Works
				</a>
				<a href="#cats" class="hover:text-primary transition-colors">
					Meet Cats
				</a>
			</nav>
			<button
				class="border-foreground bg-primary text-primary-foreground font-display border-4 px-4 py-2 text-[10px] shadow-[4px_4px_0_0_#000] active:translate-x-1 active:translate-y-1 active:shadow-none"
			>
				LOGIN
			</button>
		</div>
	</header>

	<!-- Hero Section -->
	<section class="relative overflow-hidden px-4 py-16">
		<!-- Pixel decorations -->
		<div
			class="absolute top-10 left-10 animate-[float_3s_ease-in-out_infinite] text-4xl"
		>
			<svg
				width="24"
				height="24"
				viewBox="0 0 8 8"
				class="[image-rendering:pixelated]"
			>
				<rect x="3" y="0" width="2" height="2" fill="#FF6B9D" />
				<rect x="1" y="2" width="6" height="4" fill="#FF6B9D" />
				<rect x="0" y="3" width="8" height="2" fill="#FF6B9D" />
			</svg>
		</div>
		<div
			class="absolute top-20 right-20 animate-[float_4s_ease-in-out_infinite_0.5s] text-4xl"
		>
			<svg
				width="24"
				height="24"
				viewBox="0 0 8 8"
				class="[image-rendering:pixelated]"
			>
				<rect x="3" y="0" width="2" height="2" fill="#FF6B9D" />
				<rect x="1" y="2" width="6" height="4" fill="#FF6B9D" />
				<rect x="0" y="3" width="8" height="2" fill="#FF6B9D" />
			</svg>
		</div>

		<div class="mx-auto max-w-4xl text-center">
			<!-- Pixel cat mascot -->
			<div
				class="mb-8 animate-[pixel-bounce_1s_steps(4,end)_infinite]"
			>
				<svg
					width="128"
					height="128"
					viewBox="0 0 32 32"
					class="mx-auto [image-rendering:pixelated]"
				>
					<!-- Ears -->
					<rect x="6" y="4" width="4" height="4" fill="#FFA07A" />
					<rect x="22" y="4" width="4" height="4" fill="#FFA07A" />
					<!-- Inner ears -->
					<rect x="7" y="5" width="2" height="2" fill="#FFB6C1" />
					<rect x="23" y="5" width="2" height="2" fill="#FFB6C1" />
					<!-- Head -->
					<rect x="6" y="8" width="20" height="16" fill="#FFA07A" />
					<!-- Eyes -->
					<rect x="10" y="12" width="4" height="4" fill="white" />
					<rect x="18" y="12" width="4" height="4" fill="white" />
					<rect x="12" y="14" width="2" height="2" fill="#333" />
					<rect x="20" y="14" width="2" height="2" fill="#333" />
					<!-- Sparkle in eyes -->
					<rect x="11" y="13" width="1" height="1" fill="white" />
					<rect x="19" y="13" width="1" height="1" fill="white" />
					<!-- Nose -->
					<rect x="15" y="17" width="2" height="2" fill="#FF6B9D" />
					<!-- Mouth -->
					<rect x="13" y="19" width="2" height="1" fill="#333" />
					<rect x="17" y="19" width="2" height="1" fill="#333" />
					<rect x="14" y="20" width="1" height="1" fill="#333" />
					<rect x="17" y="20" width="1" height="1" fill="#333" />
					<!-- Whiskers -->
					<rect x="4" y="16" width="4" height="1" fill="#333" />
					<rect x="4" y="18" width="4" height="1" fill="#333" />
					<rect x="24" y="16" width="4" height="1" fill="#333" />
					<rect x="24" y="18" width="4" height="1" fill="#333" />
					<!-- Blush -->
					<rect x="8" y="17" width="2" height="2" fill="#FFB6C1" />
					<rect x="22" y="17" width="2" height="2" fill="#FFB6C1" />
				</svg>
			</div>

			<h2
				class="font-display mb-6 text-xl leading-relaxed sm:text-2xl md:text-3xl"
			>
				FIND YOUR CAT'S<br />
				<span class="text-primary">PURRFECT MATCH</span>
			</h2>

			<p
				class="text-muted-foreground mx-auto mb-8 max-w-2xl text-2xl sm:text-3xl"
			>
				The retro dating app where cats find love, one pixel at a
				time!
			</p>

			<!-- CTA Form -->
			<div
				class="bg-muted border-foreground mx-auto max-w-md border-4 p-6 shadow-[8px_8px_0_0_#000]"
			>
				<p class="font-display mb-4 text-[10px]">JOIN THE WAITLIST</p>
				<div class="flex flex-col gap-3 sm:flex-row">
					<input
						type="email"
						placeholder="Enter your email..."
						bind:value={email}
						class="border-foreground bg-background focus:border-primary flex-1 border-4 px-4 py-3 text-xl focus:outline-none"
					/>
					<button
						class="border-foreground bg-accent text-accent-foreground font-display hover:bg-success border-4 px-6 py-3 text-[10px] whitespace-nowrap shadow-[4px_4px_0_0_#000] transition-colors active:translate-x-1 active:translate-y-1 active:shadow-none"
					>
						SIGN UP
					</button>
				</div>
				<p class="text-muted-foreground mt-3 text-lg">
					Free for all cats. Humans pay $9.99/mo
				</p>
			</div>
		</div>
	</section>

	<!-- Features Section -->
	<section
		id="features"
		class="bg-muted border-foreground border-y-4 px-4 py-16"
	>
		<div class="mx-auto max-w-6xl">
			<h3 class="font-display mb-12 text-center text-lg sm:text-xl">
				<span class="text-secondary">8-BIT</span> FEATURES
			</h3>

			<div class="grid gap-8 md:grid-cols-3">
				<!-- Feature 1 -->
				<div
					class="bg-background border-foreground border-4 p-6 shadow-[4px_4px_0_0_#000]"
				>
					<div class="mb-4 text-5xl">
						<svg
							width="48"
							height="48"
							viewBox="0 0 16 16"
							class="[image-rendering:pixelated]"
						>
							<rect x="3" y="1" width="2" height="2" fill="#FF6B9D" />
							<rect
								x="11"
								y="1"
								width="2"
								height="2"
								fill="#FF6B9D"
							/>
							<rect
								x="1"
								y="3"
								width="14"
								height="10"
								fill="#FF6B9D"
							/>
							<rect
								x="0"
								y="5"
								width="16"
								height="6"
								fill="#FF6B9D"
							/>
						</svg>
					</div>
					<h4 class="font-display text-primary mb-3 text-xs">
						PAWSITIVE MATCHING
					</h4>
					<p class="text-muted-foreground text-xl">
						Our pixel-perfect algorithm matches cats based on nap
						preferences, treat tastes, and zoomie schedules.
					</p>
				</div>

				<!-- Feature 2 -->
				<div
					class="bg-background border-foreground border-4 p-6 shadow-[4px_4px_0_0_#000]"
				>
					<div class="mb-4 text-5xl">
						<svg
							width="48"
							height="48"
							viewBox="0 0 16 16"
							class="[image-rendering:pixelated]"
						>
							<rect
								x="2"
								y="2"
								width="12"
								height="12"
								fill="#6C5CE7"
							/>
							<rect x="4" y="4" width="3" height="3" fill="white" />
							<rect x="9" y="4" width="3" height="3" fill="white" />
							<rect x="5" y="5" width="1" height="1" fill="#333" />
							<rect x="10" y="5" width="1" height="1" fill="#333" />
							<rect x="6" y="9" width="4" height="2" fill="#333" />
						</svg>
					</div>
					<h4 class="font-display text-secondary mb-3 text-xs">
						MEOW MESSENGER
					</h4>
					<p class="text-muted-foreground text-xl">
						Send pixel art stickers, purrs, and hisses. Express
						yourself in glorious 8-bit style!
					</p>
				</div>

				<!-- Feature 3 -->
				<div
					class="bg-background border-foreground border-4 p-6 shadow-[4px_4px_0_0_#000]"
				>
					<div class="mb-4 text-5xl">
						<svg
							width="48"
							height="48"
							viewBox="0 0 16 16"
							class="[image-rendering:pixelated]"
						>
							<rect x="7" y="1" width="2" height="2" fill="#F9CA24" />
							<rect x="5" y="3" width="6" height="2" fill="#F9CA24" />
							<rect
								x="3"
								y="5"
								width="10"
								height="2"
								fill="#F9CA24"
							/>
							<rect
								x="1"
								y="7"
								width="14"
								height="2"
								fill="#F9CA24"
							/>
							<rect
								x="3"
								y="9"
								width="10"
								height="2"
								fill="#F9CA24"
							/>
							<rect
								x="5"
								y="11"
								width="6"
								height="2"
								fill="#F9CA24"
							/>
							<rect
								x="7"
								y="13"
								width="2"
								height="2"
								fill="#F9CA24"
							/>
						</svg>
					</div>
					<h4 class="font-display text-warning mb-3 text-xs">
						TREAT REWARDS
					</h4>
					<p class="text-muted-foreground text-xl">
						Earn pixel treats for daily logins. Trade them for premium
						catnip and exclusive accessories!
					</p>
				</div>
			</div>
		</div>
	</section>

	<!-- How It Works -->
	<section id="how" class="px-4 py-16">
		<div class="mx-auto max-w-4xl">
			<h3 class="font-display mb-12 text-center text-lg sm:text-xl">
				HOW IT <span class="text-accent">WORKS</span>
			</h3>

			<div class="space-y-8">
				<div class="flex items-start gap-6">
					<div
						class="border-foreground bg-primary text-primary-foreground font-display flex h-16 w-16 shrink-0 items-center justify-center border-4 text-sm shadow-[4px_4px_0_0_#000]"
					>
						1
					</div>
					<div>
						<h4 class="font-display mb-2 text-xs">
							CREATE YOUR MEOW-FILE
						</h4>
						<p class="text-muted-foreground text-xl">
							Upload your cat's cutest pixel portrait and list their
							favorite things (boxes, laser pointers, judging humans).
						</p>
					</div>
				</div>

				<div class="flex items-start gap-6">
					<div
						class="border-foreground bg-secondary text-secondary-foreground font-display flex h-16 w-16 shrink-0 items-center justify-center border-4 text-sm shadow-[4px_4px_0_0_#000]"
					>
						2
					</div>
					<div>
						<h4 class="font-display mb-2 text-xs">SWIPE WITH PAWS</h4>
						<p class="text-muted-foreground text-xl">
							Swipe right to boop, left to hiss. Our algorithm learns
							your cat's type faster than they knock things off
							tables.
						</p>
					</div>
				</div>

				<div class="flex items-start gap-6">
					<div
						class="border-foreground bg-accent text-accent-foreground font-display flex h-16 w-16 shrink-0 items-center justify-center border-4 text-sm shadow-[4px_4px_0_0_#000]"
					>
						3
					</div>
					<div>
						<h4 class="font-display mb-2 text-xs">
							ARRANGE A PLAYDATE
						</h4>
						<p class="text-muted-foreground text-xl">
							Match? Time for a virtual playdate! Share a sunbeam
							through video chat or meet at a local cat cafe.
						</p>
					</div>
				</div>
			</div>
		</div>
	</section>

	<!-- Meet Cats Section -->
	<section
		id="cats"
		class="bg-muted border-foreground border-y-4 px-4 py-16"
	>
		<div class="mx-auto max-w-6xl">
			<h3 class="font-display mb-12 text-center text-lg sm:text-xl">
				FEATURED <span class="text-primary">FURBALLS</span>
			</h3>

			<div class="grid gap-6 sm:grid-cols-2 lg:grid-cols-4">
				<!-- Cat Profile 1 -->
				<div
					class="bg-background border-foreground border-4 p-4 shadow-[4px_4px_0_0_#000]"
				>
					<div
						class="bg-muted border-foreground mb-4 flex aspect-square items-center justify-center border-4"
					>
						<svg
							width="80"
							height="80"
							viewBox="0 0 32 32"
							class="[image-rendering:pixelated]"
						>
							<rect x="6" y="4" width="4" height="4" fill="#808080" />
							<rect
								x="22"
								y="4"
								width="4"
								height="4"
								fill="#808080"
							/>
							<rect
								x="6"
								y="8"
								width="20"
								height="16"
								fill="#808080"
							/>
							<rect
								x="10"
								y="12"
								width="4"
								height="4"
								fill="#90EE90"
							/>
							<rect
								x="18"
								y="12"
								width="4"
								height="4"
								fill="#90EE90"
							/>
							<rect x="12" y="14" width="2" height="2" fill="#333" />
							<rect x="20" y="14" width="2" height="2" fill="#333" />
							<rect
								x="15"
								y="17"
								width="2"
								height="2"
								fill="#FFB6C1"
							/>
						</svg>
					</div>
					<h4 class="font-display text-primary text-[10px]">
						WHISKERS
					</h4>
					<p class="text-muted-foreground text-lg">3 years | Tabby</p>
					<p class="mt-2 text-xl">
						"Looking for someone to share my cardboard box empire"
					</p>
				</div>

				<!-- Cat Profile 2 -->
				<div
					class="bg-background border-foreground border-4 p-4 shadow-[4px_4px_0_0_#000]"
				>
					<div
						class="bg-muted border-foreground mb-4 flex aspect-square items-center justify-center border-4"
					>
						<svg
							width="80"
							height="80"
							viewBox="0 0 32 32"
							class="[image-rendering:pixelated]"
						>
							<rect x="6" y="4" width="4" height="4" fill="#000" />
							<rect x="22" y="4" width="4" height="4" fill="#000" />
							<rect x="6" y="8" width="20" height="16" fill="#000" />
							<rect
								x="10"
								y="12"
								width="4"
								height="4"
								fill="#FFD700"
							/>
							<rect
								x="18"
								y="12"
								width="4"
								height="4"
								fill="#FFD700"
							/>
							<rect x="12" y="14" width="2" height="2" fill="#333" />
							<rect x="20" y="14" width="2" height="2" fill="#333" />
							<rect
								x="15"
								y="17"
								width="2"
								height="2"
								fill="#FFB6C1"
							/>
						</svg>
					</div>
					<h4 class="font-display text-secondary text-[10px]">
						MIDNIGHT
					</h4>
					<p class="text-muted-foreground text-lg">
						5 years | Black Cat
					</p>
					<p class="mt-2 text-xl">
						"Professional napper seeking cuddle partner for 3am
						zoomies"
					</p>
				</div>

				<!-- Cat Profile 3 -->
				<div
					class="bg-background border-foreground border-4 p-4 shadow-[4px_4px_0_0_#000]"
				>
					<div
						class="bg-muted border-foreground mb-4 flex aspect-square items-center justify-center border-4"
					>
						<svg
							width="80"
							height="80"
							viewBox="0 0 32 32"
							class="[image-rendering:pixelated]"
						>
							<rect x="6" y="4" width="4" height="4" fill="#FFA500" />
							<rect
								x="22"
								y="4"
								width="4"
								height="4"
								fill="#FFA500"
							/>
							<rect
								x="6"
								y="8"
								width="20"
								height="16"
								fill="#FFA500"
							/>
							<rect x="10" y="8" width="4" height="8" fill="white" />
							<rect x="18" y="8" width="4" height="8" fill="white" />
							<rect
								x="10"
								y="12"
								width="4"
								height="4"
								fill="#87CEEB"
							/>
							<rect
								x="18"
								y="12"
								width="4"
								height="4"
								fill="#87CEEB"
							/>
							<rect x="12" y="14" width="2" height="2" fill="#333" />
							<rect x="20" y="14" width="2" height="2" fill="#333" />
							<rect
								x="15"
								y="17"
								width="2"
								height="2"
								fill="#FFB6C1"
							/>
						</svg>
					</div>
					<h4 class="font-display text-accent text-[10px]">MOCHI</h4>
					<p class="text-muted-foreground text-lg">
						2 years | Calico
					</p>
					<p class="mt-2 text-xl">
						"Treat enthusiast. Will knock things off tables for
						attention"
					</p>
				</div>

				<!-- Cat Profile 4 -->
				<div
					class="bg-background border-foreground border-4 p-4 shadow-[4px_4px_0_0_#000]"
				>
					<div
						class="bg-muted border-foreground mb-4 flex aspect-square items-center justify-center border-4"
					>
						<svg
							width="80"
							height="80"
							viewBox="0 0 32 32"
							class="[image-rendering:pixelated]"
						>
							<rect x="6" y="4" width="4" height="4" fill="white" />
							<rect x="22" y="4" width="4" height="4" fill="white" />
							<rect x="7" y="5" width="2" height="2" fill="#FFB6C1" />
							<rect
								x="23"
								y="5"
								width="2"
								height="2"
								fill="#FFB6C1"
							/>
							<rect x="6" y="8" width="20" height="16" fill="white" />
							<rect
								x="10"
								y="12"
								width="4"
								height="4"
								fill="#ADD8E6"
							/>
							<rect
								x="18"
								y="12"
								width="4"
								height="4"
								fill="#ADD8E6"
							/>
							<rect x="12" y="14" width="2" height="2" fill="#333" />
							<rect x="20" y="14" width="2" height="2" fill="#333" />
							<rect
								x="15"
								y="17"
								width="2"
								height="2"
								fill="#FFB6C1"
							/>
							<rect
								x="8"
								y="16"
								width="2"
								height="2"
								fill="#FFB6C1"
							/>
							<rect
								x="22"
								y="16"
								width="2"
								height="2"
								fill="#FFB6C1"
							/>
						</svg>
					</div>
					<h4 class="font-display text-pink text-[10px]">SNOWBALL</h4>
					<p class="text-muted-foreground text-lg">
						4 years | Persian
					</p>
					<p class="mt-2 text-xl">
						"Fluffy royalty. Must appreciate fine things (me)"
					</p>
				</div>
			</div>
		</div>
	</section>

	<!-- Stats Section -->
	<section class="px-4 py-16">
		<div class="mx-auto max-w-4xl">
			<div class="grid grid-cols-2 gap-6 text-center md:grid-cols-4">
				<div>
					<p class="font-display text-primary text-2xl sm:text-3xl">
						50K+
					</p>
					<p class="text-muted-foreground text-xl">Happy Cats</p>
				</div>
				<div>
					<p class="font-display text-secondary text-2xl sm:text-3xl">
						10K+
					</p>
					<p class="text-muted-foreground text-xl">Matches Made</p>
				</div>
				<div>
					<p class="font-display text-accent text-2xl sm:text-3xl">
						99%
					</p>
					<p class="text-muted-foreground text-xl">Purr Rate</p>
				</div>
				<div>
					<p class="font-display text-warning text-2xl sm:text-3xl">
						1M+
					</p>
					<p class="text-muted-foreground text-xl">Treats Given</p>
				</div>
			</div>
		</div>
	</section>

	<!-- Final CTA -->
	<section
		class="bg-primary text-primary-foreground border-foreground border-y-4 px-4 py-16"
	>
		<div class="mx-auto max-w-2xl text-center">
			<h3 class="font-display mb-6 text-lg sm:text-xl">
				READY TO FIND LOVE?
			</h3>
			<p class="mb-8 text-2xl opacity-90">
				Join thousands of cats already swiping their way to happiness!
			</p>
			<button
				class="border-foreground bg-background text-foreground font-display hover:bg-muted border-4 px-8 py-4 text-sm shadow-[4px_4px_0_0_#000] transition-colors active:translate-x-1 active:translate-y-1 active:shadow-none"
			>
				START MATCHING
			</button>
		</div>
	</section>

	<!-- Footer -->
	<footer class="border-foreground border-t-4 px-4 py-8">
		<div class="mx-auto max-w-6xl">
			<div
				class="flex flex-col items-center justify-between gap-6 md:flex-row"
			>
				<div class="flex items-center gap-3">
					<svg
						width="24"
						height="24"
						viewBox="0 0 16 16"
						class="[image-rendering:pixelated]"
					>
						<rect
							x="4"
							y="2"
							width="2"
							height="2"
							fill="currentColor"
						/>
						<rect
							x="10"
							y="2"
							width="2"
							height="2"
							fill="currentColor"
						/>
						<rect
							x="3"
							y="4"
							width="10"
							height="8"
							fill="currentColor"
						/>
						<rect x="5" y="6" width="2" height="2" fill="white" />
						<rect x="9" y="6" width="2" height="2" fill="white" />
						<rect x="7" y="9" width="2" height="1" fill="#FF6B9D" />
					</svg>
					<span class="font-display text-[10px]">PURRFECT MATCH</span>
				</div>
				<nav class="flex gap-6 text-xl">
					<a href="#" class="hover:text-primary">About</a>
					<a href="#" class="hover:text-primary">Privacy</a>
					<a href="#" class="hover:text-primary">Terms</a>
					<a href="#" class="hover:text-primary">Contact</a>
				</nav>
				<p class="text-muted-foreground text-lg">
					Made with <span
						class="text-primary animate-[blink_1s_steps(2,end)_infinite]"
						>&lt;3</span
					> for cats
				</p>
			</div>
		</div>
	</footer>
</div>
