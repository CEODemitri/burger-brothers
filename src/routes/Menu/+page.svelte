<script>
	import { fade } from 'svelte/transition';
	import MediumCards from '../../components/Cards/MediumCards.svelte';

	// Define card data for each category
	const categories = {
		Drinks: [
			{
				src: '/specials/drinks/blueberrySlush.png',
				price: 5.99,
				name: 'Blueberry Slush',
				description: 'Big taste of blueberries from the gardens of Oz.'
			},
			{
				src: '/specials/drinks/mangoTea.png',
				price: 5.99,
				name: 'Mango Sweet Tea',
				description: 'Big taste of mangos from the Giants of Peru.'
			},
			{
				src: '/specials/drinks/sLemonadeSlush.png',
				price: 5.99,
				name: 'Strawberry Slush',
				description:
					'Big taste of strawberries from the gardens of Athena. Cold and Sweet, oh just right'
			},
			{
				src: '/specials/drinks/sLemonadeSlush.png',
				price: 5.99,
				name: 'Strawberry Slush',
				description:
					'Big taste of strawberries from the gardens of Athena. Cold and Sweet, oh just right'
			},
			{
				src: '/specials/drinks/sLemonadeSlush.png',
				price: 5.99,
				name: 'Strawberry Slush',
				description:
					'Big taste of strawberries from the gardens of Athena. Cold and Sweet, oh just right'
			}
		],
		Appetizers: [
			{
				src: '/specials/appetizers/flower.png',
				price: 22.99,
				name: 'Cauliflower',
				description:
					'You smell me. Quinoa from the untapped valleys you and I never seen, across this earth. Finest ingredients.'
			},
			{
				src: '/specials/appetizers/pickles.png',
				price: 14.99,
				name: 'Fried Pickles',
				description:
					'You see me. Chops raised on our farms. If you know good food, what are we talking about, order now.'
			},
			{
				src: '/specials/appetizers/spinachDip.png',
				price: 30.99,
				name: 'Spinach Dip',
				description:
					'You feel me. All natural eggs, from the land, paired elegantly with fresh cut hashbrowns, twice.'
			},
			{
				src: '/specials/appetizers/spinachDip.png',
				price: 30.99,
				name: 'Spinach Dip',
				description:
					'You feel me. All natural eggs, from the land, paired elegantly with fresh cut hashbrowns, twice.'
			},
			{
				src: '/specials/appetizers/spinachDip.png',
				price: 30.99,
				name: 'Spinach Dip',
				description:
					'You feel me. All natural eggs, from the land, paired elegantly with fresh cut hashbrowns, twice.'
			},
			{
				src: '/specials/appetizers/spinachDip.png',
				price: 30.99,
				name: 'Spinach Dip',
				description:
					'You feel me. All natural eggs, from the land, paired elegantly with fresh cut hashbrowns, twice.'
			}
		],
		Entrees: [
			{
				src: '/specials/grill-quinoa.png',
				price: 85.99,
				name: 'Grilled Quinoa',
				description:
					'You smell me. Quinoa from the untapped valleys you and I never seen, across this earth. Finest ingredients.'
			},
			{
				src: '/specials/pork.png',
				price: 45.99,
				name: 'Pork Chop',
				description:
					'You see me. Chops raised on our farms. If you know good food, what are we talking about, order now.'
			},
			{
				src: '/specials/bk.png',
				price: 65.99,
				name: 'Break Fast',
				description:
					'You feel me. All natural eggs, from the land, paired elegantly with fresh cut hashbrowns, twice.'
			},
			{
				src: '/specials/bk.png',
				price: 65.99,
				name: 'Break Fast',
				description:
					'You feel me. All natural eggs, from the land, paired elegantly with fresh cut hashbrowns, twice.'
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
				src: '/specials/desserts/roseCheeseCake.png',
				price: 7.99,
				name: 'RoseCake',
				description: 'Edible roses paired perfectly with lush cheesecake baked fresh every morning.'
			},
			{
				src: '/specials/desserts/chocolateGold.png',
				price: 18.99,
				name: 'Gold Chocolate',
				description: 'I dare you. And say cheese with these.'
			},
			{
				src: '/specials/desserts/cashewCream.png',
				price: 10.99,
				name: 'Cashew Cream',
				description: 'Tastyically fresh ice cream. Brilliance in every bite.'
			},
			{
				src: '/specials/desserts/cashewCream.png',
				price: 10.99,
				name: 'Cashew Cream',
				description: 'Tastyically fresh ice cream. Brilliance in every bite.'
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
	let cart = [];

	function addToCart(item, quantity) {
		const existingItem = cart.find((i) => i.name === item.name);
		if (existingItem) {
			existingItem.quantity += quantity;
		} else {
			cart = [...cart, { ...item, quantity }];
		}
	}
</script>

<div class="flex-1 bg-[#000] mx-auto">
	<h1 class="text-3xl md:text-5xl lg:text-[6rem] leading-[1em] ff-serif text-center uppercase pt-8">
		<span class="ff-sans">Brothers' </span>Menu
	</h1>
	<div class="content flex">
		<!-- Sidebar Menu -->
		<nav class="flex flex-col gap-4 bg-gray-900/50 ff-sans py-8 px-4 md:fixed">
			{#each Object.keys(categories) as category}
				<button
					on:click={() => (selectedCategory = category)}
					class:bg-gray-500={selectedCategory === category}
					class="text-grey-800 px-4 py-2 rounded-md"
				>
					{category}
				</button>
			{/each}
			<!-- Main Content -->
		</nav>

		<div class="px-4 py-8 md:m-auto">
			{#each categories[selectedCategory] as item}
				<div class="flex items-center space-x-4 p-4 bg-gray-900/50 rounded-md">
					<img src={item.src} alt={item.name} class="w-36 h-36 md:w-60 md:h-60 rounded-md" />
					<div class="flex flex-col">
						<h3 class="text-lg font-semibold text-white">{item.name}</h3>
						<p class="text-sm text-gray-400">{item.description}</p>
						<p class="text-sm text-gray-400">{item.price}</p>
						<div class="flex flex-col md:flex-row items-center">
							<input
								type="number"
								min="1"
								bind:value={item.quantity}
								class="w-16 text-center text-gray-800"
							/>
							<button
								on:click={() => addToCart(item, item.quantity)}
								class="ml-4 px-4 py-2 bg-gray-800 text-white rounded-md">Add to Cart</button
							>
						</div>
					</div>
				</div>
			{/each}
		</div>
	</div>

	<footer class="bg-gray-900/70 p-4 h-60">
		<!-- ... (other HTML) -->

		<div class="h-20 overflow-y-auto flex items-center">
			<div class="flex space-x-2">
				{#each cart as item}
					<div class="flex flex-col items-center space-y-2 px-4 py-2 bg-gray-800 rounded-md">
						<img src={item.src} alt={item.name} class="w-16 h-16 rounded-md" />
						<p class="text-sm text-white">{item.name}</p>
						<p class="text-sm text-white">{item.price} x {item.quantity}</p>
					</div>
				{/each}
			</div>
		</div>
	</footer>
</div>

<style>
	main {
		max-width: 1440px;
	}
</style>
