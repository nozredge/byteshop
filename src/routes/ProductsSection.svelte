<script>
    import ProductsTitle from "./ProductsTitle.svelte";
    import Products from "./Products.svelte";
</script>

<div class="products-section-container">
    <ProductsTitle />
    <Products />
</div>

<style>
    .products-section-container {
        width: 70vw;
        height: 150vh;
        display: grid;
        grid-template-rows: 1fr 6fr;
    }
</style>