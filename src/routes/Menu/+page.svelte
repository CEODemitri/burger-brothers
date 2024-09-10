<script>
	import { fade } from 'svelte/transition';
	import MediumCards from '../../components/Cards/MediumCards.svelte';
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

<main class="flex-1 w-full bg-[#000]">
	<h1 class="text-3xl md:text-5xl lg:text-[6rem] leading-[1em] ff-serif text-center uppercase pt-8">
		<span class="ff-sans">Brothers' </span>Menu
	</h1>
	<div class="content flex">
		<ul class="menu menu-horizontal px-1 flex flex-col w-1/5 h-[70vh] bg-gray-900">
			<li>
				<div class="collapse collapse-plus">
					<input type="radio" name="my-accordion-3" checked="checked" />
					<div class="collapse-title font-medium">Drinks</div>
					<div class="collapse-content">
						<p>hello</p>
					</div>
				</div>
			</li>
			<li>
				<div class="collapse collapse-plus">
					<input type="radio" name="my-accordion-3" checked="checked" />
					<div class="collapse-title font-medium">Appetizers</div>
					<div class="collapse-content">
						<p>hello</p>
					</div>
				</div>
			</li>
			<li>
				<div class="collapse collapse-plus">
					<input type="radio" name="my-accordion-3" checked="checked" />
					<div class="collapse-title font-medium">Entrees</div>
					<div class="collapse-content">
						<p>hello</p>
					</div>
				</div>
			</li>
			<li>
				<div class="collapse collapse-plus">
					<input type="radio" name="my-accordion-3" checked="checked" />
					<div class="collapse-title font-medium">Feasts</div>
					<div class="collapse-content">
						<p>hello</p>
					</div>
				</div>
			</li>
			<li>
				<div class="collapse collapse-plus">
					<input type="radio" name="my-accordion-3" checked="checked" />
					<div class="collapse-title font-medium">Desserts</div>
					<div class="collapse-content">
						<p>hello</p>
					</div>
				</div>
			</li>
			<li>
				<div class="collapse collapse-plus">
					<input type="radio" name="my-accordion-3" checked="checked" />
					<div class="collapse-title font-medium">Seniors</div>
					<div class="collapse-content">
						<p>hello</p>
					</div>
				</div>
			</li>
		</ul>

		<article class="w-4/5 h-[70vh] pt-8">
			<div class="hero">
				<div class="hero-content text-center">
					<div class="max-w-md">
						<h1 class="text-5xl font-bold">Hello there</h1>
						<p class="py-6">
							Provident cupiditate voluptatem et in. Quaerat fugiat ut assumenda excepturi
							exercitationem quasi. In deleniti eaque aut repudiandae et a id nisi.
						</p>
						<button class="btn btn-primary">Get Started</button>
					</div>
				</div>
			</div>
		</article>
	</div>

	<footer class="bg-gray-800 p-4">
		<div class="flex items-center justify-between">
			<h2 class="text-lg font-semibold">Cart</h2>
			<svg
				xmlns="http://www.w3.org/2000/svg"
				width="24"
				height="24"
				viewBox="0 0 24 24"
				fill="none"
				stroke="currentColor"
				stroke-width="2"
				stroke-linecap="round"
				stroke-linejoin="round"
				class="h-6 w-6"
			>
				<circle cx="8" cy="21" r="1"></circle>
				<circle cx="19" cy="21" r="1"></circle>
				<path d="M2.05 2.05h2l2.66 12.42a2 2 0 0 0 2 1.58h9.78a2 2 0 0 0 1.95-1.57l1.65-7.43H5.12"
				></path>
			</svg>
		</div>
		<hr class="my-2 border-t border-gray-200" />
		<div class="h-20 overflow-y-auto">
			<div class="flex space-x-2">
				<img
					src="/placeholder.svg?height=40&width=40"
					alt="Burger 1"
					class="w-10 h-10 rounded-full"
				/>
				<img
					src="/placeholder.svg?height=40&width=40"
					alt="Burger 2"
					class="w-10 h-10 rounded-full"
				/>
				<img
					src="/placeholder.svg?height=40&width=40"
					alt="Burger 3"
					class="w-10 h-10 rounded-full"
				/>
				<img src="/placeholder.svg?height=40&width=40" alt="Fries" class="w-10 h-10 rounded-full" />
				<img src="/placeholder.svg?height=40&width=40" alt="Drink" class="w-10 h-10 rounded-full" />
			</div>
		</div>
	</footer>
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
