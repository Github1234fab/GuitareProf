<script>
        export let title;
        export let subtitle;
        export let bgImageUrl;
</script>

<div class="card" style="background-image: url({bgImageUrl})">
        <h1>{title}</h1>
        <p>{subtitle}</p>
</div>

<style>
        .card {
                display: flex;
                align-items: center;
                justify-content: center;
                background-size: cover;
                background-position: center;
                min-width: 300px;
                height: 500px;
                padding: 50px;
                background-color: var(--white);
                color: white;
                position: relative;
                box-shadow: 0px 0px 10px 0px rgba(0, 0, 0, 0.75);
        }
        .card h1 {
                color: var(--bgHeader);
                text-align: center;
                font-size: 1.5rem;
                position: absolute;
                top: 550px;
        }
        .card p {
                color: var(--bgHeader);
                text-align: center;
                font-size: 1.2rem;
                font-weight: 400;
                position: absolute;
                top: 650px;
        }
</style>
