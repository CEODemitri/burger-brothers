<script>
	export let item; // Receive item data as a prop
</script>

<div class="card min-w-[480px]">
	<img src={item.src} alt={item.name} class="w-full h-48 object-cover" />
	<div class="p-4">
		<h2 class="text-lg font-semibold">{item.name}</h2>
		<p class="text-gray-500">{item.description}</p>
		<div class="flex justify-between items-center mt-4">
			<span class="text-lg font-semibold">${item.price.toFixed(2)}</span>
			<button class="bg-gray-900 text-white px-4 py-2 rounded">Add to Cart</button>
		</div>
	</div>
</div>

<style>
	.card {
		@apply shadow-md rounded-lg overflow-hidden;
	}
</style>
