<script>
	import { onMount } from 'svelte';
	import Cards from '../components/Cards/Cards.svelte';
	import Reviewers from '../components/Reviewers.svelte';
	import SectionHeader from '../components/SectionHeader.svelte';

	// starter items
	const flower = {
		src: '/specials/appetizers/flower.png',
		price: 22.99,
		name: 'Cauliflower',
		description:
			'You smell me. Quinoa from the untapped valleys you and I never seen, across this earth. Finest ingredients.'
	};

	const pickles = {
		src: '/specials/appetizers/pickles.png',
		price: 14.99,
		name: 'Fried Pickles',
		description:
			'You see me. Chops raised on our farms. If you know good food, what are we talking about, order now.'
	};

	const spinachDip = {
		src: '/specials/appetizers/spinachDip.png',
		price: 30.99,
		name: 'Spinach Dip',
		description:
			'You feel me. All natural eggs, from the land, paired elegantly with fresh cut hashbrowns, twice.'
	};

	// entree items
	const melt = {
		src: '/specials/grill-quinoa.png',
		price: 85.99,
		name: 'Grilled Quinoa',
		description:
			'You smell me. Quinoa from the untapped valleys you and I never seen, across this earth. Finest ingredients.'
	};

	const pork = {
		src: '/specials/pork.png',
		price: 45.99,
		name: 'Pork Chop',
		description:
			'You see me. Chops raised on our farms. If you know good food, what are we talking about, order now.'
	};

	const breakfast = {
		src: '/specials/bk.png',
		price: 65.99,
		name: 'Break Fast',
		description:
			'You feel me. All natural eggs, from the land, paired elegantly with fresh cut hashbrowns, twice.'
	};

	// dessert items
	const dessert1 = {
		/* ... */
	};
	const dessert2 = {
		/* ... */
	};
	const dessert3 = {
		/* ... */
	};

	// drink items
	const drink1 = {
		/* ... */
	};
	const drink2 = {
		/* ... */
	};
	const drink3 = {
		/* ... */
	};

	const tabs = [
		{ name: 'Starters', path: '#starters', content: [flower, pickles, spinachDip] },
		{ name: 'Entrees', path: '#entrees', content: [melt, pork, breakfast] },
		{ name: 'Drinks', path: '#drinks', content: [flower, pickles, spinachDip] },
		{ name: 'Desserts', path: '#desserts', content: [melt, pork, breakfast] }
	];

	let selectedTab = tabs[0]; // default to the first tab

	function selectTab(tab) {
		selectedTab = tab;
	}

	const popular = {
		pill: 'Burgertastic',
		title: 'Popular Menu',
		description:
			'Our burgers are meticulously crafted using only the finest ingredients. Each bite bursts with flavor and freshness, ensuring a culinary experience that delights every palate.'
	};

	const reviews = {
		pill: 'Reviews',
		title: 'Big Taste. Bigger Reviews.',
		description:
			'Join the Burger Brothers community and share your experience with us! Discover why our customers rave about Burger Brothers:'
	};

	const about = {
		pill: 'Burgerology',
		title: 'Who Are We?',
		description: `We support local farmers and source sustainable ingredients whenever possible. Our commitment to quality extends from farm to table, ensuring you enjoy food that's good for you and the planet.`
	};

	let qualities = [
		'Exceptional Service',
		'High-Quality Ingredients',
		'Unique and Delicious Menu',
		'Welcoming Atmosphere',
		'Clean and Comfortable Environment',
		'Excellent Value for Money'
	];

	onMount(() => {
		// Randomly apply the fade-in animation to each item
		document.querySelectorAll('.fade-in-out').forEach((element, index) => {
			let delay = Math.random() * 10; // Random delay between 0 and 10 seconds
			element.style.animationDelay = `${delay}s`;
		});
	});
</script>

