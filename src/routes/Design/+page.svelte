<div class="box p-4">
	<h1 class="text-4xl">Design System</h1>

	<!-- colors -->
	<section>
		<h2 class="numbered-title"><span>01</span> colors</h2>

		<div class="flex">
            <div style="flex-grow: 1;">
				<div class="bg-base" style="padding: 3rem 1rem 1rem; border: 1px solid white;">#906A8C</div>

				<p><span class="text-accent">RGB</span> 203, 85, 16 </p>
				<p><span class="text-accent">HSL</span> 22, 85%, 43% </p>
			</div>

			<div style="flex-grow: 1;">
				<div style="padding: 3rem 1rem 1rem; border: 1px solid white;">#1A1419</div>

				<p><span class="text-accent">RGB</span> 26 20 25</p>
				<p><span class="text-accent">HSL</span> 310˚, 15%, 9%</p>
			</div>

			<div style="flex-grow: 1;">
				<div class="bg-light text-dark" style="padding: 3rem 1rem 1rem; border: 1px solid white;">
					#D1CCD0
				</div>

				<p><span class="text-accent">RGB</span> 209 204 208</p>
				<p><span class="text-accent">HSL</span> 312˚, 6%, 81%</p>
			</div>
		</div>
	</section>

	<!-- typography -->
	<section id="typography" style="margin: 4rem 0;">
		<h2 class="numbered-title"><span>02</span> typography</h2>

		<div class="flex">
			<div class="flow" style="flex-basis: 100%; --flow-space: 4rem;">
				<div>
					<p class="text-accent">Heading 1 - Merriweather Regular - 150px</p>
					<p class="fs-900 ff-serif uppercase">Earth</p>
				</div>

				<div>
					<p class="text-accent">Heading 2 - Merriweather Regular - 100px</p>
					<p class="fs-800 ff-serif uppercase">Venus</p>
				</div>

				<div>
					<p class="text-accent">Heading 3 - Merriweather Regular - 56px</p>
					<p class="fs-700 ff-serif uppercase">Jupiter & Saturn</p>
				</div>

				<div>
					<p class="text-accent">Heading 4 - Merriweather Regular - 32px</p>
					<p class="fs-600 ff-serif uppercase">Uranus, Neptune, Pluto</p>
				</div>

				<div>
					<p class="text-accent">Heading 5 - Barlow - 28px - 4.75 Character Space</p>
					<p class="text-accent fs-500 ff-sans-normal uppercase letter-spacing-1">
						So you want to travel space?
					</p>
				</div>
			</div>
			<div class="flow" style="flex-basis: 100%">
				<div>
					<p class="text-accent">Subheading 1 - Merriweather Regular - 28px</p>
					<p class="fs-500 ff-serif uppercase">384, 400 km</p>
				</div>
				<div>
					<p class="text-accent">Subheading 2 - Barlow - 14px - 2.35 Character Space</p>
					<p class="fs-200 ff-sans-normal letter-spacing-3">Avg. Distance</p>
				</div>
				<div>
					<p class="text-accent">Nav Text - Barlow - 16px - 2.7 Character Space</p>
					<p class="fs-300 ff-sans-normal letter-spacing-2">Europa</p>
				</div>
				<div>
					<p class="text-accent">Body Text - Barlow - 16px - 1.5 Character Space</p>
					<p>
						Europa is the second largest and most massive of the four inner planets of the Solar
						System, and the largest in terms of volume and mass. It is a gas giant with an
						atmosphere of nitrogen, oxygen, and other hydrocarbons, with a surface pressure of about
						92 times that of Earth, and a temperature of -148.8 °C.
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
				<ul class="primary-navigation flex underline-indicators" style="--gap: 4rem;">
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

		<div class="flex">
			<div style="margin-top: 5rem;">
				<!-- explore button -->
				<a href="#" class="large-button uppercase ff-serif fs-600 text-dark bg-light">Explore</a>
			</div>

			<div class="flow" style="margin-bottom: 50vh; --flow-space: 4rem;">
				<!-- tabs -->
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
				<!-- numbers -->
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
				</div>
			</div>
		</div>
	</section>
</div>

<style>
    section {
        margin: 4rem 0;
    }
</style>
