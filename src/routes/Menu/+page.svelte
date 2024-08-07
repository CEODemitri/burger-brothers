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
	<div class="navbar">
		<ul class="menu menu-horizontal px-1 flex flex-col">
			<li><a>Drinks</a></li>
			<li><a>Appetizers</a></li>
			<li><a>Entrees</a></li>
			<li><a>Feasts</a></li>
			<li><a>Desserts</a></li>
			<li><a>Seniors</a></li>
		</ul>
	</div>

	<div></div>
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
