<script>
	import '../app.css';
	import '@fontsource/hammersmith-one';
	import '@fontsource/finger-paint';
</script>

<div class="navbar bg-[#000]">
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
				<img src="../logo.png" alt="" class="w-14" />
				<figcaption>
					<h1 class="text-2xl font-bold text-gray-900 sr-only">Burger Brothers Logo</h1>
				</figcaption>
			</figure>
			<span class="sr-only">Burger Brothers</span>
		</a>
	</div>
	<div class="navbar-end">
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
		<button class="btn btn-ghost btn-circle">
			<div class="indicator">
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
						d="M15 17h5l-1.405-1.405A2.032 2.032 0 0118 14.158V11a6.002 6.002 0 00-4-5.659V5a2 2 0 10-4 0v.341C7.67 6.165 6 8.388 6 11v3.159c0 .538-.214 1.055-.595 1.436L4 17h5m6 0v1a3 3 0 11-6 0v-1m6 0H9"
					/>
				</svg>
				<span class="badge badge-xs badge-primary indicator-item"></span>
			</div>
		</button>
		<button class="bg-action text-xs md:text-sm px-5 py-2 ff-serif">Order Online</button>
	</div>
</div>
<slot />

<footer
	class="flex flex-col gap-2 sm:flex-row py-6 w-full shrink-0 items-center px-4 md:px-6 border-t bg-dark text-white m-auto"
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
