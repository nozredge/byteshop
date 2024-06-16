<script>
    import Product from "./Product.svelte";
</script>

<div>
    <Product name="camisa_casual" width = "70%" height="auto"/>
    <Product name="novela" width="70%" height="auto"/>
    <Product name="set_cuchillos" width="100%" height="100%"/>
    <Product name="bicicleta" width="80%" height="50%"/>
</div>

<style>
    div {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        grid-template-rows: 1fr 2fr;
        row-gap: 5em;
    }    
</style>