<script>
import Title from './Title.svelte';
</script>

<style>
    section.Benefits {
        grid-column: 1 / 5;
        margin-top: 6em;
        padding-top: 2em;
        
        background-color: #0077B6;
    }
    div.Benefits-content {
        font-family: 'Roboto', sans-serif;
        padding: 1em 2em 2em 1em;

        color: #F3F3F3;
    }
    div.Benefits-content > ul li {
        font-family: inherit;
        font-weight: 300;
        font-size: 1.5em;
        text-align: left;
        line-height: 130%;
        margin-bottom: 1.5em;
    }
    @media (min-width: 840px) {
        section.Benefits {
            display: grid;
            grid-template-columns: inherit;
            column-gap: inherit;
            width: 98.5vw;
            margin-left: -100px;
            padding-top: 1em;
        }
        div.Benefits-content {
            grid-column: 1 / 13;
            padding: 0;

            display: inherit;
            grid-template-columns: inherit;
            column-gap: inherit;
            margin: auto 100px;
        }
        div.Benefits-content > ul {
            grid-column: 1 / 7;
            padding-inline-start: 1.5em;
        }
        div.Benefits-content > ul li {
            font-family: inherit;
            font-weight: 300;
            font-size: 1.3em;
            text-align: left;
            line-height: 130%;
            margin-bottom: 1.5em;
        }
    }
</style>

<section class="Benefits" id="BENEFICIOS">
    <Title content="BENEFICIOS" inlineStyle='color: #F3F3F3;' />
    <div class="Benefits-content">
        <ul>
            <li>Manejo adecuado de los materiales de Reciclaje.</li>
            <li>Cumplimiento fiscal, por medio de factura para documentar la venta.</li>
            <li>Carta de Confidencialidad (documento de compromiso para garantizar la destrucción y reciclaje).</li>
            <li>Certificado de Buenas Prácticas en Gestión de Reciclaje </li>
        </ul>
    </div>
</section>