<script>
        import Card from "../components/Card.svelte";
        import StratoOne from "../assets/stratocastorOne.png";

        const tab = [
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
        ];
</script>

<section class="products" id="Products">
        <h1>Compétences</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta dolorem dolores esse adipisci reprehenderit deleniti quod harum eius. Illum culpa unde, tenetur ea doloribus architecto natus. Iste fugiat odio nobis?</p>
        <div class="wrapper-card">
                {#each tab as info}
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
                padding: 50px;
                background-color: var(--bgSectionA);
                z-index: 0;
        }
        .products h1 {
                font-weight: 800;
                color: var(--bgHero);
        }
        .products p {
                font-weight: 400;
   color: var(--bgHero);
                line-height: 25px;
        }
        .wrapper-card {
                display: flex;
                align-items: center;
                justify-content: center;
                gap: 30px;
                flex-wrap: wrap;
        }
        @media screen and (max-width: 768px) {
                .wrapper-card {
                        flex-direction: column;
                }
        }
</style>
