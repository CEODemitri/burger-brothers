<script>
    import "../app.css";
    
  </script>
  
  <header class="px-4 lg:px-6 h-14 flex items-center">
    <a class="flex items-center justify-center" href="/" rel="ugc">
        <figure>
            <img src="../logo.png" alt="" class="w-14">
            <figcaption>
                <h1 class="text-2xl font-bold text-gray-900 sr-only">UGC</h1>
            </figcaption>
        </figure>
        <span class="sr-only">Burger Brothers</span>
    </a>
    <nav class="ml-auto flex gap-4 sm:gap-6 text-neutral-700">
        <a class="text-sm font-medium hover:underline underline-offset-4 hover:scale-105 hover:font-extrabold" href="/Menu" rel="ugc">
            Menu
        </a>
        <a class="text-sm font-medium hover:underline underline-offset-4 hover:scale-105 hover:font-extrabold" href="/Locations" rel="ugc">
            Locations
        </a>
        <a class="text-sm font-medium hover:underline underline-offset-4 hover:scale-105 hover:font-extrabold" href="#" rel="ugc">
            About Us
        </a>
        <a class="text-sm font-medium hover:underline underline-offset-4 hover:scale-105 hover:font-extrabold" href="#" rel="ugc">
            Contact
        </a>
        <a href="#">
            <span class="material-icons">
                receipt_long
            </span>
        </a>
    </nav>
</header>
<slot />

<footer class="flex flex-col gap-2 sm:flex-row py-6 w-full shrink-0 items-center px-4 md:px-6 border-t bg-black text-white">
    <div class="flex items-center gap-2">
        <a class="flex items-center gap-2 text-sm hover:underline underline-offset-4" href="#" rel="ugc">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4">
                <path d="M22 4s-.7 2.1-2 3.4c1.6 10-9.4 17.3-18 11.6 2.2.1 4.4-.6 6-2C3 15.5.5 9.6 3 5c2.2 2.6 5.6 4.1 9 4-.9-4.2 4-6.6 7-3.8 1.1 0 3-1.2 3-1.2z"></path>
            </svg>
            Twitter
        </a>
        <a class="flex items-center gap-2 text-sm hover:underline underline-offset-4" href="#" rel="ugc">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4">
                <rect width="20" height="20" x="2" y="2" rx="5" ry="5"></rect><path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"></path><line x1="17.5" x2="17.51" y1="6.5" y2="6.5"></line>
            </svg>
            Instagram
        </a>
        <a class="flex items-center gap-2 text-sm hover:underline underline-offset-4" href="#" rel="ugc">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4">
                <path d="M18 2h-3a5 5 0 0 0-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 0 1 1-1h3z"></path>
            </svg>
            Facebook
        </a> 
    </div>
    <nav class="sm:ml-auto flex gap-4 sm:gap-6">
        <a class="text-xs hover:underline underline-offset-4" href="#" rel="ugc">
            Terms of Service
        </a>
        <a class="text-xs hover:underline underline-offset-4" href="#" rel="ugc">
            Privacy
        </a>
    </nav>
</footer>

<style>
    a {
        font-family: 'Comfortaa Variable', sans-serif;
        font-size: 13px;
        line-height: 24px;
    }
</style>
