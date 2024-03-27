<script>
    import '@fontsource-variable/comfortaa';
    import '@fontsource/fugaz-one';    

    export let src;
    export let price;
    export let name;
    export let description;
</script>

<div class="flex flex-col space-y-2 p-2 text-left">
    <img {src} width="400" height="400" alt="Burger" class="aspect-square overflow-hidden rounded-xl object-cover object-center">
    <div class="space-y-2">
        <p class="text-sm text-gray-500 dark:text-gray-400">{price}</p>
        <h3 class="text-xl font-bold">{name}</h3>
        <p class="w-72">{description}</p>
        
        <form action="" class="flex justify-center gap-7">
            <input type="number" class="w-8 bg-black text-white rounded-xl" min="0">
            <button class="bg-black text-white px-5 py-2 rounded-md">Add To Cart</button>
        </form>
    </div>
</div>

<style>
    h3 {
        font-family: 'Fugaz One', cursive;
        font-size: 2em;
    }

    button {
            font-family: 'Fugaz One', cursive;
        }

    p {
        font-family: 'Comfortaa Variable', cursive;
        font-size: 0.8em;
        color: grey;
    }
</style>