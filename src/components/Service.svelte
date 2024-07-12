<script>
        import FrameCircle from "./FrameCircle.svelte";

        const tabServices = [
                {
                        title: "Fiabilité",
                        paragraph: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta dolorem dolores esse adipisci reprehenderit ",
                        icon: "icon",
                },
                {
                        title: "Avance de crédit d'impôt",
                        paragraph: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta dolorem dolores esse adipisci reprehenderit ",
                        icon: "icon",
                },
                {
                        title: "Tarifs compétitifs",
                        paragraph: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta dolorem dolores esse adipisci reprehenderit ",
                        icon: "icon",
                },
                // {
                //         title: "",
                //         paragraph: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta dolorem dolores esse adipisci reprehenderit ",
                //         icon: "icon",
                // },
        ];
</script>

<section class="service" id="Services">
        <h1>Services</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla reprehenderit vel natus minus fuga cupiditate dolore provident inventore nesciunt consequuntur atque quidem laboriosam quaerat asperiores minima dicta nemo, modi id!</p>

        <div class="wrapper-frames-circles">
                {#each tabServices as info}
                        <FrameCircle icon={info.icon} title={info.title} paragraph={info.paragraph} />
                {/each}
        </div>
</section>

<style>
        .service {
                display: flex;
                flex-direction: column;
                align-items: center;
                justify-content: center;
                height: auto;
                gap: 50px;
                padding: 50px;
        }
        .service h1 {
                font-weight: 800;
        }
        .service p {
                font-weight: 400;
        }
        .wrapper-frames-circles {
                display: flex;
                align-items: center;
                justify-content: center;
                gap: 30px;
        }
        @media screen and (max-width: 768px) {
        
                .wrapper-frames-circles {
                        display: flex;
                        flex-direction: column;
                        align-items: center;
                        justify-content: center;
                        gap: 40px;
                }
        }
</style>
