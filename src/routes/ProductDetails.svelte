<script lang="ts">
    import "@fontsource/montserrat";
    import { store } from "./stores";

    function add_item_to_cart() 
    {
        store.update((value) => value + 1);
    }
</script>

<div class="details">
    <p>Producto</p>
    <button on:click={add_item_to_cart}>+ Agregar al carrito</button>
    <p>$23.990</p>
</div>

<style>

    button {
        all:unset; 
        border: 0.2rem solid #ccd1d1;
        border-radius: 1.2rem;
        cursor: pointer;
        color: #2c3e4f;
        padding: 0.4rem;
        text-align: center;
    }

    div {
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: 5vh 5vh;
        align-items: end;
        width: 100%;
    }

    * {
        font-family: "Montserrat";
        color: #555;
    }

    div :nth-child(3) {
        font-size: 1.4rem;
    }
</style>