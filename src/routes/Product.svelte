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
    <div class="product-image-container" >
        <div class="product-image" style="background-color: {color};">
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

    img {
        margin-top: 1rem;
        width: 100%;
        height: 100%;
    }
</style>