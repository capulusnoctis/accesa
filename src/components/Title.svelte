<script>
    export let content = "NO CONTENT";
    export let inlineStyle = 'display: initial;';
</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Karla&family=Roboto&display=swap');
    div.Title {
        text-align: center;
        grid-column: 1 / 5;
    }
    div.Title h3 {
        grid-column: inherit;
        color: #03045E;
        font-family: 'Karla', sans-serif;
        font-weight: 400;
        font-size: 2.3em;
        letter-spacing: 0.3em;
    }
    @media (min-width: 840px) {
        div.Title {
            text-align: center;
            grid-column: 1 / 13;
        }
        div.Title h3 {
            grid-column: inherit;
            color: #03045E;
            font-family: 'Karla', sans-serif;
            font-weight: 400;
            font-size: 2.3em;
            letter-spacing: 0.3em;
        }
    }
</style>

<div class="Title">
    <h3 style="{inlineStyle}">{content}</h3>
</div>