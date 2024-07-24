<script>
	export let reviewer;
	export let comment;
</script>

<div class="flex flex-col w-fit justify-center items-center text-dark">
	<div class="bg-dark w-fit rounded-full p-6">
		<svg
			xmlns="http://www.w3.org/2000/svg"
			width="100"
			height="100"
			fill="currentColor"
			class="bi bi-person-fill text-white"
			viewBox="0 0 16 16"
		>
			<path d="M3 14s-1 0-1-1 1-4 6-4 6 3 6 4-1 1-1 1zm5-6a3 3 0 1 0 0-6 3 3 0 0 0 0 6" />
		</svg>
	</div>
	<h2 class="fs-300 ff-serif text-center">{reviewer}</h2>
	<p class="w-[30ch] text-xs">
		{comment}
	</p>
</div>
