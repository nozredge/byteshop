<script>
    const full_product_name_path = '/src/lib/assets/img/';
    const extension = '.png';
    export let product_name;
</script>

<div>
    <div class="product" 
        style="background-image: url('/src/lib/assets/img/{product_name}{extension}');"></div>
</div>

<style>

    .product {
        /*background-size: 3em; */
        height: 40vh;
        width: 20vw;
        background-size: contain;
    }
</style>