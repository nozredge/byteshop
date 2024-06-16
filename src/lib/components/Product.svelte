<script>
    const full_product_name_path = '/src/lib/assets/img/';
    const extension = '.png';
    export let name;
    export let width;
    export let height;
    export let align_self = 'auto';
    export let color = "#e9ecee";
</script>

<div class="product-container"
    style="background-color: {color};">
    <div class="product" 
        style="
            background-image: url('/src/lib/assets/img/{name}{extension}');
            width: {width};
            height: {height};
            align-self: {align_self}
            ">
    </div>
</div>

<style>

    .product-container {
        width: auto;
        height: 50vh;
        display: grid;
        grid-template-rows: 5fr 3fr;
        justify-items: center;
    }

    .product {
        /*background-size: 3em; */
        background-size: contain;
        background-repeat: no-repeat;
        align-self: auto;
    }
</style>