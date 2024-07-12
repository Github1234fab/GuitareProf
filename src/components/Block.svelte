<script>
        export let title;
        export let paragraph;
</script>

<div class="block">
        <div class="wrapper-text">
                <h1>{title}</h1>
                <p>{paragraph}</p>
        </div>
</div>


<style>

        .block {
                display: flex;
                flex-direction: column;
                align-items: center;
                justify-content: center;
                gap: 50px;
                padding: 50px;
                box-shadow: 0px 0px 20px  rgba(0, 0, 0, 0.142);
                border-radius: 8px;
        }
        .wrapper-text {
                display: flex;
                flex-direction: column;
                align-items: center;
                justify-content: center;
                gap: 20px;
        }
        h1 {
                color: var(--bgHeader); 
                font-size: 2rem;
                font-weight: 800;
                text-align: center;
        }
        p {
                color: var(--bgHeader); 
                font-size: 1.3rem;
                font-weight: 400;
                text-align: center;
        }

</style>

