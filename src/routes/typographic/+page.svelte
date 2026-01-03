<script lang="ts">
	let email = $state('');
</script>

<div class="bg-background font-body text-foreground min-h-screen">
	<!-- Header -->
	<header class="border-border border-b px-8 py-6">
		<nav class="mx-auto flex max-w-6xl items-center justify-between">
			<span class="font-display text-2xl font-bold tracking-tight">
				Purrfect Match
			</span>
			<div
				class="font-body text-muted-foreground flex gap-8 text-sm tracking-wide"
			>
				<a
					href="#how"
					class="hover:text-foreground underline-offset-4 transition-all hover:underline"
				>
					How It Works
				</a>
				<a
					href="#stories"
					class="hover:text-foreground underline-offset-4 transition-all hover:underline"
				>
					Stories
				</a>
				<a
					href="#pricing"
					class="hover:text-foreground underline-offset-4 transition-all hover:underline"
				>
					Pricing
				</a>
			</div>
		</nav>
	</header>

	<!-- Hero -->
	<section class="mx-auto max-w-6xl px-8 py-24">
		<div class="grid gap-16 lg:grid-cols-[2fr_1fr]">
			<div>
				<p
					class="animate-reveal text-muted-foreground font-mono text-xs tracking-widest uppercase"
				>
					The Premier Feline Connection Service
				</p>
				<h1
					class="animate-reveal-delay-1 font-display mt-4 text-6xl leading-[1.1] font-bold tracking-tight lg:text-7xl"
				>
					Every Cat Deserves a <em class="text-secondary italic">
						Soulmate
					</em>
				</h1>
				<p
					class="animate-reveal-delay-2 text-muted-foreground mt-8 max-w-xl text-xl leading-relaxed"
				>
					Where discerning felines find their forever companions.
					Because love shouldn't be left to chance—even for cats.
				</p>
				<form class="animate-reveal-delay-3 mt-10 flex gap-4">
					<input
						type="email"
						bind:value={email}
						placeholder="Enter your email"
						class="border-border bg-muted text-foreground placeholder:text-muted-foreground focus:border-primary rounded-sm border px-6 py-4 focus:outline-none"
					/>
					<button
						type="submit"
						class="bg-foreground text-background hover:bg-primary rounded-sm px-8 py-4 font-semibold transition-all"
					>
						Join the Waitlist
					</button>
				</form>
			</div>
			<aside class="border-border border-l pl-8">
				<blockquote
					class="text-muted-foreground text-xl leading-relaxed italic"
				>
					"Finally, a dating service that understands feline
					sophistication."
				</blockquote>
				<p class="mt-4 font-mono text-xs tracking-widest uppercase">
					— Whiskers Monthly
				</p>
			</aside>
		</div>
	</section>

	<!-- Stats -->
	<section class="border-border bg-muted border-y">
		<div
			class="divide-border mx-auto grid max-w-6xl grid-cols-3 divide-x"
		>
			<div class="px-8 py-12 text-center">
				<span class="font-display text-5xl font-bold">47,000</span>
				<p
					class="text-muted-foreground mt-2 font-mono text-xs tracking-widest uppercase"
				>
					Matches Made
				</p>
			</div>
			<div class="px-8 py-12 text-center">
				<span class="font-display text-5xl font-bold">98%</span>
				<p
					class="text-muted-foreground mt-2 font-mono text-xs tracking-widest uppercase"
				>
					Satisfaction Rate
				</p>
			</div>
			<div class="px-8 py-12 text-center">
				<span class="font-display text-5xl font-bold">12</span>
				<p
					class="text-muted-foreground mt-2 font-mono text-xs tracking-widest uppercase"
				>
					Countries Served
				</p>
			</div>
		</div>
	</section>

	<!-- How It Works -->
	<section id="how" class="mx-auto max-w-6xl px-8 py-24">
		<p
			class="text-muted-foreground font-mono text-xs tracking-widest uppercase"
		>
			The Process
		</p>
		<h2 class="font-display mt-4 text-5xl font-bold tracking-tight">
			How <em class="text-secondary italic">Purrfect Match</em> Works
		</h2>

		<div class="mt-16 grid gap-12 lg:grid-cols-3">
			<article class="group">
				<span
					class="font-display text-border group-hover:text-secondary text-6xl font-bold transition-colors"
				>
					01
				</span>
				<h3 class="font-display mt-4 text-2xl font-semibold">
					Create a Profile
				</h3>
				<p class="text-muted-foreground mt-3 leading-relaxed">
					Share your cat's personality, preferences, and photo. Our
					algorithm considers everything from nap schedules to toy
					preferences.
				</p>
			</article>
			<article class="group">
				<span
					class="font-display text-border group-hover:text-secondary text-6xl font-bold transition-colors"
				>
					02
				</span>
				<h3 class="font-display mt-4 text-2xl font-semibold">
					Get Matched
				</h3>
				<p class="text-muted-foreground mt-3 leading-relaxed">
					Our sophisticated matching system pairs cats based on
					temperament, energy levels, and lifestyle compatibility.
				</p>
			</article>
			<article class="group">
				<span
					class="font-display text-border group-hover:text-secondary text-6xl font-bold transition-colors"
				>
					03
				</span>
				<h3 class="font-display mt-4 text-2xl font-semibold">
					Meet & Mingle
				</h3>
				<p class="text-muted-foreground mt-3 leading-relaxed">
					Schedule supervised playdates at partner locations or
					arrange video calls. Love awaits.
				</p>
			</article>
		</div>
	</section>

	<!-- Pullquote -->
	<section class="border-border bg-muted border-y px-8 py-20">
		<div class="mx-auto max-w-4xl text-center">
			<blockquote
				class="font-display text-4xl leading-relaxed font-medium italic lg:text-5xl"
			>
				"In a world of seven billion humans, your cat still managed to
				find their one true love."
			</blockquote>
			<p
				class="text-muted-foreground mt-8 font-mono text-sm tracking-widest uppercase"
			>
				Our Promise
			</p>
		</div>
	</section>

	<!-- Success Stories -->
	<section id="stories" class="mx-auto max-w-6xl px-8 py-24">
		<div class="grid gap-16 lg:grid-cols-[1fr_2fr]">
			<div>
				<p
					class="text-muted-foreground font-mono text-xs tracking-widest uppercase"
				>
					Love Stories
				</p>
				<h2
					class="font-display mt-4 text-5xl font-bold tracking-tight"
				>
					Tales of Connection
				</h2>
			</div>
			<div class="space-y-12">
				<article class="border-accent border-l-4 pl-6">
					<p class="text-muted-foreground text-lg leading-relaxed">
						"Mr. Fluffington was an introvert. He'd never shown
						interest in other cats. Then he met Princess Midnight
						through Purrfect Match. They now share a sunny window spot
						every afternoon."
					</p>
					<p class="mt-4 font-mono text-xs tracking-widest uppercase">
						— Sarah T., Cat Parent, Brooklyn
					</p>
				</article>
				<article class="border-accent border-l-4 pl-6">
					<p class="text-muted-foreground text-lg leading-relaxed">
						"I was skeptical. A dating app for cats? But watching
						Mochi and Tofu groom each other for the first time—I
						became a believer."
					</p>
					<p class="mt-4 font-mono text-xs tracking-widest uppercase">
						— David K., Cat Parent, Portland
					</p>
				</article>
			</div>
		</div>
	</section>

	<!-- Pricing -->
	<section
		id="pricing"
		class="border-border bg-muted border-t px-8 py-24"
	>
		<div class="mx-auto max-w-6xl">
			<p
				class="text-muted-foreground font-mono text-xs tracking-widest uppercase"
			>
				Membership
			</p>
			<h2 class="font-display mt-4 text-5xl font-bold tracking-tight">
				Simple, Fair Pricing
			</h2>

			<div class="mt-16 grid gap-8 lg:grid-cols-3">
				<article class="bg-background rounded-sm p-8">
					<h3 class="font-display text-2xl font-semibold">
						Curious Kitten
					</h3>
					<p class="text-muted-foreground mt-2">
						For cats just starting out
					</p>
					<p class="mt-6">
						<span class="font-display text-4xl font-bold">Free</span>
					</p>
					<ul class="text-muted-foreground mt-6 space-y-3 text-sm">
						<li>5 matches per month</li>
						<li>Basic profile</li>
						<li>Community access</li>
					</ul>
				</article>

				<article
					class="border-foreground bg-background rounded-sm border-2 p-8"
				>
					<h3 class="font-display text-2xl font-semibold">
						Social Cat
					</h3>
					<p class="text-muted-foreground mt-2">
						For serious seekers
					</p>
					<p class="mt-6">
						<span class="font-display text-4xl font-bold">$9</span>
						<span class="text-muted-foreground">/month</span>
					</p>
					<ul class="text-muted-foreground mt-6 space-y-3 text-sm">
						<li>Unlimited matches</li>
						<li>Advanced compatibility</li>
						<li>Video call dates</li>
						<li>Priority support</li>
					</ul>
				</article>

				<article class="bg-background rounded-sm p-8">
					<h3 class="font-display text-2xl font-semibold">Top Cat</h3>
					<p class="text-muted-foreground mt-2">
						The ultimate experience
					</p>
					<p class="mt-6">
						<span class="font-display text-4xl font-bold">$29</span>
						<span class="text-muted-foreground">/month</span>
					</p>
					<ul class="text-muted-foreground mt-6 space-y-3 text-sm">
						<li>Everything in Social</li>
						<li>Professional photoshoot</li>
						<li>Concierge matchmaking</li>
						<li>Exclusive events</li>
					</ul>
				</article>
			</div>
		</div>
	</section>

	<!-- Footer -->
	<footer class="border-border border-t px-8 py-12">
		<div class="mx-auto flex max-w-6xl items-center justify-between">
			<p
				class="text-muted-foreground font-mono text-xs tracking-widest uppercase"
			>
				Purrfect Match &copy; 2026
			</p>
			<div class="text-muted-foreground flex gap-6 text-sm">
				<a href="#" class="underline-offset-4 hover:underline"
					>Privacy</a
				>
				<a href="#" class="underline-offset-4 hover:underline"
					>Terms</a
				>
				<a href="#" class="underline-offset-4 hover:underline"
					>Contact</a
				>
			</div>
		</div>
	</footer>
</div>
