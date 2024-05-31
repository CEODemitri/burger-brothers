<script>
	import '@fontsource-variable/comfortaa';
	import '@fontsource/fugaz-one';

	export let src;
	export let price;
	export let name;
	export let description;
</script>

<div class="w-72 bg-[#D6CFA9] text-[#232135] relative">
	<img {src} alt={name} srcset="" class="rounded-md" />
	<div class="info h-fit mb-12 p-2">
		<h2 class="text-2xl">{name}</h2>
		<p class="text-xs text-neutral-500">{description}</p>
		<button class="bg-action text-white px-5 py-2 mt-5 ml-40 rounded-md text-sm">Add Item</button>

		<p class="absolute top-0 right-0 pr-5 pt-2 text-white">{price}</p>
	</div>
</div>
