<script>
    import { slide } from 'svelte/transition'
    import { quintOut } from 'svelte/easing';
</script>


<h1 class="text-3xl font-semibold" transition:slide={{ delay: 250, duration: 300 }}>About Burger Brothers</h1>
<p>Long Lasting, strong Will.</p>

<article>
    <section class="h-48 bg-red-500 glass">
        Hard works pays off.
    </section>
    <p>Burger Brothers was founded in 2014.</p>

    <!-- visit us -->
    <section></section>

    <!-- contact us -->
    <section></section>

    <!-- work with us -->
    <section></section>

    <!-- farmer community -->
    <section></section>
</article>