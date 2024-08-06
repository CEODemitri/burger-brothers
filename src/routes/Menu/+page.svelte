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

<main class="flex-1 w-full bg-light">
	<div class="navbar bg-base-100">
		<div class="flex-1">
			<a class="btn btn-ghost text-xl" href="/">Burger Brothers</a>
		</div>
		<div class="flex-none">
			<ul class="menu menu-horizontal px-1">
				<li><a>Drinks</a></li>
				<li>
					<details>
						<summary>Appetizers</summary>
						<ul class="bg-base-100 rounded-t-none p-2">
							<li><a>Sharing</a></li>
							<li><a>Chill</a></li>
						</ul>
					</details>
				</li>
				<li>
					<details>
						<summary>Entrees</summary>
						<ul class="bg-base-100 rounded-t-none p-2">
							<li><a>Link 1</a></li>
							<li><a>Link 2</a></li>
						</ul>
					</details>
				</li>
				<li>
					<details>
						<summary>Feasts</summary>
						<ul class="bg-base-100 rounded-t-none p-2">
							<li><a>Link 1</a></li>
							<li><a>Link 2</a></li>
						</ul>
					</details>
				</li>
				<li>
					<details>
						<summary>Desserts</summary>
						<ul class="bg-base-100 rounded-t-none p-2">
							<li><a>Link 1</a></li>
							<li><a>Link 2</a></li>
						</ul>
					</details>
				</li>
				<li>
					<details>
						<summary>Seniors</summary>
						<ul class="bg-base-100 rounded-t-none p-2">
							<li><a>Link 1</a></li>
							<li><a>Link 2</a></li>
						</ul>
					</details>
				</li>
			</ul>
		</div>
	</div>
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
