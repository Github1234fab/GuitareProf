<script>
        import FrameCircle from "./FrameCircle.svelte";

        const tabServices = [
                {
                        title: "khjfbkhs",
                        paragraph: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta dolorem dolores esse adipisci reprehenderit ",
                        icon: "icon",
                },
                {
                        title: "khjfbkhs",
                        paragraph: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta dolorem dolores esse adipisci reprehenderit ",
                        icon: "icon",
                },
                {
                        title: "khjfbkhs",
                        paragraph: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta dolorem dolores esse adipisci reprehenderit ",
                        icon: "icon",
                },
                {
                        title: "khjfbkhs",
                        paragraph: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta dolorem dolores esse adipisci reprehenderit ",
                        icon: "icon",
                },
        ];
</script>

<section class="service">
        <h1>Services</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla reprehenderit vel natus minus fuga cupiditate dolore provident inventore nesciunt consequuntur atque quidem laboriosam quaerat asperiores minima dicta nemo, modi id!</p>

        <div class="wrapper-frames-circles">
                {#each tabServices as info}
                        <FrameCircle icon={info.icon} title={info.title} paragraph={info.paragraph} />
                {/each}
                <FrameCircle />
        </div>
</section>

<style>
        .service {
                display: flex;
                flex-direction: column;
                align-items: center;
                justify-content: center;
                height: 1000px;
                gap: 50px;
                padding: 50px;
        }
        .service h1 {
                font-size: 2rem;
                font-weight: 800;
        }
        .service p {
                font-size: 1.3rem;
                font-weight: 400;
        }
        .wrapper-frames-circles {
                display: flex;
                align-items: center;
                justify-content: center;
                gap: 50px;
        }
</style>
