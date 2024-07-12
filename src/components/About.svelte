<script>
        import ProfilPicture from "../assets/Marceau.jpg";
        import Button from "../components/ButtonCTA.svelte";
        import FrameCircle from "../components/FrameCircle.svelte";

        let tab = [
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

<section class="About">
        <img src={ProfilPicture} alt="" class="img" />
        <div class="wrapper-text">
                <h1>About</h1>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quae, esse ipsa recusandae cupiditate aperiam velit nisi nobis aliquid nostrum iure officiis quas officia numquam dignissimos voluptas quasi eveniet nam cumque.</p>
                <div class="wrapper-frames-circle">
                        {#each tab as info}
                                <FrameCircle icon={info.icon} title={info.title} paragraph={info.paragraph} />
                        {/each}
                </div>
        </div>
        <Button />
</section>

<style>
        .About {
                display: grid;
                grid-template-columns: repeat(2, 1fr);
                grid-template-rows: auto;
                padding: 50px;
                height: auto;
        }
        .img {
                width: 400px;
                height: 400px;
                /* border-radius: 50%; */
                margin: 0 auto;
                display: block;
                grid-column: 1/2;
                grid-row: 1;
        }
        .wrapper-text {
                grid-column: 2/3;
                grid-row: 1;
                display: flex;
                flex-direction: column;
                justify-content: space-around;
                align-items: left;
                padding: 50px;
        }
        .wrapper-frames-circle {
                display: flex;
                align-items: center;
                justify-content: center;
                gap: 50px;
        }

        @media screen and (max-width: 768px) {
                .About {
                        grid-template-columns: 1fr;
                }
                .img {
                        grid-column: 1/2;
                        grid-row: 1;
                        width: 300px;
                        height: 300px;
                        align-self: center;
                }
                .wrapper-text {
                        grid-column: 1/2;
                        grid-row: 2;
                        padding: 20px;
                        gap: 40px;
                }
        }
</style>
