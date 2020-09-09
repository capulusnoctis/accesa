<script>
    export let content = "NO CONTENT";
</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Karla:wght@700&family=Roboto&display=swap');
    div.Title {
        grid-column: 1 / 5;
        text-align: center;
    }
    div.Title h3 {
        grid-column: inherit;
        color: #03045E;
        font-family: 'Karla', sans-serif;
    }
</style>

<div class="Title">
    <h3>{content}</h3>
</div>