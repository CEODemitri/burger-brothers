<script>
	export let pill;
	export let title;
	export let description;
</script>

<div class="text-center text-white flex flex-col mb-6 mt-20">
	<h1 class="text-slate-300 ff-body letter-spacing-3 text-[32px] md:text-[64px] ff-serif font-bold">
		{title}
	</h1>
	<p class="pill p-5 ff-serif">{pill}</p>
	<p class="fs-200 ff-sans w-[30ch] md:w-[55ch] m-auto text-wrap">{description}</p>
</div>

<style>
	p.pill {
		background-color: hsl(250, 27%, 17%);
		color: #fff;
		width: 200px;
		padding: 5px;
		border-radius: 15px;
		margin: auto;
	}
</style>
