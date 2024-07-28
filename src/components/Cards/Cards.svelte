<script>
	import '@fontsource-variable/comfortaa';
	import '@fontsource/fugaz-one';

	export let src;
	export let price;
	export let name;
	export let description;
</script>

<div class="w-72 text-[#232135] relative mb-20">
	<img {src} alt={name} srcset="" class="rounded-md" />
	<div class="info h-32 mb-6 p-2 bg-[#D6CFA9] rounded-md w-[250px] absolute top-64 left-5">
		<h2 class="text-xl ff-serif">{name}</h2>
		<p class="text-xs text-neutral-500 ff-body">{description}</p>
		<button class="bg-action text-white px-4 py-1 mt-1 ml-40 rounded-md text-[10px] shadow-xl"
			>Add Item</button
		>

		<p class="absolute top-0 right-0 mr-2 pt-2 text-white">{price}</p>
	</div>
</div>
