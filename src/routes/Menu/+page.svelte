<script>
	import { fade } from 'svelte/transition';
	import MediumCards from '../../components/Cards/MediumCards.svelte'; // Assuming you have this component

	// Define card data for each category
	const categories = {
		Drinks: [
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Coke',
				description: 'Refreshing soda.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Pepsi',
				description: 'Popular cola drink.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Water',
				description: 'Purified water.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Juice',
				description: 'Fresh fruit juice.'
			}
		],
		Appetizers: [
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Spring Rolls',
				description: 'Crispy and delicious.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Nachos',
				description: 'Cheesy and spicy.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Mozzarella Sticks',
				description: 'Fried cheese sticks.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Bruschetta',
				description: 'Tomato and basil on toast.'
			}
		],
		Entrees: [
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Grilled Chicken',
				description: 'Juicy grilled chicken.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Beef Steak',
				description: 'Tender and flavorful.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Vegetarian Lasagna',
				description: 'Hearty and satisfying.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Salmon Fillet',
				description: 'Grilled to perfection.'
			}
		],
		Feasts: [
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'BBQ Platter',
				description: 'A variety of grilled meats.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Seafood Feast',
				description: 'A mix of seafood delights.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Vegetarian Feast',
				description: 'A selection of vegetarian dishes.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Meat Lovers',
				description: 'A hearty meat platter.'
			}
		],
		Desserts: [
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Cheesecake',
				description: 'Rich and creamy.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Brownies',
				description: 'Chocolatey goodness.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Ice Cream',
				description: 'Cold and sweet.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Tiramisu',
				description: 'Coffee-flavored treat.'
			}
		],
		Seniors: [
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Senior Special 1',
				description: 'A special for seniors.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Senior Special 2',
				description: 'Another senior delight.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Senior Special 3',
				description: 'Senior exclusive.'
			},
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Senior Special 4',
				description: 'A treat for our seniors.'
			}
		]
	};

	let selectedCategory = 'Drinks'; // Default category

	function selectCategory(category) {
		selectedCategory = category;
	}
</script>

<main class="flex-1 bg-[#000] mx-auto">
	<h1 class="text-3xl md:text-5xl lg:text-[6rem] leading-[1em] ff-serif text-center uppercase pt-8">
		<span class="ff-sans">Brothers' </span>Menu
	</h1>
	<div class="content flex">
		<!-- Sidebar Menu -->
		<ul class="menu menu-horizontal flex flex-col h-[70vh] bg-gray-900 text-white">
			{#each Object.keys(categories) as category}
				<li>
					<div class="collapse collapse-plus">
						<input
							type="radio"
							name="my-accordion-2"
							id={category}
							bind:group={selectedCategory}
							value={category}
							checked={selectedCategory === category}
							on:change={() => selectCategory(category)}
						/>
						<label for={category} class="collapse-title font-medium cursor-pointer">
							{category}
						</label>
						<div class="collapse-content p-4">
							<p>{categories[category].length} items</p>
						</div>
					</div>
				</li>
			{/each}
		</ul>

		<!-- Main Content -->
		<article class="w-4/5 h-[70vh] pt-8">
			<div class="hero">
				<div class="hero-content text-center">
					<div class="max-w-md">
						<h1 class="text-5xl font-bold">{selectedCategory}</h1>
						<p class="py-6">
							Here are the items available in the {selectedCategory} category.
						</p>
						<!-- Display cards for the selected category -->
						<div class="grid grid-cols-1 lg:grid-cols-4 gap-4">
							{#each categories[selectedCategory] as item}
								<MediumCards {item} />
							{/each}
						</div>
					</div>
				</div>
			</div>
		</article>
	</div>

	<footer class="bg-gray-900/70 p-4 h-60">
		<div class="flex items-center justify-between">
			<h2 class="text-lg font-semibold text-white">Cart</h2>
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
				class="h-6 w-6 text-white"
			>
				<circle cx="8" cy="21" r="1"></circle>
				<circle cx="19" cy="21" r="1"></circle>
				<path d="M2.05 2.05h2l2.66 12.42a2 2 0 0 0 2 1.58h9.78a2 2 0 0 0 1.95-1.57l1.65-7.43H5.12"
				></path>
			</svg>
		</div>
		<hr class="my-2 border-t border-gray-200" />
		<div class="h-20 overflow-y-auto flex items-center">
			<div class="flex space-x-2">
				<img
					src="/placeholder.svg?height=40&width=40"
					alt="Item 1"
					class="w-10 h-10 rounded-full"
				/>
				<img
					src="/placeholder.svg?height=40&width=40"
					alt="Item 2"
					class="w-10 h-10 rounded-full"
				/>
				<img
					src="/placeholder.svg?height=40&width=40"
					alt="Item 3"
					class="w-10 h-10 rounded-full"
				/>
				<img
					src="/placeholder.svg?height=40&width=40"
					alt="Item 4"
					class="w-10 h-10 rounded-full"
				/>
				<img
					src="/placeholder.svg?height=40&width=40"
					alt="Item 5"
					class="w-10 h-10 rounded-full"
				/>
			</div>
		</div>
	</footer>
</main>

<style>
	main {
		max-width: 1440px;
	}

	.dot {
		width: 10px;
		height: 10px;
		border-radius: 50%;
		background-color: #000;
		display: inline-block;
		margin: 0 5px;
	}
</style>
