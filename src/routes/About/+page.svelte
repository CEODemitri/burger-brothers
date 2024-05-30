<script>
  import '@fontsource-variable/comfortaa';
  import '@fontsource/fugaz-one';   
</script>

<!-- history, locations, leaders, partners, in the works, -->
<div class="container px-4">
	<div class="flex flex-col items-center gap-4 text-center">
		<img
			src="/placeholder.svg"
			width="400"
			height="200"
			alt="Burger Bento"
			class="aspect-[2/1] overflow-hidden rounded-lg object-cover object-center"
		/>
		<div class="grid gap-2">
			<h1 class="text-3xl font-bold tracking-tighter sm:text-4xl text-[#232135]">Our Locations</h1>
			<p
				class="text-gray-500 md:text-xl/relaxed lg:text-base/relaxed xl:text-xl/relaxed dark:text-gray-400"
			>
				Visit us at one of our convenient locations.
			</p>
		</div>
	</div>
	<div class="grid max-w-3xl w-full mx-auto gap-6 lg:gap-8">
		
    <!-- location 1 -->
    <div class="relative group mt-10">
			<div
				class="rounded-lg border bg-card text-card-foreground shadow-sm overflow-visible"
				data-v0-t="card"
			>
				<a class="absolute inset-0 z-10 rounded-lg focus-visible:outline-none" href="#"></a>
				<div class="p-6">
					<h3 class="font-semibold whitespace-nowrap tracking-tight text-2xl">Union Square</h3>
					<p class="text-sm text-muted-foreground">10 Union Square, San Francisco, CA 94108</p>
				</div>
				<button
					class="inline-flex items-center justify-center whitespace-nowrap text-sm font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 bg-black text-white hover:bg-primary/90 h-11 rounded-md px-8"
				>
					Book a Table
				</button>
				<img
					src="/placeholder.svg"
					width="600"
					height="300"
					alt="Bento Box"
					class="aspect-[2/1] mt-5 object-cover object-center rounded-b-lg"
				/>
			</div>
			Indoor seating for 50 guests. Try our special truffle fries available only at this location.
		</div>

    <!-- location 2 -->
		<div class="relative group mt-10">
			<div
				class="rounded-lg border bg-card text-card-foreground shadow-sm overflow-visible"
				data-v0-t="card"
			>
				<a class="absolute inset-0 z-10 rounded-lg focus-visible:outline-none" href="#"></a>
				<div class="p-6">
					<h3 class="font-semibold whitespace-nowrap tracking-tight text-2xl">Times Square</h3>
					<p class="text-sm text-muted-foreground">234 W 42nd St, New York, NY 10036</p>
				</div>
        <button
					class="inline-flex items-center justify-center whitespace-nowrap text-sm font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 bg-black text-white hover:bg-primary/90 h-11 rounded-md px-8"
				>
					Book a Table
				</button>
				<img
					src="/placeholder.svg"
					width="600"
					height="300"
					alt="Bento Box"
					class="aspect-[2/1] mt-5 object-cover object-center rounded-b-lg"
				/>
			</div>
			Indoor seating for 30 guests. Enjoy our limited edition matcha milkshakes available only at this
			location.
		</div>

    <!-- location 3 -->
		<div class="relative group mt-10 mb-16">
			<div
				class="rounded-lg border bg-card text-card-foreground shadow-sm overflow-visible"
				data-v0-t="card"
			>
				<a class="absolute inset-0 z-10 rounded-lg focus-visible:outline-none" href="#"></a>
				<div class="p-6">
					<h3 class="font-semibold whitespace-nowrap tracking-tight text-2xl">Waikiki Beach</h3>
					<p class="text-sm text-muted-foreground">2255 Kuhio Ave, Honolulu, HI 96815</p>
				</div>
        <button
					class="inline-flex items-center justify-center whitespace-nowrap text-sm font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 bg-black text-white hover:bg-primary/90 h-11 rounded-md px-8"
				>
					Book a Table
				</button>
				<img
					src="/placeholder.svg"
					width="600"
					height="300"
					alt="Bento Box"
					class="aspect-[2/1] mt-5 object-cover object-center rounded-b-lg"
				/>
			</div>
			Oceanfront seating for 20 guests. Don't miss our Hawaiian pineapple burgers available only at this
			location.
		</div>
	</div>
</div>

<style>
  h1, h2, h3 {
    font-family: 'Fugaz One', system-ui;
  }

  /* switching the button font for a bit of variance on this page */
  p, button {
    font-family: 'Comfortaa Variable', sans-serif;
  }
</style>