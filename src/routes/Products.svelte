<script>
    import Product from "./Product.svelte";
</script>

<div>
    <Product name="camisa_casual"/>
    <Product name="libro" color="#F6F9FF"/>
    <Product name="set_cuchillos" color="#Fafff5"/>
    <Product name="pods"  color="#Fafff5"/>
    <Product name="telefono2" color="#F6F9FF"/>
    <Product name="zapatos"/>
</div>

<style>
    div {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        grid-template-rows: 1fr 1fr;
        gap: 3em;
    }    
</style>