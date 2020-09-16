<script>
    function toggleMenu() {
        let showMenu = document.querySelector('#Navbar').dataset.show;
        showMenu = parseInt(showMenu);
        if (showMenu === 0) {
            document.querySelector('#overlay').style.display = 'block';
            document.querySelector('#Navbar').style.right = '0%';
            document.querySelector('#Navbar').dataset.show = 1;
        } else {
            document.querySelector('#overlay').style.display = 'none';
            document.querySelector('#Navbar').style.right = '-100%';
            document.querySelector('#Navbar').dataset.show = 0;
        }
    }
</script>

<style>
    div.Menubar, div.Menubar ul {
        display: grid;
        column-gap: 4%;
        grid-template-columns: repeat(4, 1fr);
        grid-column: 1 / 5;
    }
    ul li {
        list-style: none;
        display: inline-flex;
    }
    ul li:first-child {
        grid-column: 1/3;
        font-size: 1em;
        justify-content: flex-start;
        align-items: center;
    }
    ul li:last-child {
        grid-column: 4;
        justify-content: center;
        font-size: 1.6em;
        padding: 1em;
        align-items: center;
    }
    ul li i {
        color: #03045E;
        cursor: pointer;
    }
    nav.Menubar-bar {
        background-color: #0077B6;
        color:#F3F3F3;
        width: 40%;
        height: 100vh;
        position: fixed;
        right: -100%;
        top: 0;

        padding: 1em 2em;
        z-index: 5;
        border-radius: 2px;
    }
    nav.Menubar-bar li {
        list-style: none;
        text-align: center;
        padding-top: 2em;
    }
    nav.Menubar-bar li:first-child, nav.Menubar-bar li:nth-child(2) {
        padding-top: 0;
    }
    #close_menu {
        font-size: 4em;
        text-align: right;
        cursor: pointer;
    }
    #overlay {
        position: fixed;
        background-color: #3f3f3f5e;
        display: none;
        top: 0;
        bottom: 0;
        right: 0;
        left: 0;
        z-index: 2;
    }
</style>
<div class="Menubar">
    <ul class="Menubar-content">
        <li><img src="#" alt="ACCESA LOGO"></li>
        <li><i on:click={toggleMenu} class="fas fa-bars"></i></li>
    </ul>
    <nav class="Menubar-bar" data-show="0" id="Navbar">
        <li id="close_menu"><span on:click={toggleMenu}>&times;</span></li>
        <li><img src="#" alt="LOGO CORTO"></li>
        <li><a href="#NOSOTROS">NOSOTROS</a></li>
        <li><a href="#SERVICIOS">SERVICIOS</a></li>
        <li><a href="#BENEFICIOS">BENEFICIOS</a></li>
        <li><a href="#CONTACTO">CONTACTO</a></li>
    </nav>
</div>
<div id="overlay"></div>