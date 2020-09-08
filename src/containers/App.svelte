<script>

import Header from "../components/Header.svelte";

</script>

<style>
    :global(body) {
        background-color: #FFFFFF;
        margin: 0;
        padding: 0;
    }
    div.main {
        display: grid;
        column-gap: 4%;
        grid-template-columns: repeat(4, 1fr);
        position: relative;
        margin: auto 4%;
    }
    div.main div.uno {
        background-color: #c6c9da4b;
        grid-column: 1;
        height:100vh;
    }
    div.main div.dos {
        background-color: #c6c9da4b;
        grid-column: 2;
        height:100vh;
    }
    div.main div.tres {
        background-color: #c6c9da4b;
        grid-column: 3;
        height:100vh;
    }
    div.main div.cuatro {
        background-color: #c6c9da4b;
        grid-column: 4;
        height:100vh;
    }
</style>

<div class="main">
    <Header/>
    <div class="uno"></div>
    <div class="dos"></div>
    <div class="tres"></div>
    <div class="cuatro"></div>
</div>