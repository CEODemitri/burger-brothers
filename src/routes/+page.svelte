<script>
	// Supports weights 300-700
	import Cards from './components/Cards/Cards.svelte';
	import Carousel from './components/Home/Carousel.svelte';

	const melt = {
		src: '/specials/grill-quinoa.png',
		price: 85.99,
		name: 'Grilled Quinoa',
		description: 'You smell me. Quinoa from the untapped valleys across this earth. Finest ingredients.'
	};

	const pork = {
		src: '/specials/pork.png',
		price: 45.99,
		name: 'Pork Chop',
		description: 'You see me. Chops raised on our farms. If you know good food, what are we talking about, order now.'
	};

	const breakfast = {
		src: '/specials/bk.png',
		price: 65.99,
		name: 'Break Fast',
		description: 'You feel me. All natural eggs paired elegantly with fresh cut hashbrowns.'
	};
</script>

<!--
// v0 by Vercel.
// https://v0.dev/t/NTp0OzPUCg9
-->
<div class="flex flex-col min-h-[100dvh]">
	<div class="banner h-10 bg-black text-center text-white py-2">
		<p>Homepage Banner: Important Text Here</p>
	</div>

	<main class="flex-1">
		<section class="w-full py-12 md:py-18 lg:py-24">
			<div class="container flex flex-col items-center justify-center space-y-4 px-4 md:px-6 m-auto">
				<div class="space-y-2 text-center">
					<span class="pill bg-black text-white w-fit p-1 m-auto px-3 rounded-xl">Legendary</span>
					<h1 class="text-[4rem] md:text-[5rem] lg:text-[6rem] font-bold tracking-tighter">
						Burger Brothers
					</h1>
					<p
						class="mx-auto max-w-[100ch] text-gray-500 md:text-xl/relaxed lg:text-base/relaxed xl:text-xl/relaxed dark:text-gray-400 font"
					>
						Premium and fresh ingredients all day loaded into your favorite buns. Gourmet flavors
						dripping. The perfect burger. YOUR perfect burger, Made your way.
					</p>
				</div>
				<img
					src="/landing/heroBurger-grilled_chz.png"
					width="600"
					height="400"
					alt="Hero"
					class="mx-auto aspect-video overflow-hidden rounded-xl object-cover object-center lg:w-[75%]"
				/>
				<section>
					<button class="text-white bg-black p-2 rounded-md special hover:scale-125 hover:mx-4"
						><a href="/Menu" class="special">Order Online</a></button
					>
					<a href="/Locations" class="underline p-2 rounded-md special">Find a Location</a>
				</section>
			</div>
		</section>

		<!-- review carousel -->
		<h2 class="text-3xl font-bold tracking-tighter sm:text-4xl md:text-5xl my-5 mx-5">Flavors for all Ranges</h2>
		<Carousel />

		<!-- popular section -->
		<section class="w-full py-12 md:py-24 lg:py-32 border-t bg-neutral-200">
			<div class="container grid items-center justify-center gap-4 px-4 text-center md:px-6 m-auto">
				<span class="pill bg-black text-white w-fit m-auto px-3 rounded-xl">Burgertastic</span>
				<div class="space-y-3">
					<h2 class="text-3xl font-bold tracking-tighter sm:text-4xl md:text-5xl">Popular Menu</h2>
					<p
						class="mx-auto max-w-[600px] text-gray-500 md:text-xl/relaxed lg:text-base/relaxed xl:text-xl/relaxed dark:text-gray-400"
					>
						Limited timing creations. We chef in parallel with nature; many of our beautiful
						creations are seasonal, not to be abused or imitated.
					</p>
				</div>
				<div
					class="mx-auto grid max-w-5xl items-start gap-6 sm:grid-cols-2 md:gap-12 lg:max-w-none lg:grid-cols-3"
				>
					<Cards {...breakfast} />
					<Cards {...melt} />
					<Cards {...pork} />
				</div>
			</div>
		</section>

		<!-- Value Section -->
		<!-- written with more wisdom; all styles here are preloaded. no editing has been done -->
		<article class="max-w-xl md:max-w-2xl m-auto mt-16">
			<h2 class="text-3xl font-bold tracking-tighter sm:text-4xl md:text-5xl text-center">Your Bucks Matter</h2>
			<p class="mt-4">Cut the foogazi and come experience a Real Burger.</p>

			<section class="flex flex-col gap-5 my-10">
                <!-- copy and paste these generic cards and styles with no edit -->
				<div class="card card-side bg-base-100 shadow-xl">
					<figure>
						<img
							src="https://daisyui.com/images/stock/photo-1635805737707-575885ab0820.jpg"
							alt="Movie"
						/>
					</figure>
					<div class="card-body">
						<h2 class="card-title">Real Organic Ingredients</h2>
						<p>Click the button to watch on Jetflix app.</p>
						<div class="card-actions justify-end">
							<button class="btn btn-primary">Interactive Map</button>
						</div>
					</div>
				</div>

                <div class="card card-side bg-base-100 shadow-xl">
					<div class="card-body">
						<h2 class="card-title">Passionate Chefs and Staff</h2>
						<p>Click the button to watch on Jetflix app.</p>
						<div class="card-actions justify-end">
							<button class="btn btn-primary">See Staff</button>
						</div>
					</div>
                    <figure>
						<img
							src="https://daisyui.com/images/stock/photo-1635805737707-575885ab0820.jpg"
							alt="Movie"
						/>
					</figure>
				</div>

                <div class="card card-side bg-base-100 shadow-xl">
                    <figure>
						<img
							src="https://daisyui.com/images/stock/photo-1635805737707-575885ab0820.jpg"
							alt="Movie"
						/>
					</figure>
					<div class="card-body">
						<h2 class="card-title">Golden Recipe</h2>
						<p>Click the button to watch on Jetflix app.</p>
						<div class="card-actions justify-end">
							<button class="btn btn-primary">Order Now</button>
						</div>
					</div>
				</div>
			</section>
		</article>
	</main>
</div>

<style>
	h1,
	h2,
	h3,
	.special {
		font-family: 'Fugaz One', system-ui;
	}

	p,
	button {
		font-family: 'Comfortaa Variable', sans-serif;
		font-size: 16px;
		line-height: 24px;
	}
</style>
