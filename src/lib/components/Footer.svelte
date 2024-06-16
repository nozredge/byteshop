<footer>
    <div class="footer-container">
        <div class="contact-details">
            <div>
                <h3 class="contact-title">
                    TIENDA
                </h3>
            </div>
            <div>Contáctanos</div>
            <div>Métodos de pago</div>
            <div>Formas de envío a todo Chile</div>
        </div>

        <div class="copyright">
            <h2>
                Shop Bytechile - Copyright © 2024 Todos los derechos reservados
            </h2>
        </div>
    </div>
</footer>

<style>
    footer {
        width: 100vw;
        height: 30vh;
        background-color: #6c757d;
        display: flex;
        justify-content: center;
    }

    .footer-container {
        width: 40vw;
        display: grid;
        grid-template-rows: 3fr 2fr;
    }

    .contact-details {
        display: flex;
        flex-wrap: wrap;
        align-content: space-evenly;
    }

    .contact-details > div {
        width: 100%;
        display: flex;
        justify-content: start;
    }

    .contact-title {
        margin-bottom: 2em;
    }

    .copyright {
        display: flex;
        align-items: center;
    }
</style>