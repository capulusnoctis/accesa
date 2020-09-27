<script>
import Title from './Title.svelte';

function checkFormat() {
    let phLength = event.target.value.length;
    if(phLength === 4)
        event.target.value += ' ';
    if(phLength === 9)
        event.target.value += ' ';
}
</script>

<style>
    section.Contact {
        grid-column: 1 / 5;
        margin-top: 12em;
        padding-top: 3em;
    }
    div.Contact-content {
        font-family: 'Roboto', sans-serif;

        color: #49484D;
    }
    div.Contact-content p {
        font-family: inherit;
        font-weight: 300;
        font-size: 1.5em;
        text-align: left;
        line-height: 135%;
    }
    div.Contact-content form {
        grid-column: 1 / 5;
        display: grid;
        font-size: 1.5em;
    }
    div.Contact-content form label {
        display: block;
        font-weight: 300;
    }
    div.Contact-content form input,
    div.Contact-content form textarea,
    div.Contact-content form button {
        border: 1px solid #0077B6;
        border-radius: 5px;
        padding: 6px;
        grid-column: 1 / 5;
        font-size: 1em;
        font-weight: 300;
        font-family: inherit;
        margin-bottom: 1em;
    }
    div.Contact-content form input {
        height: 24px;
    }
    div.Contact-content form textarea {
        height: 3em;
    }
    div.Contact-content form input::placeholder,
    div.Contact-content form textarea::placeholder {
        font-weight: 300;
        font-size: 0.8em;
    }
    div.Contact-content form button {
        background-color: #0077B6;
        color: #F3F3F3;
        cursor: pointer;
    }

    div.content-list {
        grid-column: 1 / 5;
        display: grid;
        grid-template-columns: auto auto auto;
        text-align: center;
    }
    div.content-list div i {
        font-size: 47px;
        color: #0077B6;
    }
    .annotation {
        display: none;
    }
    @media (min-width: 840px) {
        section.Contact {
            grid-column: 1 / 13;
        }
        div.Contact-content {
            display: grid;
            grid-template-columns: repeat(12, 1fr);
            column-gap: 20px;
            font-family: 'Roboto', sans-serif;

            color: #49484D;
        }
        div.Contact-content p {
            text-align: center;
        }
        div.Contact-content p:nth-child(1) {
            grid-column: 1 / 7;
        }
        div.Contact-content p:nth-child(3) {
            grid-column: 7 / 13;
            grid-row: 1;
        }
        div.Contact-content form {
            grid-column: 7 / 13;
            display: grid;
            font-size: 1.35em;
        }
        div.content-list {
            grid-column: 1 / 7;
            display: block;
            text-align: left;
        }
        div.content-list div {
            margin-top: 3em;
        }
        div.content-list div a {
            text-decoration: none;
            color: #0077B6;
            font-size: 1.35em;
            align-items: center;
        }
        div.content-list div a i {
            font-size: 47px;
            color: #0077B6;
        }
        .annotation {
            display: initial;
            color: inherit;
            font-family: inherit;
            font-size: inherit;
            padding-left: 2em;
        }
    }
</style>

<section class="Contact" id="CONTACTO">
    <Title content="CONTACTO"/>
    <div class="Contact-content">
        <p>
            ¿Tienes interés? Puedes contactarnos por cualquiera de los siguientes medios:
        </p>
        <div class="content-list">
            <div>
                <a href="https://api.whatsapp.com/send?phone=+502-3284-2891" target="_blank"><i class="fab fa-whatsapp"></i><span class="annotation">+502 3284 2891</span></a>
                <!-- <a href="https://api.whatsapp.com/send?phone=+50241" target="_blank"><i class="fab fa-whatsapp"></i></a> -->
            </div>
            <!-- <div>
                <a href="#"><i class="fab fa-facebook"></i></a>
            </div> -->
            <div>
                <a href="mailto:reciclaje@accesagroup.com"><i class="fas fa-envelope"></i><span class="annotation">reciclaje@accesagroup.com</span></a>
            </div>
            <div>
                <a href="tel:+502-3284-2891"><i class="fas fa-phone-alt"></i><span class="annotation">+502 3284 2891</span></a>
            </div>
        </div>
        <p>
            O puedes llenar el siguiente formulario:
        </p>
        <form name="contact" method="POST">
            <input type="hidden" name="form-name" value="contact" />
            <label for="inNombre">Nombre:</label>
            <input type="text" name="name" id="inNombre" placeholder="Tu Nombre" required>

            <label for="inLastName">Apellido:</label>
            <input type="text" name="last_name" id="inLastName" placeholder="Tu Apellido" required>

            <label for="inEmail">Email:</label>
            <input type="email" name="email" id="inEmail" placeholder="Tu correo electrónico">

            <label for="inPhone">Teléfono:</label>
            <input type="tel" value="" maxlength="14" on:keydown={checkFormat} name="phone" id="inPhone" placeholder="Tu teléfono. (Ej. +502 1234 5678)" required>
            
            <label for="inMessage">Mensaje:</label>
            <textarea name="message" id="inMessage" placeholder="Tu mensaje" required></textarea>
            
            <button type="submit" class="button-submit">Enviar</button>
        </form>
    </div>
</section>