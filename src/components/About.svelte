<script>
    import Title from './Title.svelte';
</script>

<style>
    section.About {
        grid-column: 1 / 5;
        margin-top: 6em;
    }
    div.About-content {
        font-family: 'Roboto', sans-serif;

        color: #49484D;
    }
    div.About-content p {
        font-family: inherit;
        font-weight: 300;
        font-size: 1.5em;
        text-align: justify;
        line-height: 135%;
    }
    div.About-content p:nth-child(2) {
        display: none;
    }
    div.About-image {
        display: none;
    }
    @media (min-width: 840px) {
        section.About {
            grid-column: 1 / 13;
            display: inherit;
            grid-template-columns: inherit;
            column-gap: inherit;
        }
        div.About-content {
            grid-column: 1 / 7;
            margin-top: 1.5em;
        }
        div.About-content p {
            font-size: 1.35em;
            font-weight: 400;
        }
        div.About-content p:nth-child(2) {
            display: initial;
        }
        div.About-image {
            display: initial;
            grid-column: 7 / 13;
            text-align: center;
            margin-top: 1.5em;
        }
        div.About-image img {
            width: 100%;
            margin: 2em;
        }
    }
</style>

<section class="About" id="NOSOTROS">
    <Title content="NOSOTROS"/>
    <div class="About-content">
        <p>
            Somos una empresa enfocada en detener el daño que se produce al medio ambiente por el desecho inadecuado del papel, plásticos y chatarras; por lo que damos a nuestros clientes un servicio de alta calidad en la recolección y reciclaje, supervisando el traslado de material a nuestro centro de reciclaje y de ahí, a su destino final.
        </p>
        <p>
            Y de esta forma, llegar a ser una empresa que promueve la recolección responsable, gestionando los materiales de manera sostenible.
        </p>
    </div>
    <div class="About-image">
        <img src="https://bit.ly/32NFuKE" alt="IMAGEN NOSOTROS">
    </div>
</section>