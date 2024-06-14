<script>
    import { HeartIcon, SearchIcon, ShoppingCartIcon } from 'svelte-feather-icons'
    import Logo from '$lib/components/Logo.svelte'
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
            <div class="total-price">$24.900</div>
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
        background-color: #f4f4f8;
    }

    .underline {
        background-color: #6c757d;
        height: 0.5em;
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
        height: 15vh;
        width: 60vw;
    }

    a {
        text-decoration: none;
        font-size: 1.2em;
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
        font-family: "M PLUS Rounded 1c", sans-serif;
    }

    

</style>