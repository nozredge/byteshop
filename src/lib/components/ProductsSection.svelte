<script>
    import ProductsTitle from "./ProductsTitle.svelte";
    import Product from "./Product.svelte";
</script>

<div class="products-section-container">
    <ProductsTitle />
</div>

<style>
    .products-section-container {
        width: 70vw;
        height: 89vh;
        display: grid;
        grid-template-rows: 1fr 6fr;
    }
</style>