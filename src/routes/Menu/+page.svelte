<script>
  import { fade } from 'svelte/transition'; 
	import MediumCards from '../components/Cards/MediumCards.svelte';
	let currentPage = 0;
	const pages = Array(2).fill(0); // Change this to the number of pages you have

	const cardData = [
		// Page 1
		[
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Grilled Quinoa',
				description:
					'You smell me. Quinoa from the untapped valleys across this earth. Finest ingredients.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Grilled Quinoa',
				description:
					'You smell me. Quinoa from the untapped valleys across this earth. Finest ingredients.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Grilled Quinoa',
				description:
					'You smell me. Quinoa from the untapped valleys across this earth. Finest ingredients.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Grilled Quinoa',
				description:
					'You smell me. Quinoa from the untapped valleys across this earth. Finest ingredients.'
			}
		],
		// Page 2
		[
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'New Page',
				description:
					'You smell me. Quinoa from the untapped valleys across this earth. Finest ingredients.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'New Page',
				description:
					'You smell me. Quinoa from the untapped valleys across this earth. Finest ingredients.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'New Page',
				description:
					'You smell me. Quinoa from the untapped valleys across this earth. Finest ingredients.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'New Page',
				description:
					'You smell me. Quinoa from the untapped valleys across this earth. Finest ingredients.'
			}
		]
		// Add more pages as needed
	];
</script>

