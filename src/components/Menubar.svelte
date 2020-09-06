<style>
    div.Menubar, div.Menubar nav {
        display: grid;
        column-gap: 4%;
        grid-template-columns: repeat(4, 1fr);
        grid-column: 1 / 5;
    }
    nav li {
        list-style: none;
        display: inline-flex;
    }
    nav li:first-child {
        grid-column: 1/3;
        font-size: 1em;
        justify-content: flex-start;
        align-items: center;
    }
    nav li:last-child {
        grid-column: 4;
        justify-content: center;
        font-size: 1.5em; 
        padding: 1.5em;
        align-items: center;
    }
    nav li i {
        color: #03045E;
        cursor: pointer;
    }
</style>
<div class="Menubar">
    <nav class="Menubar-content">
        <li><img src="#" alt="ACCESA LOGO"></li>
        <li><i class="fas fa-bars"></i></li>
    </nav>
</div>