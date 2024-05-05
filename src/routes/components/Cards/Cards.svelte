<script>
	import '@fontsource-variable/comfortaa';
	import '@fontsource/fugaz-one';

	export let src;
	export let price;
	export let name;
	export let description;
</script>

<div class="w-72 bg-[#D6CFA9] text-[#232135]">
	<img {src} alt="" srcset="" class="rounded-md" />
	<div class="info h-36 mb-12">
		<h2 class="text-2xl">{name}</h2>
		<p class="text-xs">{description}</p>
		<button class="bg-[#BC5C28] text-white px-5 py-2 rounded-md text-sm">Add Item</button>

		<p>{price}</p>
	</div>
</div>
