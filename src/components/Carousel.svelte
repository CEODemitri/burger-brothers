<script>
	import { onMount } from 'svelte';
	import Slick from 'slick-slider';

	export let items;

	let slick;

	onMount(() => {
		slick = new Slick('.carousel', {
			infinite: true,
			slidesToShow: 3,
			slidesToScroll: 1,
			arrows: true,
			dots: true,
			responsive: [
				{
					breakpoint: 1024,
					settings: {
						slidesToShow: 2,
						slidesToScroll: 1
					}
				},
				{
					breakpoint: 600,
					settings: {
						slidesToShow: 1,
						slidesToScroll: 1
					}
				}
			]
		});
	});

	onDestroy(() => {
		if (slick) {
			slick.destroy();
		}
	});
</script>

<div class="carousel">
	{#each items as item}
		<div class="slide">
			<slot name="item" {item} />
		</div>
	{/each}
</div>

<style>
	.carousel {
		/* Add your carousel styles here */
	}

	.slick-prev,
	.slick-next {
		/* Add your arrow button styles here */
	}

	.slick-dots {
		/* Add your dot button styles here */
	}
</style>
