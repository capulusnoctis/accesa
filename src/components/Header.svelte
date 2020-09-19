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
    div.Header-subtitle h2 {
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
</style>

<header class="Header">
    <Menubar/>
    <div class="Header-title">
        <h1>Accesa <span class="highlight-blue">Reciclaje</span></h1>
    </div>
    <div class="Header-subtitle">
        <h2>Recolección y reciclaje de manera <span class="highlight-blue">inteligente</span>.</h2>
    </div>
    <div class="Header-image">
        <img src="https://bit.ly/3iX1FU8" alt="HERO">
    </div>
</header>