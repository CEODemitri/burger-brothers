<script>
	// Supports weights 300-700
	import Cards from './components/Cards/Cards.svelte';
	import Carousel from './components/Home/Carousel.svelte';

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

	<div class="menu hidden sm:block">
		<section class="triangle"></section>
		<section class="box max-w-screen-md">
			<span class="links text-xl">Catering</span>
			<span class="links text-xl">Order Online</span>
			<span class="links text-xl">Find Location</span>
		</section>
	</div>

	<Cards {...melt} />
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

	h1,
	h2 {
		font-family: 'Fugaz One', system-ui;
	}

	p {
		font-family: 'Comfortaa Variable', sans-serif;
		line-height: 24px;
	}
</style>
