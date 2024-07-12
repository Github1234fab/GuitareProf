<script>
        import Card from "../components/Card.svelte";
        import StratoOne from "../assets/stratocastorOne.png";

        const tab = [
                {
                        title: "Théorie",
                        subtitle: "lore zjeklfnlzej efjn elfnjz ljfkzenfj fjen fine jfj jf fj ljzenf",
                        bgImageUrl: StratoOne,
                },
                {
                        title: "Théorie",
                        subtitle: "lore zjeklfnlzej efjn elfnjz ljfkzenfj fjen fine jfj jf fj ljzenf",
                },
                {
                        title: "Théorie",
                        subtitle: "lore zjeklfnlzej efjn elfnjz ljfkzenfj fjen fine jfj jf fj ljzenf",
                },
                {
                        title: "Théorie",
                        subtitle: "lore zjeklfnlzej efjn elfnjz ljfkzenfj fjen fine jfj jf fj ljzenf",
                },
        ];
</script>

<section class="products">
        <h1>products</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta dolorem dolores esse adipisci reprehenderit deleniti quod harum eius. Illum culpa unde, tenetur ea doloribus architecto natus. Iste fugiat odio nobis?</p>
        <div class="wrapper-card">
                {#each tab as info}
                        <Card title={info.title} subtitle={info.subtitle} bgImageUrl={info.bgImageUrl} />
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
                background-color: var(--bgSectionB);
        }
        .products h1 {
                font-size: 2rem;
                font-weight: 800;
        }
        .products p {
                font-size: 1.3rem;
                font-weight: 400;
        }
        .wrapper-card {
                display: flex;
                align-items: center;
                justify-content: center;
                gap: 50px;
        }
        @media screen and (max-width: 768px) {
                .wrapper-card {
                        flex-direction: column;
                }
        }
</style>
