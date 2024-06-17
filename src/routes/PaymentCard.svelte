<script>
    import "@fontsource/montserrat";
    import { XSquareIcon } from "svelte-feather-icons";
</script>

<div class="payment-card">
    <div class="x-icon"><XSquareIcon size="30"/></div>
    <div class="total-label">Total:</div>
    <div class="total">$179000</div>
    <button class="buy-btn">Pagar</button>
</div>


<style>

    * {
        font-family: "Montserrat";
        color: #343E49;
    }
    .payment-card {
        padding: 1.2rem;
        background-color: #f6f9f9;
        position: absolute;
        width: 26vw;
        height: 25vh;
        padding-top: 2rem;
        padding-left: 2rem;
        padding-right: 2rem;
        left: 40vw;
        top: 20vh;
        z-index: 1;
        opacity: 0;
        display: grid;
        grid-template-columns: 3fr 1fr;
        grid-template-rows: 4fr 5fr 2fr;
        box-shadow: #5d6d7d 0.5rem 0.5rem 15px;
    }

    .buy-btn {
        grid-column: 1/3;
        grid-row: 3;
        border-radius: 1.5rem;
        margin-bottom: 2rem;
        cursor: pointer;
        border-style: solid;
        background-color: #78bbf7;
        border-color: #78bbf7;
        font-size: 1.5rem;
        height: 3.2rem;
        width: 25rem;
        justify-self: center;
        color: #f6f9f9;
        font-weight: bold;
    }

    .buy-btn:hover {
        background-color: #75b6f3;
        border-color: #75b6f3;
    }

    .total-label {
        font-size: 1.8rem;
        grid-row: 2;
    }
    
    .total {
        font-size: 1.8rem;
        grid-row: 2;
    }

    .x-icon {
        grid-column: 2;
        justify-self: self-end;
        color: #343E49;
        margin-bottom: 3rem;
    }
    
</style>