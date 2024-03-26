<script>
    // Supports weights 300-700
    import '@fontsource-variable/comfortaa';
    import '@fontsource/fugaz-one';    
</script>

<!--
// v0 by Vercel.
// https://v0.dev/t/NTp0OzPUCg9
-->
<div class="flex flex-col min-h-[100dvh]">
    <div class="banner h-10 bg-black text-center text-white py-2">
        <p>Homepage Banner: Important Text Here</p>
    </div>
    
    <main class="flex-1">
        <section class="w-full py-12 md:py-18 lg:py-24">
            <div class="container flex flex-col items-center justify-center space-y-4 px-4 md:px-6">
                <div class="space-y-2 text-center">
                    <h1 class="text-3xl font-bold tracking-tighter sm:text-4xl md:text-5xl lg:text-6xl/none">
                        Burger Brothers
                    </h1>
                    <p class="mx-auto max-w-[100ch] text-gray-500 md:text-xl/relaxed lg:text-base/relaxed xl:text-xl/relaxed dark:text-gray-400 font">
                        Premium and fresh ingredients all day loaded into your favorite buns. Gourmet flavors dripping. The perfect burger. YOUR perfect burger, Made your way.
                    </p>
                </div>
                <img src="/landing/heroBurger-grilled_chz.png" width="600" height="400" alt="Hero" class="mx-auto aspect-video overflow-hidden rounded-xl object-cover object-center lg:w-[75%]">
                <section>
                    <button class="text-white bg-black p-2 rounded-md special hover:scale-125 hover:mx-4">Order Online</button>
                    <a href="/Menu" class="underline p-2 rounded-md special">Full Menu</a>
                </section>
            </div>
        </section>
        <section class="w-full py-12 md:py-24 lg:py-32 border-t">
            <div class="container grid items-center justify-center gap-4 px-4 text-center md:px-6">
                <span class="pill bg-black text-white w-fit m-auto px-3 rounded-xl ">Burgertastic</span>
                <div class="space-y-3">
                    <h2 class="text-3xl font-bold tracking-tighter sm:text-4xl md:text-5xl">
                        Seasonal Menu
                    </h2>
                    <p class="mx-auto max-w-[600px] text-gray-500 md:text-xl/relaxed lg:text-base/relaxed xl:text-xl/relaxed dark:text-gray-400">
                        Limited timing creations. We in parallel with nature; many of our beautiful creations are seasonal, not to be abused or imitated.
                    </p>
                </div>
                <div class="mx-auto grid max-w-5xl items-start gap-6 sm:grid-cols-2 md:gap-12 lg:max-w-none lg:grid-cols-3">
                    <div class="flex flex-col items-center space-y-2">
                        <img src="/placeholder.svg" width="400" height="400" alt="Burger" class="aspect-square overflow-hidden rounded-xl object-cover object-center">
                        <div class="space-y-2 text-center">
                            <h3 class="text-xl font-bold">Classic Burger</h3>
                            <p class="text-sm text-gray-500 dark:text-gray-400">$50.99</p>
                        </div>
                    </div>
                    <div class="flex flex-col items-center space-y-2">
                        <img src="/placeholder.svg" width="400" height="400" alt="Burger" class="aspect-square overflow-hidden rounded-xl object-cover object-center">
                        <div class="space-y-2 text-center">
                            <h3 class="text-xl font-bold">Cheeseburger</h3>
                            <p class="text-sm text-gray-500 dark:text-gray-400">$60.99</p>
                        </div>
                    </div>
                    <div class="flex flex-col items-center space-y-2">
                        <img src="/placeholder.svg" width="400" height="400" alt="Burger" class="aspect-square overflow-hidden rounded-xl object-cover object-center">
                        <div class="space-y-2 text-center">
                            <h3 class="text-xl font-bold">Bacon Burger</h3>
                            <p class="text-sm text-gray-500 dark:text-gray-400">$70.99</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>
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
</div>

<style>
    h1, h2, h3, .special {
        font-family: 'Fugaz One', system-ui;
    }

    p, button {
        font-family: 'Comfortaa Variable', sans-serif;
        font-size: 16px;
        line-height: 24px;
    }
</style>