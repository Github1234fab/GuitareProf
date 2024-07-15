<script>
        import Card from "../components/Card.svelte";
        import StratoOne from "../assets/stratocastorOne.png";

        const tabA = [
                {
                        title: "Connaissances de base",
                },
                {
                        title: "Arpèges",
                },
                {
                        title: "Improvisation",
                },
                {
                        title: "Accords",
                },
                {
                        title: "Rythmiques",
                },
                {
                        title: "Song&Tab",
                },
        ];
        const tabB = [
                {
                        title: "Théorie musicale",
                },
                {
                        title: "Riffs",
                },
                {
                        title: "Gammes & modes",
                },
                {
                        title: "Techniques de jeu",
                },
                {
                        title: "Harmonie",
                },
                {
                        title: "Étude de Styles",
                },
        ];
</script>

<section class="products" id="Products">
        <h1>Compétences</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta dolorem dolores esse adipisci reprehenderit deleniti quod harum eius. Illum culpa unde, tenetur ea doloribus architecto natus. Iste fugiat odio nobis?</p>
        <div class="wrapper-cardA">
                {#each tabA as info}
                        <Card title={info.title} />
                {/each}
        </div>
        <div class="wrapper-cardB">
                {#each tabB as info}
                        <Card title={info.title} />
                {/each}
        </div>
</section>

<style>
        .products {
                display: flex;
                flex-direction: column;
                align-items: center;
                justify-content: center;
                height: auto;
                gap: 50px;
                padding: 100px;
                background: radial-gradient(rgb(109, 109, 212), rgb(10, 10, 105));
                z-index: 0;
        }
        .products h1 {
                font-weight: 800;
                color: var(--white);
        }
        .products p {
                font-weight: 400;
                color: var(--white);
                line-height: 25px;
        }
        .wrapper-cardA,
        .wrapper-cardB {
                display: flex;
                align-items: center;
                justify-content: center;
                gap: 30px;
                flex-wrap: wrap;
                width: 100%;
        }

        @media screen and (max-width: 1375px) {
                .wrapper-cardA,
                .wrapper-cardB {
                        display: flex;
                        align-items: center;
                        justify-content: center;
                        flex-wrap: wrap;
                        gap: 40px;
                        width: 60%;
                }
        }
</style>
