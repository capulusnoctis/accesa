<script>

import Menubar from "./Menubar.svelte";

</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Karla&family=Roboto&display=swap');
    div.Header {
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
    }
</style>

<div class="Header">
    <Menubar/>
    <div class="Header-title">
        <h1>Accesa <span class="highlight-blue">Reciclaje</span></h1>
    </div>
    <div class="Header-subtitle">
        <h2>Recolección y reciclaje de manera <span class="highlight-blue">inteligente</span>.</h2>
    </div>
    <div class="Header-image">
        <img src="#" alt="HERO">
    </div>
</div>