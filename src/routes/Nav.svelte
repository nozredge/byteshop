<script lang="ts">
    import { HeartIcon, SearchIcon, ShoppingCartIcon } from 'svelte-feather-icons'
    import Logo from './Logo.svelte'
    import "@fontsource/montserrat";
    import { store } from './stores';
    
    let cart_total: number;
    
    store.subscribe((value) => 
    {
        cart_total = value;
    });
</script>

<nav>
    <div class="container">
        <div class="logo-container">
                <Logo />
        </div>

        <div class="links-container">
            <a href="#">Home</a>
            <a href="#">Páginas</a>
            <a href="#">Blog</a>
            <a href="#">Contacto</a>
        </div>

        <div class="search-cart-container">
            <div class="search-icon">
                <SearchIcon size=30 />
            </div>

            <div class="heart-icon">
                <HeartIcon size=30 />
            </div>

            <div class="cart-icon">
                <ShoppingCartIcon size="30" />
            </div>
            <div class="total-price">{cart_total}</div>
        </div>
    </div>
</nav>

<nav class="underline"></nav>

<style>
    
    .logo-container {
        width: 20vw;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .container {
        display: flex;
        width: 100vw;
        height: 10vh;
    }

    .underline {
        background-color: #718093;
        height: 1vh;
    }

    .search-cart-container {
        width: 20vw;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .cart-icon {
        margin-left: 2em;
        color: #1e1e24;
    }

    .heart-icon {
        margin-left: 2em;
        color: #1e1e24;
    }

    .search-icon {
        color: #1e1e24
    }

    .total-price {
        font-size: 1em;
        margin-left: 1em;
    }

    .links-container {
        display: flex;
        justify-content: space-evenly;
        align-items: center;
        width: 60vw;
    }

    a {
        text-decoration: none;
        font-size: 1.4em;
        color: #1e1e24;
    }

    a:hover{
        color: #7a7877;
        /*font-size: 1.3em;*/
        text-decoration-thickness: 0.1em;
        text-decoration-style: solid;
        text-decoration-line: underline;
    }

    * {
        font-family: "Montserrat";
    }

    

</style>