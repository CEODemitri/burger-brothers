<script>
	import '../app.css';
	import '@fontsource-variable/comfortaa';
	import '@fontsource/fugaz-one';
	import '@fontsource/prosto-one';
</script>

<header class="px-4 lg:px-6 h-14 flex items-center bg-light text-dark">
	<a class="flex items-center justify-center" href="/" rel="ugc">
		<figure>
			<img src="../logo.png" alt="" class="w-14" />
			<figcaption>
				<h1 class="text-2xl font-bold text-gray-900 sr-only">Burger Brothers Logo</h1>
			</figcaption>
		</figure>
		<span class="sr-only">Burger Brothers</span>
	</a>
	<nav class="ml-auto flex gap-4 sm:gap-6 text-dark">
		<a
			class="text-sm font-medium hover:underline underline-offset-4 hover:scale-105 hover:font-extrabold"
			href="/Menu"
			rel="ugc"
		>
			Menu
		</a>
		<a
			class="text-sm font-medium hover:underline underline-offset-4 hover:scale-105 hover:font-extrabold"
			href="/Locations"
			rel="ugc"
		>
			About
		</a>
		<a
			class="text-sm font-medium hover:underline underline-offset-4 hover:scale-105 hover:font-extrabold"
			href="/Events"
			rel="ugc"
		>
			FAQ
		</a>
		<a
			class="text-sm font-medium hover:underline underline-offset-4 hover:scale-105 hover:font-extrabold"
			href="/Shop"
			rel="ugc"
		>
			Shop
		</a>
		<a href="#">
			<span class="material-icons"> receipt_long </span>
		</a>

		<label class="cursor-pointer grid place-items-center">
			<input type="checkbox" value="synthwave" class="toggle theme-controller bg-base-content row-start-1 col-start-1 col-span-2"/>
			<svg class="col-start-1 row-start-1 stroke-base-100 fill-base-100" xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="5"/><path d="M12 1v2M12 21v2M4.2 4.2l1.4 1.4M18.4 18.4l1.4 1.4M1 12h2M21 12h2M4.2 19.8l1.4-1.4M18.4 5.6l1.4-1.4"/></svg>
			<svg class="col-start-2 row-start-1 stroke-base-100 fill-base-100" xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"></path></svg>
		  </label>
	</nav>
</header>
<slot />

<footer
	class="flex flex-col gap-2 sm:flex-row py-6 w-full shrink-0 items-center px-4 md:px-6 border-t bg-dark text-white"
>
	<div class="flex items-center gap-2">
		<a
			class="flex items-center gap-2 text-sm hover:underline underline-offset-4"
			href="#"
			rel="ugc"
		>
			<svg
				xmlns="http://www.w3.org/2000/svg"
				width="24"
				height="24"
				viewBox="0 0 24 24"
				fill="none"
				stroke="currentColor"
				stroke-width="2"
				stroke-linecap="round"
				stroke-linejoin="round"
				class="w-4 h-4"
			>
				<path
					d="M22 4s-.7 2.1-2 3.4c1.6 10-9.4 17.3-18 11.6 2.2.1 4.4-.6 6-2C3 15.5.5 9.6 3 5c2.2 2.6 5.6 4.1 9 4-.9-4.2 4-6.6 7-3.8 1.1 0 3-1.2 3-1.2z"
				></path>
			</svg>
			Twitter
		</a>
		<a
			class="flex items-center gap-2 text-sm hover:underline underline-offset-4"
			href="#"
			rel="ugc"
		>
			<svg
				xmlns="http://www.w3.org/2000/svg"
				width="24"
				height="24"
				viewBox="0 0 24 24"
				fill="none"
				stroke="currentColor"
				stroke-width="2"
				stroke-linecap="round"
				stroke-linejoin="round"
				class="w-4 h-4"
			>
				<rect width="20" height="20" x="2" y="2" rx="5" ry="5"></rect><path
					d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"
				></path><line x1="17.5" x2="17.51" y1="6.5" y2="6.5"></line>
			</svg>
			Instagram
		</a>
		<a
			class="flex items-center gap-2 text-sm hover:underline underline-offset-4"
			href="#"
			rel="ugc"
		>
			<svg
				xmlns="http://www.w3.org/2000/svg"
				width="24"
				height="24"
				viewBox="0 0 24 24"
				fill="none"
				stroke="currentColor"
				stroke-width="2"
				stroke-linecap="round"
				stroke-linejoin="round"
				class="w-4 h-4"
			>
				<path d="M18 2h-3a5 5 0 0 0-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 0 1 1-1h3z"></path>
			</svg>
			Facebook
		</a>
	</div>
	<nav class="sm:ml-auto flex gap-4 sm:gap-6">
		<a class="text-xs hover:underline underline-offset-4" href="#" rel="ugc"> Terms of Service </a>
		<a class="text-xs hover:underline underline-offset-4" href="#" rel="ugc"> Privacy </a>
	</nav>
</footer>

<style>
	a {
		font-family: 'Comfortaa Variable', sans-serif;
		font-size: 13px;
		line-height: 24px;
	}
</style>
