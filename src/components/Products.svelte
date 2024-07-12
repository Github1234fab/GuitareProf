<script>
        import Card from "../components/Card.svelte";
        import StratoOne from "../assets/stratocastorOne.png";

        const tab = [
                {
                        title: "Théorie",
                        subtitle: "vekhrbvekrhbvkerhbvkehrbvkherbvvnfslnvslfjnvlsjfnv",
                        bgImageUrl: StratoOne,
                },
                {
                        title: "Théorie",
                        subtitle: "vekhrbvekrhbvkerhbvkehrbvkherbvsfvsfvfvfsvsfv",
                },
                {
                        title: "Théorie",
                        subtitle: "vekhrbvekrhbvkerhbvkehrbvkherbvsfvsfvsfvsfv",
                },
                {
                        title: "Théorie",
                        subtitle: "vekhrbvekrhbvkerhbvkehrbvkherbvsfvsfvsfvsfvsfvsfvsfvfsv",
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
                height: 2000px;
                gap: 50px;
                padding: 50px;
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
                flex-wrap: wrap;
                gap: 150px;
        }
</style>
