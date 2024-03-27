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
        <a class="text-sm font-medium hover:underline underline-offset-4 hover:scale-105" href="/Menu" rel="ugc">
            Menu
        </a>
        <a class="text-sm font-medium hover:underline underline-offset-4 hover:scale-105" href="/Locations" rel="ugc">
            Locations
        </a>
        <a class="text-sm font-medium hover:underline underline-offset-4 hover:scale-105" href="#" rel="ugc">
            About Us
        </a>
        <a class="text-sm font-medium hover:underline underline-offset-4 hover:scale-105" href="#" rel="ugc">
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