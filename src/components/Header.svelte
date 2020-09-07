<script>

import Menubar from "./Menubar.svelte";

</script>

<style>
    div.Header {
        grid-column: 1 / 5;
    }
    div.Header-title {
        font-size: 28px;
        color: #49484D;
    }
    .highlight-blue {
        color: #0077B6;
    }
</style>

<div class="Header">
    <Menubar/>
    <div class="Header-title">
        <h1>Accesa <span class="highlight-blue">Reciclaje</span></h1>
    </div>
</div>