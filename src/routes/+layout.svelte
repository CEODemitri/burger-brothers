<script>
	import '../app.css';
	import '@fontsource/hammersmith-one';
	import '@fontsource/finger-paint';
</script>

<div class="navbar bg-[#000] m-auto px-8">
	<div class="navbar-start">
		<nav class="flex gap-4 sm:gap-6 text-dark uppercase items-center">
			<svg
				width="36"
				height="16"
				viewBox="0 0 46 36"
				fill="none"
				xmlns="http://www.w3.org/2000/svg"
			>
				<path d="M0 3H46" stroke="#BC5C28" stroke-width="4" />
				<path d="M0 18H46" stroke="#BC5C28" stroke-width="4" />
				<path d="M0 33H46" stroke="#BC5C28" stroke-width="4" />
			</svg>

			<a
				class="hover:underline underline-offset-4 hover:scale-105 hover:font-extrabold hidden md:block"
				href="/Menu"
				rel="ugc"
			>
				Menu
			</a>
			<a
				class="hover:underline underline-offset-4 hover:scale-105 hover:font-extrabold hidden md:block"
				href="/Services"
				rel="ugc"
			>
				Services
			</a>
			<a
				class="hover:underline underline-offset-4 hover:scale-105 hover:font-extrabold hidden md:block"
				href="/About"
				rel="ugc"
			>
				About
			</a>
			<a
				class="hover:underline underline-offset-4 hover:scale-105 hover:font-extrabold hidden md:block"
				href="/Events"
				rel="ugc"
			>
				FAQ
			</a>
		</nav>
	</div>
	<div class="navbar-center">
		<a class="flex items-center justify-center" href="/" rel="ugc">
			<figure>
				<img src="../logos/noBg.png" alt="" class="w-16 ml-40 md:ml-0" />
				<figcaption>
					<h1 class="text-2xl font-bold text-gray-900 sr-only">Burger Brothers Logo</h1>
				</figcaption>
			</figure>
			<span class="sr-only">Burger Brothers</span>
		</a>
	</div>
	<div class="hidden md:flex navbar-end">
		<button class="btn btn-ghost btn-circle">
			<svg
				xmlns="http://www.w3.org/2000/svg"
				class="h-5 w-5"
				fill="none"
				viewBox="0 0 24 24"
				stroke="currentColor"
			>
				<path
					stroke-linecap="round"
					stroke-linejoin="round"
					stroke-width="2"
					d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"
				/>
			</svg>
		</button>
		<button class="bg-action text-xs md:text-sm px-5 py-2 ff-serif">Order Online</button>
	</div>
</div>
<slot />

<footer class="footer bg-dark text-neutral-content p-10 m-auto">
	<aside>
		<img alt="small logo" src="../logos/noBg.png" class="w-36" />
		<p>
			Burger Brothers, LLC
			<br />
			Premium burger Eatery since 1985
			<span class="block text-xs mt-4"
				>Our commitment to quality extends from farm to table, ensuring you enjoy food that's good
				for you and the planet.</span
			>
		</p>
	</aside>
	<nav>
		<h6 class="footer-title">Social</h6>
		<div class="grid grid-flow-col gap-4">
			<a href="/" class="">
				<svg
					xmlns="http://www.w3.org/2000/svg"
					width="24"
					height="24"
					viewBox="0 0 24 24"
					class="bg-yellow-400 rounded-sm p-1"
				>
					<path
						d="M24 4.557c-.883.392-1.832.656-2.828.775 1.017-.609 1.798-1.574 2.165-2.724-.951.564-2.005.974-3.127 1.195-.897-.957-2.178-1.555-3.594-1.555-3.179 0-5.515 2.966-4.797 6.045-4.091-.205-7.719-2.165-10.148-5.144-1.29 2.213-.669 5.108 1.523 6.574-.806-.026-1.566-.247-2.229-.616-.054 2.281 1.581 4.415 3.949 4.89-.693.188-1.452.232-2.224.084.626 1.956 2.444 3.379 4.6 3.419-2.07 1.623-4.678 2.348-7.29 2.04 2.179 1.397 4.768 2.212 7.548 2.212 9.142 0 14.307-7.721 13.995-14.646.962-.695 1.797-1.562 2.457-2.549z"
					></path>
				</svg>
			</a>
			<a href="/">
				<svg
					xmlns="http://www.w3.org/2000/svg"
					width="24"
					height="24"
					viewBox="0 0 24 24"
					class="bg-teal-400 rounded-sm p-1"
				>
					<path
						d="M19.615 3.184c-3.604-.246-11.631-.245-15.23 0-3.897.266-4.356 2.62-4.385 8.816.029 6.185.484 8.549 4.385 8.816 3.6.245 11.626.246 15.23 0 3.897-.266 4.356-2.62 4.385-8.816-.029-6.185-.484-8.549-4.385-8.816zm-10.615 12.816v-8l8 3.993-8 4.007z"
					></path>
				</svg>
			</a>
			<a href="/">
				<svg
					xmlns="http://www.w3.org/2000/svg"
					width="24"
					height="24"
					viewBox="0 0 24 24"
					class="bg-indigo-400 rounded-sm p-1"
				>
					<path
						d="M9 8h-3v4h3v12h5v-12h3.642l.358-4h-4v-1.667c0-.955.192-1.333 1.115-1.333h2.885v-5h-3.808c-3.596 0-5.192 1.583-5.192 4.615v3.385z"
					></path>
				</svg>
			</a>
		</div>
	</nav>
</footer>

<style>
	* {
		max-width: 1440px;
		overflow: hidden;
	}

	a {
		font-family: 'Hammersmith One', sans-serif;
		font-size: 13px;
		line-height: 24px;
		color: #808080;
	}

	button {
		border-radius: 10px 0 10px 0;
	}
</style>
