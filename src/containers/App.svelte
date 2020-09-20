<script>
    import Header from '../components/Header.svelte';
    import About from '../components/About.svelte';
    import Services from '../components/Services.svelte';
    import Benefits from '../components/Benefits.svelte';
    import Contact from '../components/Contact.svelte';
    import Footer from '../components/Footer.svelte';
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
    @media (min-width: 840px) {
        div.main {
            display: grid;
            column-gap: 20px;
            grid-template-columns: repeat(12, 1fr);
            margin: auto 100px;
            z-index: -2;
        }
    }
</style>

<div class="main">
    <Header/>
    <About/>
    <Services/>
    <Benefits/>
    <Contact/>
</div>

<Footer/>