<div class="home overflow-hidden">
	<div class="hero-section text-white px-4 relative">
		<h1
			class="text-5xl md:text-8xl lg:text-[9rem] leading-[1em] ff-serif text-center uppercase pt-8 text"
		>
			<span class="ff-sans">Burger </span>Brothers
		</h1>
		<p class="w-[75%] md:w-[550px] text-[0.9rem] ff-body p-4 lg:py-12">
			Discover a burger experience like no other at Burger Brothers. We are more than just a
			restaurant; we are a celebration of all things delicious, juicy, and perfectly crafted between
			two buns. From our hand-selected ingredients to our passion for flavor, every burger tells a
			story of quality and satisfaction.
		</p>

		<article class="flex justify-center">
			<!-- call to action space -->
			<section class="flex sm:flex-row text-sm py-4 bg-indigo-900/30 px-4 my-4 rounded-md">
				<p class="links">
					<svg
						xmlns="http://www.w3.org/2000/svg"
						fill="currentColor"
						class="bi bi-receipt-cutoff w-[26px] lg:w-70 h-10"
						viewBox="0 0 16 16"
					>
						<path
							d="M3 4.5a.5.5 0 0 1 .5-.5h6a.5.5 0 1 1 0 1h-6a.5.5 0 0 1-.5-.5m0 2a.5.5 0 0 1 .5-.5h6a.5.5 0 1 1 0 1h-6a.5.5 0 0 1-.5-.5m0 2a.5.5 0 0 1 .5-.5h6a.5.5 0 1 1 0 1h-6a.5.5 0 0 1-.5-.5m0 2a.5.5 0 0 1 .5-.5h6a.5.5 0 0 1 0 1h-6a.5.5 0 0 1-.5-.5m0 2a.5.5 0 0 1 .5-.5h6a.5.5 0 0 1 0 1h-6a.5.5 0 0 1-.5-.5M11.5 4a.5.5 0 0 0 0 1h1a.5.5 0 0 0 0-1zm0 2a.5.5 0 0 0 0 1h1a.5.5 0 0 0 0-1zm0 2a.5.5 0 0 0 0 1h1a.5.5 0 0 0 0-1zm0 2a.5.5 0 0 0 0 1h1a.5.5 0 0 0 0-1zm0 2a.5.5 0 0 0 0 1h1a.5.5 0 0 0 0-1z"
						/>
						<path
							d="M2.354.646a.5.5 0 0 0-.801.13l-.5 1A.5.5 0 0 0 1 2v13H.5a.5.5 0 0 0 0 1h15a.5.5 0 0 0 0-1H15V2a.5.5 0 0 0-.053-.224l-.5-1a.5.5 0 0 0-.8-.13L13 1.293l-.646-.647a.5.5 0 0 0-.708 0L11 1.293l-.646-.647a.5.5 0 0 0-.708 0L9 1.293 8.354.646a.5.5 0 0 0-.708 0L7 1.293 6.354.646a.5.5 0 0 0-.708 0L5 1.293 4.354.646a.5.5 0 0 0-.708 0L3 1.293zm-.217 1.198.51.51a.5.5 0 0 0 .707 0L4 1.707l.646.647a.5.5 0 0 0 .708 0L6 1.707l.646.647a.5.5 0 0 0 .708 0L8 1.707l.646.647a.5.5 0 0 0 .708 0L10 1.707l.646.647a.5.5 0 0 0 .708 0L12 1.707l.646.647a.5.5 0 0 0 .708 0l.509-.51.137.274V15H2V2.118z"
						/>
					</svg>
					<span> Order Online </span>
				</p>
				<p class="links">
					<svg
						xmlns="http://www.w3.org/2000/svg"
						fill="currentColor"
						class="bi bi-pin-map w-[26px] lg:w-70 h-10"
						viewBox="0 0 16 16"
					>
						<path
							fill-rule="evenodd"
							d="M3.1 11.2a.5.5 0 0 1 .4-.2H6a.5.5 0 0 1 0 1H3.75L1.5 15h13l-2.25-3H10a.5.5 0 0 1 0-1h2.5a.5.5 0 0 1 .4.2l3 4a.5.5 0 0 1-.4.8H.5a.5.5 0 0 1-.4-.8z"
						/>
						<path
							fill-rule="evenodd"
							d="M8 1a3 3 0 1 0 0 6 3 3 0 0 0 0-6M4 4a4 4 0 1 1 4.5 3.969V13.5a.5.5 0 0 1-1 0V7.97A4 4 0 0 1 4 3.999z"
						/>
					</svg>
					<span> Find Location </span>
				</p>
				<p class="links">
					<!-- icon -->
					<svg
						xmlns="http://www.w3.org/2000/svg"
						fill="currentColor"
						class="bi bi-people w-[26px] lg:w-70 h-10"
						viewBox="0 0 16 16"
					>
						<path
							d="M15 14s1 0 1-1-1-4-5-4-5 3-5 4 1 1 1 1zm-7.978-1L7 12.996c.001-.264.167-1.03.76-1.72C8.312 10.629 9.282 10 11 10c1.717 0 2.687.63 3.24 1.276.593.69.758 1.457.76 1.72l-.008.002-.014.002zM11 7a2 2 0 1 0 0-4 2 2 0 0 0 0 4m3-2a3 3 0 1 1-6 0 3 3 0 0 1 6 0M6.936 9.28a6 6 0 0 0-1.23-.247A7 7 0 0 0 5 9c-4 0-5 3-5 4q0 1 1 1h4.216A2.24 2.24 0 0 1 5 13c0-1.01.377-2.042 1.09-2.904.243-.294.526-.569.846-.816M4.92 10A5.5 5.5 0 0 0 4 13H1c0-.26.164-1.03.76-1.724.545-.636 1.492-1.256 3.16-1.275ZM1.5 5.5a3 3 0 1 1 6 0 3 3 0 0 1-6 0m3-2a2 2 0 1 0 0 4 2 2 0 0 0 0-4"
						/>
					</svg>
					<span> Catering </span>
				</p>
			</section>
			<img
				src="../HeroB.png"
				alt="juicy burger"
				class="p-0 m-0 box-content w-[600px] hidden sm:inline-block absolute"
			/>
		</article>
	</div>

	<!-- popular menu -->
	<div>
		<SectionHeader {...popular} />
		<div class="text-dark">
			<article class="flex justify-center ff-sans m-5 fs-400 flex-wrap">
				{#each tabs as tab}
					<a
						href={tab.path}
						on:click|preventDefault={() => selectTab(tab)}
						class="px-6 py-1 rounded-md mx-3 text-slate-500 hover:bg-orange-600 hover:text-white"
						>{tab.name}</a
					>
				{/each}
			</article>
		</div>

		<article class="p-5 flex flex-wrap justify-center">
			{#each selectedTab.content as item}
				<Cards {...item} />
			{/each}
		</article>
		<button class="m-auto text-center"><a href="/" class="">View More</a></button>
		<hr class="my-20 w-2/3 m-auto" />
	</div>

	<!-- review section -->
	<SectionHeader {...reviews} />
	<div class="flex justify-around flex-wrap p-5">
		<Reviewers />
	</div>

	<!-- about section -->
	<article class="bg-orange-900/10 h-fit py-10">
		<SectionHeader {...about} />
		<ul class="flex justify-center mt-16 items-center m-auto">
			{#each qualities as quality}
				<li>
					<h2 class="fade-in-out font-bold ff-serif text-xs w-11/12">{quality}</h2>
				</li>
			{/each}
		</ul>

		<section class="w-full py-8 md:py-16 lg:py-24">
			<div
				class="container grid items-center justify-center gap-8 px-4 md:px-6 lg:grid-cols-2 lg:gap-16"
			>
				<div class="space-y-4 text-[0.8em]/loose">
					<p class="">
						At our restaurant, we take pride in our rich history and commitment to delivering an
						exceptional dining experience. Founded in 1985, we've been serving the community with
						our unique blend of traditional and innovative cuisine, all while fostering a warm and
						inviting atmosphere.
					</p>
					<p>
						Our philosophy is simple: use the freshest, locally-sourced ingredients to create dishes
						that delight the senses and nourish the soul. From our signature dishes to our seasonal
						specials, every plate is crafted with passion and attention to detail.
					</p>
				</div>
				<div class="grid grid-cols-2 gap-4">
					<img
						src="../landing/heroImg.png"
						width="300"
						height="300"
						alt="Beautiful Burgers"
						class="rounded-lg object-cover"
						style="aspect-ratio: 300 / 300; object-fit: cover;"
					/>
					<img
						src="../landing/staunt.png"
						width="300"
						height="300"
						alt="Restaurant Atmosphere"
						class="rounded-lg object-cover"
						style="aspect-ratio: 300 / 300; object-fit: cover;"
					/>
					<img
						src="../landing/farming.png"
						width="300"
						height="300"
						alt="Farmers"
						class="rounded-lg object-cover"
						style="aspect-ratio: 300 / 300; object-fit: cover;"
					/>
					<img
						src="../landing/cheese.png"
						width="300"
						height="300"
						alt="Restaurant Team"
						class="rounded-lg object-cover"
						style="aspect-ratio: 300 / 300; object-fit: cover;"
					/>
				</div>
			</div>
		</section>
	</article>
</div>

<style>
	.home {
		margin: auto;
		max-width: 1440px;
		height: fit-content;
		background-color: #1c1b1f;
	}

	.hero-section {
		height: 70vh;
		background-color: #000000;
	}

	.text {
		width: 100%;
		font-size: clamp(4rem, 10vw, 9rem);
	}

	.links {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		gap: 5px;
		color: cornflowerblue;
	}

	@media (max-width: 767px) {
		.home {
			height: fit-content;
		}

		.hero-section {
			height: fit-content;
		}
	}

	.fade-in-out {
		animation: fadeInOut 15s infinite;
	}

	@keyframes fadeInOut {
		0% {
			opacity: 0;
		}
		50% {
			opacity: 1;
		}
		100% {
			opacity: 0;
		}
	}
</style>
