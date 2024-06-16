<script>
    import Nav from "./Nav.svelte"
    import Body from "./Body.svelte"
    import Footer from "./Footer.svelte";
</script>

<Nav />
<Body />
<Footer />

<style>
    /* http://meyerweb.com/eric/tools/css/reset/ 
   v2.0 | 20110126
   License: none (public domain)
    */
    :global(Nav, Body, Footer){
        margin: 0;
        padding: 0;
        border: 0;
        font-size: 100%;
        font: inherit;
        vertical-align: baseline;
    }
</style>
