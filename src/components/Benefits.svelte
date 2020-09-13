<script>
import Title from './Title.svelte';
</script>

<style>
    div.Benefits {
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
</style>

<div class="Benefits">
    <Title content="BENEFICIOS" inlineStyle='color: #F3F3F3;' />
    <div class="Benefits-content">
        <ul>
            <li>Manejo adecuado de los materiales de Reciclaje.</li>
            <li>Cumplimiento fiscal, por medio de factura para documentar la venta.</li>
            <li>Carta de Confidencialidad (documento de compromiso para garantizar la destrucción y reciclaje).</li>
            <li>Certificado de Buenas Prácticas en Gestión de Reciclaje </li>
        </ul>
    </div>
</div>