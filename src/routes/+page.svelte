<script>
	// Supports weights 300-700
	import Cards from '../components/Cards/Cards.svelte';
	import Review from '../components/Review.svelte';
	import SectionHeader from '../components/SectionHeader.svelte';

	// starter items
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

	// entree items
	const entree1 = {
		/* ... */
	};
	const entree2 = {
		/* ... */
	};
	const entree3 = {
		/* ... */
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
		{ name: 'Starters', path: '#starters', content: [melt, pork, breakfast] },
		{ name: 'Entrees', path: '#entrees', content: [entree1, entree2, entree3] },
		{ name: 'Drinks', path: '#drinks', content: [drink1, drink2, drink3] },
		{ name: 'Desserts', path: '#desserts', content: [dessert1, dessert2, dessert3] }
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
</script>

<div class="home">
	<div class="hero-section">
		<div class="overlay"></div>

		<article class="ml-10 pt-6 text-white">
			<h1 class="text-5xl md:text-7xl lg:text-[96px]leading-3 relative ff-serif">
				Burger Brothers
			</h1>
			<p class="lg:w-[966px] text-sm p-1 mt-5">
				Discover a burger experience like no other at Burger Brothers. We are more than just a
				restaurant; we are a celebration of all things delicious, juicy, and perfectly crafted
				between two buns. From our hand-selected ingredients to our passion for flavor, every burger
				tells a story of quality and satisfaction.
			</p>
		</article>
	</div>

	<!-- call to action space -->
	<div class="menu hidden sm:block h-fit">
		<section class="triangle"></section>
		<section class="box max-w-screen-md max-h-44 fs-300 flex items-center">
			<p class="links border-r-2">
				<!-- icon -->
				<svg
					xmlns="http://www.w3.org/2000/svg"
					fill="currentColor"
					class="bi bi-people w-70 h-10"
					viewBox="0 0 16 16"
				>
					<path
						d="M15 14s1 0 1-1-1-4-5-4-5 3-5 4 1 1 1 1zm-7.978-1L7 12.996c.001-.264.167-1.03.76-1.72C8.312 10.629 9.282 10 11 10c1.717 0 2.687.63 3.24 1.276.593.69.758 1.457.76 1.72l-.008.002-.014.002zM11 7a2 2 0 1 0 0-4 2 2 0 0 0 0 4m3-2a3 3 0 1 1-6 0 3 3 0 0 1 6 0M6.936 9.28a6 6 0 0 0-1.23-.247A7 7 0 0 0 5 9c-4 0-5 3-5 4q0 1 1 1h4.216A2.24 2.24 0 0 1 5 13c0-1.01.377-2.042 1.09-2.904.243-.294.526-.569.846-.816M4.92 10A5.5 5.5 0 0 0 4 13H1c0-.26.164-1.03.76-1.724.545-.636 1.492-1.256 3.16-1.275ZM1.5 5.5a3 3 0 1 1 6 0 3 3 0 0 1-6 0m3-2a2 2 0 1 0 0 4 2 2 0 0 0 0-4"
					/>
				</svg>
				<span> Catering </span>
			</p>
			<p class="links border-r-2">
				<svg
					xmlns="http://www.w3.org/2000/svg"
					fill="currentColor"
					class="bi bi-receipt-cutoff w-70 h-10"
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
					class="bi bi-pin-map w-70 h-10"
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
		</section>
	</div>

	<!-- popular menu -->
	<SectionHeader {...popular} />
	<div class="text-dark">
		<article class="flex justify-center ff-sans m-5 fs-400 flex-wrap">
			{#each tabs as tab}
				<a
					href={tab.path}
					on:click|preventDefault={() => selectTab(tab)}
					class="border px-6 py-1 border-purple-950 rounded-md mx-3">{tab.name}</a
				>
			{/each}
		</article>
	</div>

	<article class="p-5 flex flex-wrap justify-center">
		{#each selectedTab.content as item}
			<Cards {...item} />
		{/each}
	</article>

	<!-- review section -->
	<SectionHeader {...reviews} />
	<div class="flex justify-around flex-wrap p-5">
		<Review
			reviewer="Emily T."
			comment="'Delicious burgers with top-notch ingredients! My favorite spot for a juicy, satisfying meal.'"
		/>
		<Review
			reviewer="Michael S."
			comment="'The variety of flavors is amazing. Every burger is a masterpiece!'"
		/>
		<Review
			reviewer="Florida E."
			comment="'Great atmosphere and friendly service. Perfect place to enjoy a burger with friends.'"
		/>
	</div>

	<!-- about section -->
	<SectionHeader {...about} />
	<p class="text-black w-[25ch] md:w-[75ch] m-auto text-md p-3">
		Located conveniently in the heart of Metropolis, Burger Brothers invites you to indulge in the
		ultimate burger experience. Whether you dine in, take out, or order online, our commitment to
		exceptional food and service ensures every visit is a treat. Ready to embark on a burger journey
		like no other? Join us at Burger Brothers and taste the difference quality makes. Your taste
		buds will thank you.
	</p>
</div>

<style>
	.home {
		margin: auto;
		max-width: 1440px;
		height: fit-content;
		background: linear-gradient(180deg, #fff, #e2ddc2);
	}

	@media (max-width: 767px) {
		.home {
			height: 4400px;
		}
	}

	.hero-section {
		max-width: 1440px;
		height: 600px;
		background: url('../landing/heroImg.png');
		background-position: center;
		background-repeat: no-repeat;
		position: relative;
		margin: auto;
	}

	.overlay {
		background-color: rgba(0, 0, 0, 0.4);
		width: 100%;
		height: 100%;
		position: absolute;
	}

	.menu {
		margin-bottom: -150px;
	}

	.triangle {
		width: 0;
		height: 0;
		border-left: 40px solid transparent;
		border-right: 40px solid transparent;
		border-bottom: 60px solid #232135;
		position: relative;
		top: -150px;
		margin: auto;
	}

	.box {
		width: 60vw;
		min-width: fit-content;
		padding: 0 13px;
		height: 15vh;
		background-color: #232135;
		position: relative;
		top: -150px;
		margin: auto;
		border-radius: 30px 0 30px 0;
		display: grid;
		grid-template-columns: repeat(3, 1fr);
		text-align: center;
	}

	.links {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		gap: 5px;
	}
</style>
