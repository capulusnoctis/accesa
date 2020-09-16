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
</style>

<section class="About" id="NOSOTROS">
    <Title content="NOSOTROS"/>
    <div class="About-content">
        <p>
            Somos una empresa enfocada en detener el daño que se produce al medio ambiente por el desecho inadecuado del papel, plásticos y chatarras; por lo que damos a nuestros clientes un servicio de alta calidad en la recolección y reciclaje, supervisando el traslado de material a nuestro centro de reciclaje y de ahí, a su destino final.
        </p>
    </div>
</section>