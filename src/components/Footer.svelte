<style>
    footer.Footer {
        margin-top: 10em;
        color: #F3F3F3;
        background-color: #49484D;
        position: relative;
        bottom: 0;
        left: 0;
        right: 0;
        padding: 1em;
        display: grid;
        grid-template-columns: repeat(4, 1fr);
    }
    div.Footer-content {
        font-family: 'Roboto', sans-serif;
        grid-column: 1 / 5;
        display: inherit;
        grid-template-columns: repeat(2, 1fr);
    }
    div.Footer-content div {
        display: inline-block;
        text-align: center;
        padding: 0.5em 1em;
    }
    div.Footer-content div.copyright {
        text-align: center;
        display: block;
        grid-column: 1 / 3;
    }
    a {
        color: inherit;
    }
</style>

<footer class="Footer">
    <div class="Footer-content">
        <div>
            <a href="sitemap">Ver sitemap</a>
        </div>
        <div>
            <a href="politicas">Políticas de Privacidad</a>
        </div>
        <div class="copyright">
            © Accesa Group 2020
        </div>
    </div>
</footer>