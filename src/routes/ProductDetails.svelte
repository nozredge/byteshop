<script>
    import "@fontsource/montserrat";
</script>

<div class="details">
    <p>Producto</p>
    <p>+ Agregar al carrito</p>
    <p>$23.990</p>
</div>

<style>
    div {
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: 5vh 7vh;
        width: 100%;
    }

    p {
        font-family: "Montserrat";
        color: #343a40;
    }

    div :nth-child(3) {
        font-size: 1.5rem;
    }

    div :nth-child(2) {
        color:#e84855;
    }

    div :nth-child(2):hover {
        cursor: pointer;
        font-size: 1.1rem;
        color:#e84815;
    }
</style>