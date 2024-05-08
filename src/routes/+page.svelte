<script>
	// Supports weights 300-700
	import Cards from '../components/Cards/Cards.svelte';
	import SectionHeader from '../components/SectionHeader.svelte';

	const melt = {
		src: '/specials/grill-quinoa.png',
		price: 85.99,
		name: 'Grilled Quinoa',
		description:
			'You smell me. Quinoa from the untapped valleys across this earth. Finest ingredients.'
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
		description: 'You feel me. All natural eggs paired elegantly with fresh cut hashbrowns, twice.'
	};

	// popular menu
	const tabs = [
		{ name: 'Starters', path: '#starters' },
		{ name: 'Entrees', path: '#entrees' },
		{ name: 'Drinks', path: '#drinks' },
		{ name: 'Desserts', path: '#desserts' }
	];

	const popular = {
		pill: 'Burgertastic',
		title: 'Popular Menu',
		description: 'Lorem ipsum dolor sit am, consect et ning ut Lorem ipsum dolor sit am. Ere metus in ning versert but auctor limere vel'
	}
</script>

<div class="home">
	<div class="hero-section">
		<div class="overlay"></div>

		<article class="hero-text ml-10 pt-10">
			<h1 class="text-white text-7xl lg:text-[96px]">Burger Brothers</h1>
			<p class="lg:w-[966px] text-md p-1 mt-5">
				Lorem ipsum dolor sit amet consectetur. Placerat sed integer fusce venenatis. Lacinia
				pretium magna maecenas quis. Egestas tortor quam cursus tellus.
			</p>
		</article>
	</div>

	<!-- call to action space -->
	<div class="menu hidden sm:block h-fit">
		<section class="triangle"></section>
		<section class="box max-w-screen-md fs-300 flex items-center">
			<span class="links">Catering</span>
			<span class="links">Order Online</span>
			<span class="links">Find Location</span>
		</section>
	</div>

	<!-- popular menu -->
	<SectionHeader {...popular}/>
	<div class="text-dark">
		<article class="flex justify-center ff-sans m-5 fs-400">
			{#each tabs as tab}
				<a href={tab.path}>{tab.name}</a>
			{/each}
		</article>
	</div>

	<article class="p-5 flex flex-wrap justify-center">
		<Cards {...melt} />
		<Cards {...pork} />
		<Cards {...breakfast} />
	</article>
</div>

<style>
	.home {
		margin: auto;
		max-width: 1440px;
		height: 3080px;
		background: linear-gradient(180deg, #fff, #e2ddc2);
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

	.hero-text {
		text-shadow: 5px 10px 10px black;
	}

	.overlay {
		background-color: rgba(0, 0, 0, 0.6);
		height: 100%;
		position: absolute;
	}

	.menu {
		margin-bottom: -90px;
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
		height: 20vh;
		background-color: #232135;
		position: relative;
		top: -150px;
		margin: auto;
		border-radius: 30px 0 30px 0;
		display: grid;
		grid-template-columns: repeat(3, 1fr);
		text-align: center;
	}
</style>
