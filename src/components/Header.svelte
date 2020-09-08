<script>

import Menubar from "./Menubar.svelte";

</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Karla:wght@700&family=Roboto&display=swap');
    div.Header {
        grid-column: 1 / 5;
    }
    div.Header-title h1 {
        font-size: 3.3em;
        color: #49484D;
        font-family: 'Karla', sans-serif;
        font-weight: 700;
    }
    .highlight-blue {
        color: #0077B6;
    }
    div.Header-subtitle h2 {
        font-size: 1.5em;
        color: #49484D;
        font-family: 'Roboto', sans-serif;
        font-weight: 400;
    }
    div.Header-image {
        text-align: center;
    }
    div.Header-image i:first-child {
        position: absolute;
        left: 5.83%;
        right: 5.56%;
        top: 32%;
        bottom: 82.61%;
        font-size: 25em;
        z-index: 0;
        color: #CAF0F8;
    }
    div.Header-image i:last-child {
        position: absolute;
        left: 16.94%;
        right: 16.67%;
        top: 38%;
        bottom: 85.11%;
        z-index: 1;
        color: #5F6A6E;
        font-size: 15em;
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
        <i class="fas fa-recycle"></i>
        <i class="fas fa-mountain"></i>
    </div>
</div>