<script>
    import Title from './Title';
</script>

<style>
    div.Services {
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
    div.Services-content video {
        align-self: stretch;
        width: 100%;
    }
</style>

<div class="Services">
    <Title content="TE APORTAMOS"/>
    <div class="Services-content">
        <ul>
            <li>Manejo de archivo muerto.</li>
            <li>
                Reciclaje de cartón y plásticos:
                <ul>
                    <li>Nylon</li>
                    <li>Botellas Pet</li>
                    <li>Nylon strech film</li>
                </ul>
            </li>
            <li>Chatarra.</li>
            <li>
                Asesoría y gestión en: 
                <ul>
                    <li>Recolección.</li>
                    <li>Clasificación.</li>
                    <li>Almacenaje.</li>
                </ul>
            </li>
            <li>Elaboración y gestión de procedimientos.</li>
            <li>Implementación de formatos.</li>
            <li>Elaboración de flujogramas.</li>
        </ul>
        <video controls></video>
    </div>
</div>