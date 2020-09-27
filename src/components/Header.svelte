<script>

import Menubar from "./Menubar.svelte";

</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Karla&family=Roboto&display=swap');
    header.Header {
        grid-column: 1 / 5;
    }
    div.Header-title h1 {
        font-size: 3em;
        color: #49484D;
        font-family: 'Karla', sans-serif;
        font-weight: 700;
    }
    .highlight-blue {
        color: #0077B6;
    }
    div.Header-title h2 {
        font-size: 1.9em;
        color: #49484D;
        font-family: 'Roboto', sans-serif;
        font-weight: 400;
    }
    div.Header-image {
        text-align: center;
        /* background-color: #f2e9d8; */

    }
    div.Header-image img {
        width: 90%;

    }

    @media (min-width: 840px) {
        header.Header {
            grid-column: 1 / 13;
            display: inherit;
            grid-template-columns: inherit;
            column-gap: inherit;
            align-items: center;
        }
        div.Header-title {
            grid-column: 1 / 7;
        }
        div.Header-title h1 {
            font-size: 3.5em;
            color: #49484D;
            font-family: 'Karla', sans-serif;
            font-weight: 700;
        }
        div.Header-title h2 {
            font-size: 2.5em;
            color: #49484D;
            font-family: 'Roboto', sans-serif;
            font-weight: 400;
        }
        div.Header-image {
            text-align: center;
            grid-column: 7 / 13;

        }
        div.Header-image img {
            width: 90%;
        }
        .highlight-blue {
            color: #0077B6;
        }
    }
</style>

<header class="Header">
    <Menubar/>
    <div class="Header-title">
        <h1>Accesa <span class="highlight-blue">Reciclaje</span></h1>
        <h2>Recolección y reciclaje de manera <span class="highlight-blue">inteligente</span>.</h2>
    </div>
    <div class="Header-image">
        <img src="https://ik.imagekit.io/sekosolares/Accesa/hero_oA1Cropj2.jpg" alt="HERO">
    </div>
</header>