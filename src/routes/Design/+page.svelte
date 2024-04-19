<div class="box p-4 bg-dark">
	<h1 class="text-4xl">Design System</h1>

	<!-- colors -->
	<section>
		<h2 class="numbered-title"><span>01</span> colors</h2>

		<div class="flex flex-wrap">
			<div style="flex-grow: 1;">
				<div class="bg-base" style="padding: 3rem 1rem 1rem; border: 1px solid white;">#906A8C</div>

				<p><span class="text-accent">RGB</span> 203, 85, 16</p>
				<p><span class="text-accent">HSL</span> 22˚, 85%, 43%</p>
			</div>

			<div style="flex-grow: 1;">
				<div style="padding: 3rem 1rem 1rem; border: 1px solid white;">#242037</div>

				<p><span class="text-accent">RGB</span> 36, 32, 55</p>
				<p><span class="text-accent">HSL</span> 250˚, 27%, 17%</p>
			</div>

			<div style="flex-grow: 1;">
				<div class="bg-light text-dark" style="padding: 3rem 1rem 1rem; border: 1px solid white;">
					#E3DDBF
				</div>

				<p><span class="text-accent">RGB</span> 209 204 208</p>
				<p><span class="text-accent">HSL</span> 227˚, 221, 191</p>
			</div>

			<div style="flex-grow: 1;">
				<div class="bg-medium text-dark" style="padding: 3rem 1rem 1rem; border: 1px solid white;">
					#ECCE8E
				</div>

				<p><span class="text-accent">RGB</span> 236, 206, 142</p>
				<p><span class="text-accent">HSL</span> 41˚, 71%, 74%</p>
			</div>

			<div style="flex-grow: 1;">
				<div class="bg-accent text-dark" style="padding: 3rem 1rem 1rem; border: 1px solid white;">
					#C3C7A9
				</div>

				<p><span class="text-accent">RGB</span> 195, 199, 169</p>
				<p><span class="text-accent">HSL</span> 68˚, 21%, 72%</p>
			</div>
		</div>
	</section>

	<!-- typography -->
	<section id="typography" style="margin: 4rem 0;">
		<h2 class="numbered-title"><span>02</span> typography</h2>

		<div class="flex flex-wrap md:flex-nowrap">
			<div class="flow" style="flex-basis: 100%; --flow-space: 4rem;">
				<div>
					<p class="text-accent">Heading 1 - Fugaz One - 150px</p>
					<p class="fs-900 ff-serif uppercase">Fresh</p>
				</div>

				<div>
					<p class="text-accent">Heading 2 - Fugaz One - 100px</p>
					<p class="fs-800 ff-serif uppercase">Flavors</p>
				</div>

				<div>
					<p class="text-accent">Heading 3 - Fugaz One - 56px</p>
					<p class="fs-700 ff-serif uppercase">This day & The Next</p>
				</div>

				<div>
					<p class="text-accent">Heading 4 - Fugaz One - 32px</p>
					<p class="fs-600 ff-serif uppercase">Tasty and Delicious</p>
				</div>

				<div>
					<p class="text-accent">Heading 5 - Prosto One - 28px - 4.75 Character Space</p>
					<p class="text-accent fs-500 ff-sans-normal uppercase letter-spacing-1">
						Eat Ours and never need another!
					</p>
				</div>
			</div>
			<div class="flow" style="flex-basis: 100%">
				<div>
					<p class="text-accent">Subheading 1 - Fugaz One - 28px</p>
					<p class="fs-500 ff-serif uppercase">Starters</p>
				</div>
				<div>
					<p class="text-accent">Subheading 2 - Comfortaa Variable - 14px - 2.35 Character Space</p>
					<p class="fs-200 ff-sans letter-spacing-3">Vegan Option</p>
				</div>
				<div>
					<p class="text-accent">Nav Text - Comfortaa Variable - 16px - 2.7 Character Space</p>
					<p class="fs-300 ff-sans letter-spacing-2">About Us</p>
				</div>
				<div>
					<p class="text-accent">Body Text - Prosto One - 16px - 1.5 Character Space</p>
					<p>
						Started one two way back. Best combos here and there, come and try us. This is pure filler text so use your imaination. Sides and drinks. The more the merrier, dare us if you may. The world is yours.
					</p>
				</div>
			</div>
		</div>
	</section>

	<!-- interaction -->
	<section>
		<h2 class="numbered-title"><span>03</span> Interactive Elements</h2>

		<!-- navigation -->
		<div>
			<nav>
				<ul class="primary-navigation flex underline-indicators ff-sans" style="--gap: 4rem;">
					<li class="active">
						<a class="uppercase text-light letter-spacing-2" href="#"><span>01</span>Active</a>
					</li>
					<li>
						<a class="uppercase text-light letter-spacing-2" href="#"><span>02</span>Hover</a>
					</li>
					<li><a class="uppercase text-light letter-spacing-2" href="#"><span>03</span>Idle</a></li>
				</ul>
			</nav>
		</div>

		<div class="flex flex-col">
			<!-- explore button -->
			<div style="margin-top: 5rem;">
				<a href="#" class="large-button uppercase text-dark bg-light">Explore</a>
			</div>

			<!-- tabs -->
			<div class="flow" style="--flow-space: 4rem;">
				<div class="tab-list underline-indicators flex">
					<button
						aria-selected="true"
						class="uppercase ff-sans text-accent bg-dark letter-spacing-2">Moon</button
					>
					<button
						aria-selected="false"
						class="uppercase ff-sans text-accent bg-dark letter-spacing-2">Jupiter</button
					>
					<button
						aria-selected="false"
						class="uppercase ff-sans text-accent bg-dark letter-spacing-2">Pluto</button
					>
				</div>

				<!-- dots -->
				<div class="dot-indicators flex">
					<button aria-selected="true"><span class="sr-only"></span></button>
					<button aria-selected="false"><span class="sr-only"></span></button>
					<button aria-selected="false"><span class="sr-only"></span></button>
				</div>
				<!-- numbers
				<div class="flex">
					<div class="flow" style="--flow-space: 4rem;">
						<div class="numbers">
							<p class="text-accent bg-light">1</p>
						</div>
						<div>
							<p class="text-light">2</p>
						</div>
						<div>
							<p class="text-light">3</p>
						</div>
					</div>
				</div> -->
			</div>
		</div>
	</section>

	<!-- component library -->
	<section>
		<h2 class="numbered-title"><span>04</span>Component Library</h2>
	</section>
</div>

<style>
	section {
		margin: 4rem 0;
	}
</style>
