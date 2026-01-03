<script lang="ts">
	let email = $state('');
</script>

<div class="bg-background text-foreground min-h-screen">
	<!-- Hazard stripe header -->
	<div
		class="h-4 bg-[repeating-linear-gradient(45deg,var(--color-warning),var(--color-warning)_10px,var(--color-foreground)_10px,var(--color-foreground)_20px)]"
	></div>

	<!-- Navigation -->
	<nav class="border-secondary bg-muted border-b-2 px-6 py-4">
		<div class="mx-auto flex max-w-6xl items-center justify-between">
			<div class="flex items-center gap-3">
				<div
					class="border-secondary bg-warning flex h-12 w-12 items-center justify-center rounded border-2 text-2xl"
				>
					🐱
				</div>
				<span
					class="font-(family-name:--font-display) text-3xl tracking-wide"
				>
					PAWMATCH INDUSTRIES
				</span>
			</div>
			<div class="flex gap-6 text-sm tracking-wider uppercase">
				<a href="#features" class="hover:text-primary transition">
					Systems
				</a>
				<a href="#testimonials" class="hover:text-primary transition">
					Reports
				</a>
				<a href="#pricing" class="hover:text-primary transition">
					Protocols
				</a>
				<button
					class="border-secondary bg-primary text-primary-foreground hover:bg-primary/80 rounded border-2 px-4 py-2 font-bold transition active:scale-95"
				>
					[ACCESS PORTAL]
				</button>
			</div>
		</div>
	</nav>

	<!-- Hero Section -->
	<section
		class="border-secondary relative overflow-hidden border-b-2 px-6 py-24"
	>
		<div
			class="pointer-events-none absolute inset-0 bg-[radial-gradient(circle,rgba(0,0,0,0.1)_1px,transparent_1px)] bg-size-[20px_20px]"
		></div>
		<div class="relative mx-auto max-w-6xl">
			<div class="grid items-center gap-12 lg:grid-cols-2">
				<div>
					<div
						class="border-warning bg-warning/20 mb-4 inline-block rounded border-2 px-3 py-1 text-xs tracking-widest uppercase"
					>
						⚠ SYSTEM ACTIVE
					</div>
					<h1
						class="font-(family-name:--font-display) text-6xl leading-none lg:text-8xl"
					>
						INDUSTRIAL<br />GRADE<br />CAT MATCHING
					</h1>
					<p class="text-muted-foreground mt-6 max-w-lg text-lg">
						Heavy-duty feline compatibility protocols. Built for
						serious cat owners who demand precision-engineered
						connections.
					</p>
					<div class="mt-8 flex gap-4">
						<button
							class="border-secondary bg-primary text-primary-foreground hover:bg-primary/80 rounded border-2 px-8 py-4 font-(family-name:--font-display) text-xl tracking-wide transition active:scale-95"
						>
							INITIATE MATCH SEQUENCE
						</button>
						<button
							class="border-secondary bg-muted hover:bg-border rounded border-2 px-8 py-4 font-(family-name:--font-display) text-xl tracking-wide transition active:scale-95"
						>
							VIEW SPECS
						</button>
					</div>
				</div>
				<div class="relative">
					<div
						class="border-secondary bg-muted rounded border-2 p-8 shadow-lg"
					>
						<div
							class="mb-4 flex items-center gap-2 text-xs tracking-wider uppercase"
						>
							<span
								class="bg-success inline-block h-3 w-3 animate-pulse rounded-full"
							></span>
							UNIT STATUS: ONLINE
						</div>
						<div
							class="border-border bg-background aspect-square rounded border-2 p-4"
						>
							<div
								class="flex h-full flex-col items-center justify-center text-center"
							>
								<div class="mb-4 text-8xl">😺</div>
								<div
									class="font-(family-name:--font-display) text-2xl"
								>
									UNIT #4827
								</div>
								<div class="text-muted-foreground text-sm">
									MAINE COON | 3 YRS | 18 LBS
								</div>
								<div class="mt-4 flex gap-2">
									<span
										class="bg-secondary text-secondary-foreground rounded px-2 py-1 text-xs"
									>
										PLAYFUL
									</span>
									<span
										class="bg-secondary text-secondary-foreground rounded px-2 py-1 text-xs"
									>
										CERTIFIED
									</span>
									<span
										class="bg-warning text-primary-foreground rounded px-2 py-1 text-xs"
									>
										98% MATCH
									</span>
								</div>
							</div>
						</div>
					</div>
					<div
						class="border-secondary absolute -right-4 -bottom-4 h-24 w-24 animate-[machinery_4s_linear_infinite] rounded-full border-4 border-dashed"
					></div>
				</div>
			</div>
		</div>
	</section>

	<!-- Stats Section -->
	<section
		class="border-secondary bg-secondary text-secondary-foreground border-b-2 px-6 py-12"
	>
		<div
			class="mx-auto grid max-w-6xl grid-cols-2 gap-8 lg:grid-cols-4"
		>
			{#each [{ num: '47,892', label: 'ACTIVE UNITS' }, { num: '12,456', label: 'MATCHES MADE' }, { num: '99.7%', label: 'SUCCESS RATE' }, { num: '24/7', label: 'UPTIME' }] as stat}
				<div class="text-center">
					<div class="font-(family-name:--font-display) text-5xl">
						{stat.num}
					</div>
					<div class="mt-2 text-sm tracking-wider opacity-80">
						{stat.label}
					</div>
				</div>
			{/each}
		</div>
	</section>

	<!-- Features Section -->
	<section
		id="features"
		class="border-secondary border-b-2 px-6 py-24"
	>
		<div class="mx-auto max-w-6xl">
			<div class="mb-16 text-center">
				<h2 class="font-(family-name:--font-display) text-5xl">
					OPERATIONAL SYSTEMS
				</h2>
				<p class="text-muted-foreground mt-4">
					Military-spec matching technology
				</p>
			</div>
			<div class="grid gap-8 md:grid-cols-3">
				{#each [{ icon: '⚙️', title: 'COMPATIBILITY ENGINE', desc: 'Advanced algorithms analyze 47 distinct feline parameters for optimal pairing.' }, { icon: '📊', title: 'BEHAVIORAL ANALYTICS', desc: 'Real-time monitoring of play patterns, sleep cycles, and treat preferences.' }, { icon: '🔒', title: 'SECURE PROTOCOLS', desc: 'End-to-end encrypted communication between verified cat owners.' }, { icon: '📍', title: 'LOCATION MATRIX', desc: 'Geo-targeted matching within your designated operational zone.' }, { icon: '🏷️', title: 'CERTIFICATION SYSTEM', desc: 'All units verified through our rigorous inspection process.' }, { icon: '📡', title: 'LIVE MONITORING', desc: '24/7 support team ready to assist with any matching anomalies.' }] as feature}
					<div
						class="border-secondary bg-muted hover:border-primary rounded border-2 p-6 transition hover:shadow-lg"
					>
						<div
							class="border-border bg-background mb-4 flex h-16 w-16 items-center justify-center rounded border-2 text-3xl"
						>
							{feature.icon}
						</div>
						<h3 class="font-(family-name:--font-display) text-xl">
							{feature.title}
						</h3>
						<p class="text-muted-foreground mt-2 text-sm">
							{feature.desc}
						</p>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- Testimonials -->
	<section
		id="testimonials"
		class="border-secondary bg-muted border-b-2 px-6 py-24"
	>
		<div class="mx-auto max-w-6xl">
			<h2
				class="mb-16 text-center font-(family-name:--font-display) text-5xl"
			>
				FIELD REPORTS
			</h2>
			<div class="grid gap-8 md:grid-cols-2">
				{#each [{ text: 'The matching protocol exceeded all expectations. Unit Whiskers found her perfect companion within 48 hours of system deployment.', author: 'OPERATOR J. WILSON', unit: 'UNIT #2847' }, { text: 'Industrial-grade reliability. Zero downtime. My cats have never been happier. This is the future of feline compatibility.', author: 'OPERATOR M. CHEN', unit: 'UNIT #9156' }] as testimonial}
					<div
						class="border-secondary bg-background rounded border-2 p-8"
					>
						<p class="mb-6 text-lg italic">"{testimonial.text}"</p>
						<div class="flex items-center gap-4">
							<div
								class="bg-secondary flex h-12 w-12 items-center justify-center rounded text-xl"
							>
								👤
							</div>
							<div>
								<div class="font-bold">{testimonial.author}</div>
								<div class="text-muted-foreground text-sm">
									{testimonial.unit}
								</div>
							</div>
						</div>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- Pricing -->
	<section
		id="pricing"
		class="border-secondary border-b-2 px-6 py-24"
	>
		<div class="mx-auto max-w-6xl">
			<h2
				class="mb-16 text-center font-(family-name:--font-display) text-5xl"
			>
				ACCESS PROTOCOLS
			</h2>
			<div class="grid gap-8 md:grid-cols-3">
				{#each [{ name: 'BASIC', price: '$0', period: '/MONTH', features: ['5 Match Requests', 'Standard Filters', 'Email Support', 'Basic Analytics'], highlighted: false }, { name: 'PROFESSIONAL', price: '$19', period: '/MONTH', features: ['Unlimited Matches', 'Advanced Filters', 'Priority Support', 'Full Analytics', 'Verified Badge'], highlighted: true }, { name: 'ENTERPRISE', price: '$49', period: '/MONTH', features: ['Everything in Pro', 'API Access', 'Dedicated Manager', 'Custom Protocols', 'Multi-Unit Support'], highlighted: false }] as tier}
					<div
						class="rounded border-2 p-8 {tier.highlighted
							? 'border-warning bg-warning/10'
							: 'border-secondary bg-muted'}"
					>
						{#if tier.highlighted}
							<div
								class="bg-warning text-primary-foreground mb-4 inline-block rounded px-3 py-1 text-xs font-bold"
							>
								RECOMMENDED
							</div>
						{/if}
						<h3 class="font-(family-name:--font-display) text-2xl">
							{tier.name}
						</h3>
						<div class="mt-4">
							<span
								class="font-(family-name:--font-display) text-5xl"
							>
								{tier.price}
							</span>
							<span class="text-muted-foreground">{tier.period}</span>
						</div>
						<ul class="mt-6 space-y-3">
							{#each tier.features as feature}
								<li class="flex items-center gap-2 text-sm">
									<span class="text-success">✓</span>
									{feature}
								</li>
							{/each}
						</ul>
						<button
							class="border-secondary mt-8 w-full rounded border-2 py-3 font-(family-name:--font-display) text-lg transition {tier.highlighted
								? 'bg-primary text-primary-foreground hover:bg-primary/80'
								: 'bg-background hover:bg-border'} active:scale-95"
						>
							ACTIVATE
						</button>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- CTA Section -->
	<section class="bg-secondary text-secondary-foreground px-6 py-24">
		<div class="mx-auto max-w-2xl text-center">
			<h2 class="font-(family-name:--font-display) text-5xl">
				DEPLOY NOW
			</h2>
			<p class="mt-4 opacity-80">
				Enter the grid. Find your cat's perfect match today.
			</p>
			<div class="mt-8 flex gap-4">
				<input
					type="email"
					bind:value={email}
					placeholder="ENTER EMAIL ADDRESS"
					class="border-background/20 bg-background/10 placeholder:text-secondary-foreground/50 focus:border-primary flex-1 rounded border-2 px-6 py-4 focus:outline-none"
				/>
				<button
					class="border-primary bg-primary text-primary-foreground hover:bg-primary/80 rounded border-2 px-8 py-4 font-(family-name:--font-display) text-xl transition active:scale-95"
				>
					SUBMIT
				</button>
			</div>
		</div>
	</section>

	<!-- Footer -->
	<footer class="border-secondary bg-muted border-t-2 px-6 py-12">
		<div class="mx-auto max-w-6xl">
			<div class="grid gap-8 md:grid-cols-4">
				<div>
					<div class="flex items-center gap-2">
						<span class="text-2xl">🐱</span>
						<span class="font-(family-name:--font-display) text-xl">
							PAWMATCH
						</span>
					</div>
					<p class="text-muted-foreground mt-4 text-sm">
						Industrial-grade feline matching since 2024.
					</p>
				</div>
				{#each [{ title: 'SYSTEMS', links: ['Features', 'Pricing', 'API'] }, { title: 'SUPPORT', links: ['Documentation', 'Status', 'Contact'] }, { title: 'LEGAL', links: ['Privacy', 'Terms', 'Compliance'] }] as col}
					<div>
						<h4 class="font-(family-name:--font-display) text-lg">
							{col.title}
						</h4>
						<ul class="text-muted-foreground mt-4 space-y-2 text-sm">
							{#each col.links as link}
								<li>
									<a
										href="#{link.toLowerCase()}"
										class="hover:text-primary">{link}</a
									>
								</li>
							{/each}
						</ul>
					</div>
				{/each}
			</div>
			<div
				class="border-border text-muted-foreground mt-12 border-t pt-8 text-center text-sm"
			>
				© 2024 PAWMATCH INDUSTRIES. ALL SYSTEMS OPERATIONAL.
			</div>
		</div>
	</footer>

	<!-- Bottom hazard stripe -->
	<div
		class="h-4 bg-[repeating-linear-gradient(45deg,var(--color-warning),var(--color-warning)_10px,var(--color-foreground)_10px,var(--color-foreground)_20px)]"
	></div>
</div>
