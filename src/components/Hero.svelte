<script>
        import Button from "../components/ButtonCTA.svelte";
</script>

<section class="hero">
        <div class="wrapper-text">
        <h1>Cours de <span>Guitare</span> </h1>
     <h2>Apprenez la guitare avec un professeur passionné</h2> 
     <p>Vous souhaitez apprendre la guitare ou vous perfectionner tout en restant chez vous, dans votre confort? <br> Ne bougez surtout pas...j'arrive!</p>
      <a href="#section-form"><div class="button"><Button /></div></a>
     </div>
       
</section>

<style>
        .hero {
                display: flex;
                background-color: #49494c;
                color: white;
                background-image: url("../assets/coursdeguitare.jpg");
                background-repeat: no-repeat;
                background-size: cover;
                background-position: center;
                height: 100%;
                align-items: center;
                justify-content: center;
                padding: 50px;
                /* padding: 50px; */
        }
        .wrapper-text   {
                z-index: 1;
                display: flex;
                flex-direction: column;
                align-items: flex-start;
                justify-content: flex-start;
                gap: 20px;
                margin-top: 350px;
                background-color: #49494c;
                padding: 50px;
                border-radius: 10px 200px 80px 100px;
                margin-bottom: 40px;
                box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.486);
      
        }
        .hero h1 {
                font-family: "inter";
                letter-spacing: -0.2rem;
                font-size: 4.5rem;
                font-weight: 700;
        }
        .hero span {
                color: var(--CTA);
        }
        .hero h2 {
             
                font-size: 1.5rem;
                font-weight: 300;
        }
           .hero p {
   line-height: 25px;
                font-weight: 200;
        }
        .button {
                display: flex;
                align-items: center;
                justify-content: center;
                z-index:   0;
                margin-top: 25px;
        }
              a {
                text-decoration: none;
                color: white;
        }


@media screen and (max-width: 600px) {
  .hero{
        height:  100vh;
        align-items: center;
        justify-content: center;
        padding: 60px;

  }
        .wrapper-text {
                margin-top: 0;
                margin-left: 0px;
                        margin-top: 200px;
                       min-height: 60%;
                       border-radius: 50px;


        }
        .wrapper-text{
                max-height: 80%;
        }
        .hero h1 {
                font-size: 2.4rem;
                 flex: 1 1 auto; 
                 letter-spacing: -0.3;
        }
        .hero h2 {
                font-size: 1.2rem;
                 flex: 1 1 auto; 
        }
        .hero p {
                font-size: 0.9rem;
                 flex: 1 1 auto; 
        }
}
</style>
