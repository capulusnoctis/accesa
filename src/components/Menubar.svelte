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
    function setSelected() {
        let anchorCollection = document.querySelectorAll('nav.Menubar-bar li a');
        let selectedAnchor = event.target;
        
        for(let a of anchorCollection)
            a.classList.style.borderBottom = '2px solid transparent';

        selectedAnchor.style.borderBottom = '2px solid #F3F3F3';
    }
</script>

<style>
    div.Menubar, div.Menubar ul {
        display: grid;
        column-gap: 4%;
        grid-template-columns: repeat(4, 1fr);
        grid-column: 1 / 5;
        padding: 0;
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
        justify-content: flex-end;
        font-size: 1.6em;
        padding: 1em;
        align-items: center;
    }
    ul li i {
        color: #03045E;
        cursor: pointer;
    }
    ul.Menubar-content img {
        height: 6.5em;
    }
    nav.Menubar-bar {
        background-color: #0077B6;
        color:#F3F3F3;
        width: 45%;
        height: 100vh;
        position: fixed;
        right: -100%;
        top: 0;

        padding: 1em 2em;
        z-index: 5;
        border-radius: 2px;
    }
    nav.Menubar-bar img {
        height: 5em;
    }
    nav.Menubar-bar li {
        list-style: none;
        text-align: center;
        padding-top: 2.5em;
    }
    nav.Menubar-bar li:first-child, nav.Menubar-bar li:nth-child(2) {
        padding-top: 0;
    }
    nav.Menubar-bar li a {
        color: inherit;
        font-family: 'Karla', Arial, Helvetica, sans-serif;
        font-size: 1.25em;
        letter-spacing: 0.3em;
        text-decoration: none;
        padding-bottom: 1em;
    }
    nav.Menubar-bar li a:hover {
        border-bottom: 2px solid #F3F3F3;
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

    @media (min-width: 840px) {
        div.Menubar, div.Menubar ul {
            display: grid;
            column-gap: 20px;
            grid-template-columns: repeat(12, 1fr);
            grid-column: 1 / 13;
            padding: 0;
        }
        ul li {
            list-style: none;
            display: inline-flex;
        }
        ul li:first-child {
            grid-column: 1 / 3;
            font-size: 1em;
            justify-content: flex-start;
            align-items: center;
        }
        ul li:last-child {
            grid-column: 12;
        }
    }

    @media (min-width: 1200px) {
        div.Menubar {
            display: inherit;
            grid-template-columns: inherit;
            column-gap: inherit;
            padding: 0;
            grid-column: 1 / 13;
        }
        div.Menubar ul {
            grid-column: 1;

            display: initial;
            grid-template-columns: unset;
            column-gap: unset;
            padding: 0;
        }
        nav.Menubar-bar {
            background-color: inherit;
            color:#03045E;
            width: auto;
            height: auto;
            position: initial;
            right: unset;
            top: unset;
            display: inline-block;
            grid-column: 3 / 13;
            text-align: right;
            padding: 1em 2em;
            z-index: 0;
            border-radius: 0;
        }
        nav.Menubar-bar li {
            list-style: none;
            display: inline-block;
            text-align: center;
            padding: 2em 1em;
        }
        nav.Menubar-bar li a {
            color: inherit;
            font-family: 'Karla', Arial, Helvetica, sans-serif;
            font-size: 1.25em;
            letter-spacing: 0.3em;
            text-decoration: none;
            padding-bottom: 1em;
        }
        nav.Menubar-bar li a:hover {
            border-bottom: 2px solid #0077B6;
            color: #0077B6;
        }
        ul.Menubar-content li:nth-child(2),
        nav.Menubar-bar li:first-child,
        nav.Menubar-bar li:nth-child(2) {
            display: none;
        }
    }
</style>
<div class="Menubar">
    <ul class="Menubar-content">
        <li><img src="https://bit.ly/3c6fld6" alt="ACCESA LOGO"></li>
        <li><i on:click={toggleMenu} class="fas fa-bars"></i></li>
    </ul>
    <nav class="Menubar-bar" data-show="0" id="Navbar">
        <li id="close_menu"><span on:click={toggleMenu}>&times;</span></li>
        <li><img src="https://bit.ly/3my1P6U" alt="LOGO CORTO"></li>
        <li><a href="#NOSOTROS">NOSOTROS</a></li>
        <li><a href="#SERVICIOS">SERVICIOS</a></li>
        <li><a href="#BENEFICIOS">BENEFICIOS</a></li>
        <li><a href="#CONTACTO">CONTACTO</a></li>
    </nav>
</div>
<div id="overlay" on:click={toggleMenu}></div>