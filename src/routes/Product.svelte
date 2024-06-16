<script>
    import pods from '$lib/assets/img/pods.png';
    import camisa_casual from '$lib/assets/img/camisa_casual.png';
    import set_cuchillos from '$lib/assets/img/set_cuchillos.png';
    import telefono1 from '$lib/assets/img/telefono1.png';
    import telefono2 from '$lib/assets/img/telefono2.png';
    import zapatos from '$lib/assets/img/zapatos.png';


    const extension = '.png';
    export let name;
    export let width;
    export let height;
    export let align_self = 'auto';
    export let color = "#F9F9F9";
</script>

<div class="product-container"
    style="background-color: {color};">
    <!-- <div class="product" 
        style="
            background-image: url('/src/lib/assets/img/{name}{extension}');
            width: {width};
            height: {height};
            align-self: {align_self}
            ">
    </div> -->
    {#if name === 'pods'}
        <img
            loading="lazy" 
            src={pods} 
            alt="A product"
            style="
                width: {width};
                height: {height};
                align-self: {align_self}
            "
        >
    {:else if name === 'camisa_casual'}
        <img
            loading="lazy" 
            src={camisa_casual} 
            alt="A product"
            style="
                width: {width};
                height: {height};
                align-self: {align_self}
            "
        >
    {:else if name === 'set_cuchillos'}
    <img
        loading="lazy" 
        src={set_cuchillos} 
        alt="A product"
        style="
            width: {width};
            height: {height};
            align-self: {align_self}
        "
    >
    {:else if name === 'telefono1'}
        <img
            loading="lazy" 
            src={telefono1} 
            alt="A product"
            style="
                width: {width};
                height: {height};
                align-self: {align_self}
            "
        >
    {:else if name === 'telefono2'}
    <img
        loading="lazy" 
        src={telefono2} 
        alt="A product"
        style="
            width: {width};
            height: {height};
            align-self: {align_self}
        "
    >
    {:else if name === 'zapatos'}
        <img
            loading="lazy" 
            src={zapatos} 
            alt="A product"
            style="
                width: {width};
                height: {height};
                align-self: {align_self}
            "
        >
    {/if}
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
        margin-top: 3em;
        background-size: contain;
        background-repeat: no-repeat;
        align-self: auto;
    }
</style>