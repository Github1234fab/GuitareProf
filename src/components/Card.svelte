<script>
        export let title;
        export let subtitle;
        export let bgImageUrl;
</script>

<div class="wrapper-card">
        <div class="card" style="background-image: url({bgImageUrl})"></div>
        <h1>{title}</h1>
        <p class="paragraph">{subtitle}</p>
</div>

<style>
        .wrapper-card {
                display: flex;
                flex-direction: column;
                align-items: center;
                justify-content: center;
                gap: 10px;
        }
        .card {
                background-size: cover;
                background-position: center;
                min-width: 300px;
                min-height: 300px;
        }
        .wrapper-card h1 {
                color: var(--bgHeader);
                text-align: center;
                font-size: 1.5rem;
        }
        .paragraph {
                color: var(--bgHeader);
                text-align: center;
                font-size: 1.2rem;
                font-weight: 400;
        }
</style>
