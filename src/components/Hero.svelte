<script>
        import Button from "../components/ButtonCTA.svelte";
</script>

<section class="hero">
        <h1>Des cours de guitare experts, à votre portée et à votre domicile !</h1>
        <div class="button"><Button /></div>
</section>

<style>
        .hero {
                display: grid;
                grid-template-columns: repeat(2, 1fr);
                grid-template-rows: auto;
                padding: 50px;
                background-color: #49494c;
                color: white;
        }
        .hero h1 {
                text-align: center;
                font-size: 1.5rem;
                font-weight: 300;
                grid-column: 1/3;
                grid-row: 2;
                margin-top: 50px;
        }
        .button {
                display: flex;
                align-items: center;
                justify-content: center;
                grid-column: 1/3;
                grid-row: 3;
                margin-top: 30px;
        }

</style>
