<div class="text-dark p-5">
	<h1 class="ff-sans">Design System</h1>

	<!-- layout -->
	<!-- <section class="SECTION CONTAINER">
		<h2><span>ROMAN NUM</span>SECTION TITLE</h2>

		<div class="SECTION EXAMPLE">
			<article>
				<section class="EXAMPLE 1"></section>

				<section>
					<p class="NAME"></p>
					<p class="CODE"></p>
				</section>
			</article>
		</div>
	</section> -->

	<section class="p-8">
		<h2><span class="text-sm">I</span>COLORS</h2>

		<div class="flex justify-around p-2">
			<!-- 1 color -->
			<article class="flex flex-col">
				<!-- color -->
				<section class="bg-light h-28 w-28 rounded-full"></section>

				<!-- name and description -->
				<section class="text-sm">
					<p>Light</p>
					<p>50, 39%, 82%</p>
				</section>
			</article>

			<!-- 1 color -->
			<article class="flex flex-col">
				<!-- color -->
				<section class="bg-medium h-28 w-28 rounded-full"></section>

				<!-- name and description -->
				<section class="text-sm">
					<p>Medium</p>
					<p>41, 71%, 74%</p>
				</section>
			</article>

			<!-- 1 color -->
			<article class="flex flex-col">
				<!-- color -->
				<section class="bg-dark h-28 w-28 rounded-full"></section>

				<!-- name and description -->
				<section class="text-sm">
					<p>Dark</p>
					<p>250, 27%, 17%</p>
				</section>
			</article>

			<!-- 1 color -->
			<article class="flex flex-col">
				<!-- color -->
				<section class="bg-accent h-28 w-28 rounded-full"></section>

				<!-- name and description -->
				<section class="text-sm">
					<p>Accent</p>
					<p>68, 21%, 72%</p>
				</section>
			</article>

			<!-- 1 color -->
			<article class="flex flex-col">
				<!-- color -->
				<section class="bg-action h-28 w-28 rounded-full"></section>

				<!-- name and description -->
				<section class="text-sm">
					<p>Action</p>
					<p>22, 85%, 43%</p>
				</section>
			</article>
		</div>
	</section>

	<section class="p-8">
		<h2><span class="text-sm">II</span>TYPOGRAPHY</h2>

		<div class="flex">
			<div class="p-10 div">
				<article>
					<section class="text-sm flex w-2/3 justify-between">
						<p>Heading 1</p>
						<p>Fugaz One</p>
						<p>Serif</p>
						<p>96px</p>
						<p>LS3</p>
					</section>

					<section class="text-[96px] ff-serif">
						<h1 class="letter-spacing-3">Burgers</h1>
					</section>
				</article>

				<article>
					<section class="text-sm flex w-2/3 justify-between">
						<p>Heading 2</p>
						<p>Fugaz One</p>
						<p>Serif</p>
						<p>80px</p>
						<p>LS2</p>
					</section>

					<section class="text-[80px] ff-serif">
						<h2 class="letter-spacing-2">Natural Source</h2>
					</section>
				</article>

				<article>
					<section class="text-sm flex w-2/3 justify-between">
						<p>Heading 3</p>
						<p>Fugaz One</p>
						<p>Serif</p>
						<p>64px</p>
						<p>LS3</p>
					</section>

					<section class="text-[64px] ff-serif">
						<h3 class="letter-spacing-3">Fantastic</h3>
					</section>
				</article>

				<article>
					<section class="text-sm flex w-2/3 justify-between">
						<p>Heading 4</p>
						<p>Fugaz One</p>
						<p>Serif</p>
						<p>52px</p>
						<p>LS4</p>
					</section>

					<section class="text-[52px] ff-serif">
						<h4 class="letter-spacing-4">Fresh Taste</h4>
					</section>
				</article>

				<article>
					<section class="text-sm flex w-2/3 justify-between">
						<p>Heading 5</p>
						<p>Comfortaa Variable</p>
						<p>Sans</p>
						<p>40px</p>
					</section>

					<section class="text-[40px] ff-serif">
						<h5>Thank You</h5>
					</section>
				</article>
			</div>

			<!-- typography second column -->
			<div class="p-10">
				<article>
					<section class="text-sm flex w-2/3 justify-between">
						<p>Heading 5</p>
						<p>Comfortaa Variable</p>
						<p>Sans</p>
						<p>40px</p>
					</section>

					<section class="text-[40px] ff-serif">
						<h5>Thank You</h5>
					</section>
				</article>
			</div>
		</div>
	</section>
</div>

<style>
	h1,
	h2,
	h3,
	h4,
	h5 {
		padding: 0;
		margin: 0;
		box-sizing: content-box;
	}

	h2 span {
		margin-right: 0.5em;
		background-color: orange;
		padding: 0.6em;
		border-radius: 7px 0 7px 0;
	}

	.div {
		display: flex;
		flex-direction: column;
		row-gap: 40px;
	}
</style>
