<script>
  import MediumCards from "../components/Cards/MediumCards.svelte";
</script>

<main class="flex-1 w-full">
    <section class="w-full py-12 lg:py-24">
      <div class="container grid items-center justify-center gap-4 px-4 text-center md:gap-10">
        <div class="space-y-4 lg:space-y-6">
          <h1 class="text-4xl font-bold tracking-tighter sm:text-5xl md:text-6xl">Menu</h1>
          <p class="mx-auto max-w-[600px] text-gray-500 md:text-xl/relaxed lg:text-base/relaxed xl:text-xl/relaxed dark:text-gray-400">
            Handcrafted with love. Enjoy our delicious burgers. Starters, desserts, drinks, our menu has something for the whole table.
          </p>
        </div>
      </div>
    </section>

    <!-- starters -->
    <div class="rounded-lg border bg-card text-card-foreground shadow-sm bg-neutral-300" data-v0-t="card">
        <div class="p-6 flex flex-row space-y-0 items-start gap-2">
          <div class="grid gap-1">
            <h3 class="text-3xl font-semibold whitespace-nowrap leading-none tracking-tight">Starters</h3>
            <p class="text-sm text-muted-foreground">Delicious appetizers to kick off your meal.</p>
          </div>
        </div>
        <div class="p-6">
          <div class="container grid items-start gap-6 px-4 md:grid-cols-2 md:gap-10 lg:grid-cols-3">
            <MediumCards />
            <MediumCards />
            <MediumCards />
            <MediumCards />

          </div>
        </div>
      </div>

      <!-- desserts -->
      <div class="rounded-lg border bg-card text-card-foreground shadow-sm" data-v0-t="card">
        <div class="p-6 flex flex-row space-y-0 items-start gap-2">
          <div class="grid gap-1">
            <h3 class="text-3xl font-semibold whitespace-nowrap leading-none tracking-tight">Desserts</h3>
            <p class="text-sm text-muted-foreground">Delicious desserts to end your perfect meal.</p>
          </div>
        </div>
        <div class="p-6">
          <div class="container grid items-start gap-6 px-4 md:grid-cols-2 md:gap-10 lg:grid-cols-3">
            <MediumCards />
            <MediumCards />
            <MediumCards />
            <MediumCards />
          </div>
        </div>
      </div>

      <!-- add the carousel mover and logic -->
      <!-- change the p,button font to more systemmatic code -->
      <!-- components -->
      <!-- fix layout + add footer -->
      
      <!-- drinks -->
      <div class="rounded-lg border bg-card text-card-foreground shadow-sm bg-neutral-300" data-v0-t="card">
        <div class="p-6 flex flex-row space-y-0 items-start gap-2">
          <div class="grid gap-1">
            <h3 class="text-3xl font-semibold whitespace-nowrap leading-none tracking-tight">Drinks</h3>
            <p class="text-sm text-muted-foreground">Wash it down with a classic lift.</p>
          </div>
        </div>
        <div class="p-6">
          <div class="container grid items-start gap-6 px-4 md:grid-cols-2 md:gap-10 lg:grid-cols-3">
            <div class="carousel rounded-box w-96">
              <div class="carousel-item w-1/2">
                <img src="https://daisyui.com/images/stock/photo-1559703248-dcaaec9fab78.jpg" class="w-full" />
              </div> 
              <div class="carousel-item w-1/2">
                <img src="https://daisyui.com/images/stock/photo-1565098772267-60af42b81ef2.jpg" class="w-full" />
              </div> 
              <div class="carousel-item w-1/2">
                <img src="https://daisyui.com/images/stock/photo-1572635148818-ef6fd45eb394.jpg" class="w-full" />
              </div> 
              <div class="carousel-item w-1/2">
                <img src="https://daisyui.com/images/stock/photo-1494253109108-2e30c049369b.jpg" class="w-full" />
              </div> 
              <div class="carousel-item w-1/2">
                <img src="https://daisyui.com/images/stock/photo-1550258987-190a2d41a8ba.jpg" class="w-full" />
              </div> 
              <div class="carousel-item w-1/2">
                <img src="https://daisyui.com/images/stock/photo-1559181567-c3190ca9959b.jpg" class="w-full" />
              </div> 
              <div class="carousel-item w-1/2">
                <img src="https://daisyui.com/images/stock/photo-1601004890684-d8cbf643f5f2.jpg" class="w-full" />
              </div>
            </div>
          </div>
        </div>
      </div>
</main>

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