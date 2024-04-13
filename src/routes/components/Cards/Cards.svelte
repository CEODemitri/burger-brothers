<script>
	import '@fontsource-variable/comfortaa';
	import '@fontsource/fugaz-one';

	export let src;
	export let price;
	export let name;
	export let description;
</script>

<div class="flex flex-col space-y-2 p-2 text-left">
	<img
		{src}
		width="400"
		height="400"
		alt="Burger"
		class="aspect-square overflow-hidden rounded-xl object-cover object-center"
	/>
	<div class="space-y-2">
		<p class="text-sm text-gray-500">{price}</p>
		<h3 class="text-xl font-bold text-yellow-600">{name}</h3>
		<p class="w-72 text-gray-600">{description}</p>

		<form action="" class="flex justify-center items-center gap-7">
			<div class="grid gap-2">
				<label
					class="font-medium peer-disabled:cursor-not-allowed peer-disabled:opacity-70 text-sm"
					for="quantity"
				>
					Quantity
				</label>
				<button
					type="button"
					role="combobox"
					aria-controls="radix-:r3:"
					aria-expanded="false"
					aria-autocomplete="none"
					dir="ltr"
					data-state="closed"
					class="flex h-7 items-center justify-between rounded-md border border-input bg-background px-3 text-sm ring-offset-background placeholder:text-muted-foreground focus:outline-none focus:ring-2 focus:ring-ring focus:ring-offset-2 disabled:cursor-not-allowed disabled:opacity-50 w-18"
				>
					<span style="pointer-events: none;">1</span>
					<svg
						xmlns="http://www.w3.org/2000/svg"
						width="18"
						height="24"
						viewBox="0 0 18 24"
						fill="none"
						stroke="currentColor"
						stroke-width="2"
						stroke-linecap="round"
						stroke-linejoin="round"
						class="h-4 w-4 opacity-50"
						aria-hidden="true"
					>
						<path d="m6 9 6 6 6-6"></path>
					</svg>
				</button>
			</div>
			<button
				class="inline-flex items-center justify-center whitespace-nowrap text-sm font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 bg-black text-white hover:bg-primary/90 h-11 rounded-md px-8"
			>
				Add to cart
			</button>
		</form>
	</div>
</div>

<style>
	h3 {
		font-family: 'Fugaz One', cursive;
		font-size: 2em;
	}

	button {
		font-family: 'Fugaz One', cursive;
	}

	p {
		font-family: 'Comfortaa Variable', cursive;
		font-size: 0.8em;
	}
</style>
