<script>
    import Navbar from "./Navbar.svelte";
    import Hero from "./Hero.svelte";
    import Footer from "./footer.svelte";
</script>

<Hero />
<Navbar />

<slot />
<Footer />

