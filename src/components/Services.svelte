<script>
    import Title from './Title';
</script>

<style>
    section.Services {
        grid-column: 1 / 5;
        margin-top: 6em;
    }
    div.Services-content {
        font-family: 'Roboto', sans-serif;

        color: #49484D;
    }
    div.Services-content > ul li {
        font-family: inherit;
        font-weight: 300;
        font-size: 1.5em;
        text-align: left;
        line-height: 130%;
        margin-bottom: 1.5em;
    }
    div.Services-content > ul li > ul li {
        font-size: 1em;
        margin-bottom: auto;
        font-weight: normal;
    }
    div.Services-content iframe {
        align-self: stretch;
        width: 100%;
    }

    @media (min-width: 840px) {
        section.Services {
            grid-column: 1 / 13;
            margin-top: 6em;
        }
        div.Services-content {
            display: grid;
            grid-template-columns: repeat(12, 1fr);
            column-gap: 20px;
            font-family: 'Roboto', sans-serif;

            color: #49484D;
            grid-auto-flow: dense;
            margin-top: 2em;
        }
        div.Services-content > ul {
            grid-column: 7 / 13;

            display: inherit;
            grid-template-columns: repeat(6, 1fr);
            column-gap: inherit;
            padding-inline-start: 1.5em;
        }
        div.Services-content > ul li {
            font-weight: 300;
            font-size: 1.3em;
        }
        div.Services-content > ul li:nth-child(odd) {
            grid-column: 1 / 4;
        }
        div.Services-content > ul li:nth-child(even) {
            grid-column: 4 / 7;
        }
        div.Services-content > ul li > ul li {
            font-size: 1em;
            margin-bottom: auto;
            font-weight: normal;
        }
        div.Services-content iframe {
            align-self: center;
            width: 100%;
            grid-column: 1 / 7;
        }
    }
</style>

<section class="Services" id="SERVICIOS">
    <Title content="TE APORTAMOS"/>
    <div class="Services-content">
        <ul>
            <li>Reciclaje de cartón y plásticos:
                <ul>
                    <li>Nylon</li>
                    <li>Botellas Pet</li>
                    <li>Nylon strech film</li>
                </ul>
            </li>
            <li>Manejo de archivo muerto.</li>
            <li>Asesoría y gestión en: 
                <ul>
                    <li>Recolección.</li>
                    <li>Clasificación.</li>
                    <li>Almacenaje.</li>
                </ul>
            </li>
            <li>Chatarra.</li>
            <li>Elaboración y gestión de procedimientos.</li>
            <li>Implementación de formatos.</li>
            <li>Elaboración de flujogramas.</li>
        </ul>
        <iframe width="560" height="315" title="Importancia del Reciclaje" src="https://www.youtube.com/embed/kr6J_xmbJk0" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>
</section>