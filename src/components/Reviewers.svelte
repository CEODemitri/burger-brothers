<script>
	import { onMount } from 'svelte';

	let slides = [
		{
			name: 'John Doe',
			image: '../review/man1.jpg',
			text: 'This product is amazing! It has exceeded all my expectations\n and has become an essential part of my daily routine. Highly\n recommended!',
			ratings: 3
		},
		{
			name: 'Alice Smith',
			image: '../review/woman1.jpg',
			text: "I'm absolutely in love with this product! It's not only\n beautiful but also incredibly functional. I highly recommend\n it to anyone looking for a top-notch solution.",
			ratings: 4
		},
		{
			name: 'Michael Johnson',
			image: '../review/man2.jpg',
			text: "This is hands down the best product I've ever owned. The\n quality is outstanding, and the design is simply\n breathtaking. I couldn't be happier with my purchase!",
			ratings: 5
		},
		{
			name: 'Emily Martinez',
			image: '../review/man3.jpg',
			text: "I'm really impressed with this product. It's well-made,\n easy to use, and has exceeded my expectations. I would\n definitely recommend it to anyone looking for a reliable and\n high-quality solution.",
			ratings: 3
		},
		{
			name: 'Jessica Williams',
			image: '../review/woman2.jpg',
			text: "I'm so glad I found this product! It's been a game-changer\n for me and has made my life so much easier. I highly\n recommend it to anyone looking for a top-notch solution.",
			ratings: 4
		}
	];

	let currentIndex = 0;
	let carousel;

	function prevSlide() {
		currentIndex = currentIndex > 0 ? currentIndex - 1 : slides.length - 1;
		updateCarousel();
	}

	function nextSlide() {
		currentIndex = currentIndex < slides.length - 1 ? currentIndex + 1 : 0;
		updateCarousel();
	}

	function updateCarousel() {
		if (carousel) {
			const slideWidth = carousel.offsetWidth / 3; // Display 3 slides at a time
			const offset = -currentIndex * slideWidth;
			carousel.style.transform = `translateX(${offset}px)`;
		}
	}

	onMount(() => {
		updateCarousel();
		// Optional: Automatically advance slides every few seconds
		const interval = setInterval(nextSlide, 5000); // 5 seconds

		return () => clearInterval(interval); // Clean up interval on component destroy
	});
</script>

<div class="carousel">
	<div class="carousel__slides" bind:this={carousel}>
		{#each slides as slide}
			<div class="carousel__slide">
				<article
					class="flex flex-col mx-4 border border-slate-600 rounded-md px-8 py-4 min-w-fit relative"
				>
					<img src={slide.image} alt={slide.name} class="rounded-full w-32 h-32 p" />
					<div class="carousel__text">
						<h2 class="fs-300 ff-serif text-center text-orange-400">{slide.name}</h2>
						<p class="text-sm">{slide.text}</p>
						<p class="absolute top-4 left-60 sm:left-[16rem] text-blue-300">
							{slide.ratings} stars
						</p>
					</div>
				</article>
			</div>
		{/each}
	</div>
	<div class="carousel__controls">
		<button class="carousel__control carousel__control--prev" on:click={prevSlide}>
			<i class="bi bi-chevron-left"></i>
			<span class="sr-only">Previous slide</span>
		</button>
		<button class="carousel__control carousel__control--next" on:click={nextSlide}>
			<i class="bi bi-chevron-right"></i>
			<span class="sr-only">Next slide</span>
		</button>
	</div>
</div>

<style>
	.carousel {
		position: relative;
		overflow: hidden;
		width: 100%;
		margin: 4em 0;
	}

	.carousel__slides {
		display: flex;
		transition: transform 0.3s ease-in-out;
		width: 100%;
	}

	.carousel__slide {
		flex: 1 0 100%; /* Adjust for 1 slide visible by default */
		box-sizing: border-box;
		padding: 0 0.5rem; /* Adds padding around each slide */
	}

	.carousel__image {
		width: 100%;
		border-radius: 8px;
		margin-bottom: 0.5rem;
		object-fit: cover; /* Ensures image covers the container without distortion */
	}

	.carousel__text {
		font-size: 0.875rem;
		line-height: 1.4;
		overflow-wrap: break-word; /* Ensures long words break properly */
		word-wrap: break-word; /* For compatibility */
	}

	.carousel__controls {
		position: absolute;
		top: 50%;
		transform: translateY(-50%);
		display: flex;
		width: 100%;
		justify-content: space-between;
		z-index: 10;
	}

	.carousel__control {
		background: #fff;
		border: 1px solid #ddd;
		border-radius: 9999px;
		display: flex;
		align-items: center;
		justify-content: center;
		width: 2rem;
		height: 2rem;
		cursor: pointer;
	}

	.carousel__control--prev {
		left: 1rem;
	}

	.carousel__control--next {
		right: 1rem;
	}

	@media (min-width: 600px) {
		.carousel__slide {
			flex: 1 0 50%; /* Two slides visible on medium screens */
		}
	}

	@media (min-width: 1024px) {
		.carousel__slide {
			flex: 1 0 33.33%; /* Three slides visible on large screens */
		}
	}
</style>
