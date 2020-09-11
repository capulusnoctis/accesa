<script>
    import Header from '../components/Header.svelte';
    import About from '../components/About.svelte';
    import Services from '../components/Services.svelte';
    import Benefits from '../components/Benefits.svelte';
</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Karla&family=Roboto:wght@100;300;400;500;700&display=swap');
    :global(body) {
        background-color: #FFFFFF;
        margin: 0;
        padding: 0;
    }
    div.main {
        display: grid;
        column-gap: 4%;
        grid-template-columns: repeat(4, 1fr);
        margin: auto 4%;
        z-index: -2;
    }
    /* div.main div.uno {
        background-color: #c6c9da4b;
        grid-column: 1;
        height:200vh;
    }
    div.main div.dos {
        background-color: #c6c9da4b;
        grid-column: 2;
        height:200vh;
    }
    div.main div.tres {
        background-color: #c6c9da4b;
        grid-column: 3;
        height:200vh;
    }
    div.main div.cuatro {
        background-color: #c6c9da4b;
        grid-column: 4;
        height:200vh;
    } */
</style>

<div class="main">
    <Header/>
    <About/>
    <Services/>
    <Benefits/>
    <!-- <div class="uno"></div>
    <div class="dos"></div>
    <div class="tres"></div>
    <div class="cuatro"></div> -->
</div>