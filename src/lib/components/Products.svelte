<script>
    import Product from "./Product.svelte";
</script>

<div>
    <Product name="camisa_casual" width = "40%" height="90%" align_self="center"/>
    <Product name="telefono1" width="50%" height="80%" align_self="center"/>
    <Product name="set_cuchillos" width="50%" height="80%" align_self="center"/>
    <Product name="pods" width="50%" height="80%" align_self="center"/>
    <Product name="telefono2" width="50%" height="80%" align_self="center"/>
</div>

<style>
    div {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        grid-template-rows: 1fr 1fr;
        gap: 3em;
    }    
</style>