<main class="flex-1 w-full bg-light text-dark">
	<section class="w-full py-12 lg:py-24">
		<div class="container grid items-center justify-center gap-4 px-4 text-center md:gap-10">
			<div class="space-y-4 lg:space-y-6">
				<h1 class="text-4xl font-bold tracking-tighter sm:text-5xl md:text-6xl ff-serif uppercase">Menu</h1>
				<p
					class="mx-auto max-w-[600px] text-gray-500 md:text-xl/relaxed lg:text-base/relaxed xl:text-xl/relaxed dark:text-gray-400 ff-sans"
				>
					Handcrafted with love. Enjoy our delicious burgers. Starters, desserts, drinks, our menu
					has something for the whole table.
				</p>
			</div>
		</div>
	</section>

	<!-- starters -->
	<div
		class="rounded-lg border bg-card text-card-foreground shadow-sm bg-white"
		data-v0-t="card"
	>
		<div class="p-6 flex flex-row space-y-0 items-start gap-2">
			<div class="grid gap-1">
				<h3 class="text-5xl font-semibold whitespace-nowrap leading-none tracking-tight uppercase">
					Starters
				</h3>
				<p class="text-sm text-muted-foreground text-accent ff-sans">Delicious appetizers to kick off your meal.</p>
			</div>
		</div>

		<!-- Pagination -->
		<div class="pagination">
			{#each pages as _, i}
				<button class="dot" on:click={() => (currentPage = i)}></button>
			{/each}
		</div>

		<div class="w-5/6 ml-5" id="page">
			{#each pages as _, i}
				<!-- Page {i + 1} -->
				<div
					class="container grid items-start gap-6 px-4 md:grid-cols-2 md:gap-10 lg:grid-cols-3"
					style="display: {currentPage === i ? 'block' : 'none'};"
          transition:fade={{duration: 500}}
				>
					{#each cardData[i] as card}
						<MediumCards
							name={card.name}
							description={card.description}
							price={card.price}
							src={card.src}
						/>
					{/each}
				</div>
			{/each}
		</div>
	</div>

	<!-- entrees -->
	<div class="rounded-lg border bg-card text-card-foreground shadow-sm flex justify-center" data-v0-t="card">
		<div class="p-6 flex flex-row space-y-0 items-center gap-2">
			<div class="grid gap-1">
				<h3 class="text-5xl font-semibold whitespace-nowrap leading-none tracking-tight">Entrees</h3>
				<p class="text-sm text-muted-foreground">Take a peek. Do not bite the screen, only images.</p>
			</div>
		</div>
		<div class="w-96 carousel rounded-box">
			<div class="carousel-item w-full">
			  <img src="https://daisyui.com/images/stock/photo-1559703248-dcaaec9fab78.jpg" class="w-full" alt="Tailwind CSS Carousel component" />
			</div> 
			<div class="carousel-item w-full">
			  <img src="https://daisyui.com/images/stock/photo-1565098772267-60af42b81ef2.jpg" class="w-full" alt="Tailwind CSS Carousel component" />
			</div> 
			<div class="carousel-item w-full">
			  <img src="https://daisyui.com/images/stock/photo-1572635148818-ef6fd45eb394.jpg" class="w-full" alt="Tailwind CSS Carousel component" />
			</div> 
			<div class="carousel-item w-full">
			  <img src="https://daisyui.com/images/stock/photo-1494253109108-2e30c049369b.jpg" class="w-full" alt="Tailwind CSS Carousel component" />
			</div> 
			<div class="carousel-item w-full">
			  <img src="https://daisyui.com/images/stock/photo-1550258987-190a2d41a8ba.jpg" class="w-full" alt="Tailwind CSS Carousel component" />
			</div> 
			<div class="carousel-item w-full">
			  <img src="https://daisyui.com/images/stock/photo-1559181567-c3190ca9959b.jpg" class="w-full" alt="Tailwind CSS Carousel component" />
			</div> 
			<div class="carousel-item w-full">
			  <img src="https://daisyui.com/images/stock/photo-1601004890684-d8cbf643f5f2.jpg" class="w-full" alt="Tailwind CSS Carousel component" />
			</div>
		</div>
	</div>

	<!-- drinks -->
	<div class="rounded-lg border bg-card text-card-foreground shadow-sm bg-white" data-v0-t="card">
		<div class="p-6 flex flex-row space-y-0 items-start gap-2">
			<div class="grid gap-1">
				<h3 class="text-5xl font-semibold whitespace-nowrap leading-none tracking-tight">Drinks</h3>
				<p class="text-sm text-muted-foreground">Wash it down with a classic lift.</p>
			</div>
		</div>
		<div class="p-6">
			<div class="container grid items-start gap-6 px-4 md:grid-cols-2 md:gap-10 lg:grid-cols-3">
				<div class="carousel rounded-box w-96">
					<div class="carousel-item w-1/2">
						<img
							src="https://daisyui.com/images/stock/photo-1559703248-dcaaec9fab78.jpg"
							class="w-full"
              alt="coming soon"
						/>
					</div>
					<div class="carousel-item w-1/2">
						<img
							src="https://daisyui.com/images/stock/photo-1565098772267-60af42b81ef2.jpg"
							class="w-full"
              alt="coming soon"
						/>
					</div>
					<div class="carousel-item w-1/2">
						<img
							src="https://daisyui.com/images/stock/photo-1572635148818-ef6fd45eb394.jpg"
							class="w-full"
              alt="coming soon"
						/>
					</div>
					<div class="carousel-item w-1/2">
						<img
							src="https://daisyui.com/images/stock/photo-1494253109108-2e30c049369b.jpg"
							class="w-full"
              alt=""
						/>
					</div>
					<div class="carousel-item w-1/2">
						<img
							src="https://daisyui.com/images/stock/photo-1550258987-190a2d41a8ba.jpg"
							class="w-full"
              alt="coming soon"
						/>
					</div>
					<div class="carousel-item w-1/2">
						<img
							src="https://daisyui.com/images/stock/photo-1559181567-c3190ca9959b.jpg"
							class="w-full"
              alt="coming soon"
						/>
					</div>
					<div class="carousel-item w-1/2">
						<img
							src="https://daisyui.com/images/stock/photo-1601004890684-d8cbf643f5f2.jpg"
							class="w-full"
              alt="coming soon"
						/>
					</div>
				</div>
			</div>
		</div>
	</div>

	<!-- desserts -->
	<div
		class="rounded-lg border bg-card text-card-foreground shadow-sm bg-neutral-300"
		data-v0-t="card"
	>
		<div class="p-6 flex flex-row space-y-0 items-start gap-2">
			<div class="grid gap-1">
				<h3 class="text-5xl font-semibold whitespace-nowrap leading-none tracking-tight">
					Desserts
				</h3>
				<p class="text-sm text-muted-foreground">Delicious desserts to end your perfect meal.</p>
			</div>
		</div>
		<div class="p-6">
			<div class="container grid items-start gap-6 px-4 md:grid-cols-2 md:gap-10 lg:grid-cols-3">
				<MediumCards />
				<MediumCards />
				<MediumCards />
				<MediumCards />
			</div>
		</div>
	</div>

	<!-- old people -->
	<div class="rounded-lg border bg-card text-card-foreground shadow-sm bg-white" data-v0-t="card">
		<div class="p-6 flex flex-row space-y-0 items-start gap-2">
			<div class="grid gap-1">
				<h3 class="text-5xl font-semibold whitespace-nowrap leading-none tracking-tight">Old People Section</h3>
				<p class="text-sm text-muted-foreground">Wash it down with a classic lift.</p>
			</div>
		</div>
		<div class="p-6">
			<div class="container grid items-start gap-6 px-4 md:grid-cols-2 md:gap-10 lg:grid-cols-3">
				<div class="carousel rounded-box w-96">
					<div class="carousel-item w-1/2">
						<img
							src="https://daisyui.com/images/stock/photo-1559703248-dcaaec9fab78.jpg"
							class="w-full"
              alt="coming soon"
						/>
					</div>
					<div class="carousel-item w-1/2">
						<img
							src="https://daisyui.com/images/stock/photo-1565098772267-60af42b81ef2.jpg"
							class="w-full"
              alt="coming soon"
						/>
					</div>
					<div class="carousel-item w-1/2">
						<img
							src="https://daisyui.com/images/stock/photo-1572635148818-ef6fd45eb394.jpg"
							class="w-full"
              alt="coming soon"
						/>
					</div>
					<div class="carousel-item w-1/2">
						<img
							src="https://daisyui.com/images/stock/photo-1494253109108-2e30c049369b.jpg"
							class="w-full"
              alt=""
						/>
					</div>
					<div class="carousel-item w-1/2">
						<img
							src="https://daisyui.com/images/stock/photo-1550258987-190a2d41a8ba.jpg"
							class="w-full"
              alt="coming soon"
						/>
					</div>
					<div class="carousel-item w-1/2">
						<img
							src="https://daisyui.com/images/stock/photo-1559181567-c3190ca9959b.jpg"
							class="w-full"
              alt="coming soon"
						/>
					</div>
					<div class="carousel-item w-1/2">
						<img
							src="https://daisyui.com/images/stock/photo-1601004890684-d8cbf643f5f2.jpg"
							class="w-full"
              alt="coming soon"
						/>
					</div>
				</div>
			</div>
		</div>
	</div>

	<!-- add the carousel mover and logic -->
	<!-- change the p,button font to more systemmatic code -->
	<!-- components -->
	<!-- fix layout + add footer -->
</main>

<style>
	.dot {
		width: 10px;
		height: 10px;
		border-radius: 50%;
		background-color: #000;
		display: inline-block;
		margin: 0 5px;
	}
</style>
