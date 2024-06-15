<script>
    const full_product_name_path = '/src/lib/assets/img/';
    const extension = '.png';
    export let name;
</script>

<div>
    <div class="product" 
        style="background-image: url('/src/lib/assets/img/{name}{extension}');"></div>
</div>

<style>

    .product {
        /*background-size: 3em; */
        height: 40vh;
        width: 20vw;
        background-size: contain;
    }
</style>