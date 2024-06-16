<script>
    import pods from '$lib/assets/img/pods.png';
    import camisa_casual from '$lib/assets/img/camisa_casual.png';
    import set_cuchillos from '$lib/assets/img/set_cuchillos.png';
    import libro from '$lib/assets/img/libro.png';
    import telefono2 from '$lib/assets/img/telefono2.png';
    import zapatos from '$lib/assets/img/zapatos.png';

    export let name;
    export let color = "#F9F9F9";
</script>

<div class="product-container">
    <div class="product-image-container" style="background-color: {color};">
        <div class="product-image">
            {#if name === 'pods'}
                <img
                    loading="lazy" 
                    src={pods} 
                    alt="A product"
                >
            {:else if name === 'camisa_casual'}
                <img
                    loading="lazy" 
                    src={camisa_casual} 
                    alt="A product"
                >
            {:else if name === 'set_cuchillos'}
                <img
                    loading="lazy" 
                    src={set_cuchillos} 
                    alt="A product"
                >
            {:else if name === 'libro'}
                <img
                    loading="lazy" 
                    src={libro} 
                    alt="A product"
                >
            {:else if name === 'telefono2'}
                <img
                    loading="lazy" 
                    src={telefono2} 
                    alt="A product"
                >
            {:else if name === 'zapatos'}
                <img
                    loading="lazy" 
                    src={zapatos} 
                    alt="A product"
                >
            {/if}
        </div>
    </div>
</div>

<style>

    .product-container {
        display: grid;
        grid-template-rows: 5fr 2fr;
        justify-items: center;
        align-items: center;
    }

    .product-image-container {
        width: 100%;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .product-image {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 70%;
        width: 70%;
    }

    img {
        width: 100%;
        height: 100%;
    }
</style>