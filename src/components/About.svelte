<script>
        import ProfilPicture from "../assets/Marceau.jpg";
        import Button from "../components/ButtonCTA.svelte";
        import Block from "../components/Block.svelte";

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
        ];
</script>

<section class="About">
        <img src={ProfilPicture} alt="" class="img" />
        <div class="wrapper-text">
                <h1>About</h1>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quae, esse ipsa recusandae cupiditate aperiam velit nisi nobis aliquid nostrum iure officiis quas officia numquam dignissimos voluptas quasi eveniet nam cumque.</p>
                <Button />
        </div>
        <div class="wrapper-frames-circle">
                {#each tab as info}
                        <Block icon={info.icon} title={info.title} paragraph={info.paragraph} />
                {/each}
        </div>
</section>

<style>
        .About {
                display: grid;
                grid-template-columns: repeat(2, 1fr);
                grid-template-rows: repeat(2, 1fr);
                padding: 20px;
                height: auto;
        }
        .img {
                grid-column: 1/2;
                grid-row: 1;
                width: 400px;
                height: 400px;
                /* border-radius: 50%; */
                margin: 0 auto;
                display: block;
        }
        .wrapper-text {
                grid-column: 2/3;
                grid-row: 1;
                display: flex;
                flex-direction: column;
                justify-content: center;
                align-items: left;
                gap: 20px;
                margin-top: -200px;
        }
        .wrapper-frames-circle {
                grid-column: 1/3;
                grid-row: 2;
                display: flex;
                align-items: center;
                justify-content: center;
                gap: 20px;
        }
     

        @media screen and (max-width: 768px) {
                .About {
                        grid-template-columns: 1fr;
                        height: 2000px;
                }
                .img {
                        grid-column: 1/2;
                        grid-row: 1;
                        width: 200px;
                        height: 200px;
                        align-self: center;
                }
                .wrapper-text {
                        grid-column: 1/2;
                        grid-row: 2;
                        gap: 20px;
                }
                .wrapper-frames-circle {
                        grid-column: 1/3;
                        grid-row: 3;
                        display: flex;
                        flex-direction: column;
                        align-items: center;
                        justify-content: center;
                        gap: 40px;
                }
        }
</style>
