<svelte:head>
  <title>Clutter - YSWS</title>
  <link rel="icon" type="image/png" href="/favicon.png" />

  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous" />
  <link href="https://fonts.googleapis.com/css2?family=Londrina+Shadow&family=Orbitron:wght@400;900&display=swap" rel="stylesheet" />
  <link href="https://fonts.googleapis.com/css2?family=Londrina+Shadow&family=Nata+Sans:wght@100..900&family=Orbitron:wght@400..900&display=swap" rel="stylesheet" />
  <link href="https://fonts.googleapis.com/css2?family=Permanent+Marker&display=swap" rel="stylesheet" />

</svelte:head>

<style>
@import url('https://fonts.googleapis.com/css2?family=Londrina+Shadow&family=Nata+Sans:wght@100..900&family=Orbitron:wght@400..900&display=swap');

.my-londrina {
  font-family: 'Londrina Shadow', cursive;
}

.my-nata {
  font-family: 'Nata Sans', sans-serif;
}

.Orbitron {
  font-family: 'Orbitron', sans-serif;
}

.londrina {
  font-family: 'Londrina Shadow', cursive;
}

.handwritten {
  font-family: "Permanent Marker";
  font-weight: 400;
  font-style: normal;
}

.drab-dark-brown {
  color: #2f2504;
}

.drab-dark-brown-2 {
  color: #594e36; 
}

.reseda-green {
  color: #7e846b; 
}

.reseda-green2 {
  color: #afb892; 
}

.ash-gray {
  color: #a5ae9e; 
}

.platinum {
  color: #d0ddd7; 
}

.hidden {
    display: none;
}

.logo-image {
  display: block;
  width: 40vw;       
  max-width: 400px;  
  height: auto;
  margin: 0 auto;
}

@media (max-width: 768px) {
  .logo-image {
    width: 70vw;     
    max-width: 300px;
    max-height: 20vh;
  }
}

@media (max-width: 480px) {
  .logo-image {
    width: 85vw;     
    max-width: 260px;
  }
}

.trash-wrapper {
  position: fixed;      
  bottom: 0;            
  left: 50%;           
  transform: translateX(-50%) rotate(0deg);
  width: 100%;            
  text-align: center;
  z-index: 0;           
  margin: 0;        
  pointer-events: none;
}

.trash-wrapper img {
  width: 100%;          
  height: auto;
  display: block;
}



@media (max-width: 768px) {
  .trash-wrapper {
    height: auto; 
  }
}

@media (max-width: 480px) {
  .trash-wrapper {
    display: none;
    display: none;
  }
}

.made_with_heart {
  position: fixed;
  bottom: 0;
  left: 0;
  width: 100%;
  background: transparent;
  text-align: center;
  padding: 3rem 0;
  z-index: 10;
  margin-top: 0 !important;
  line-height: 4;
}

/* @media (max-width: 768px) {
  .made_with_heart {
    margin-top: 0
    font-size: 0.9rem;
    flex-direction: column;
  }
} */

@media (max-width: 375px) {
  .made_with_heart {
    display: none;
    display: none;
  }
}

html, body {
  height: 100%;
  margin: 0;
  padding: 0;
  display: flex;
  flex-direction: column;
}

img {
  position: relative;
  z-index: -1; 
}


</style>

<body style="background-color: #594e36; overflow: hidden;">
    <div style="background-color: #594e36;">
        <div style="transform: rotate(10deg); overflow-x: hidden; padding: 1rem 0;">
            <img 
                src="images/clutter_banner_website.png" 
                alt="Clutter logo" 
                class="logo-image" 
            />
        </div>

        <div style="position: relative; text-align: center; transform: rotate(-5deg); overflow-x: hidden;">
            <img src="images/notebook_paper.png" alt="Notebook paper" style="max-width: 100%; height: auto; display: block; margin: 0 auto;">
            <!-- <h1 class="Orbitron" style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); font-size: 2rem; color: #2f2504; margin: 0;"> -->
            <h1 class="text-center handwritten" style="color: #334195; text-align: center; font-size: 3rem; position: absolute; top: 50%; left: 50%; transform: translate(-50%, -180%); font-weight: 700; width: 80%; max-width: 600px;">
            <a href="/RSVP" class="rounded-lg inline-block londrina" style="text-decoration: underline; color: #7e846b;">RSVP here!</a>
            </h1>
            <h1 class="text-center handwritten drab-dark-brown-2" style="color: #334195; font-size: 1.6rem; position: absolute; top: 50%; left: 50%; transform: translate(-50%, -25%); font-weight: 200; max-width: 600px; text-align: center; overflow-wrap: break-word;">
            <span class="rounded-lg inline-block drab-dark-brown-2" style="text-decoration: none; display: block; width: 100%; line-height: 1.4; ">You ship a script <br/>to organizes your<br> digital life, we ship you <br>something to <br>organize your<br> physical life!</span>
            </h1>
        </div>
        <div class="text-center p-10 flex justify-center made_with_heart" style="position: relative; z-index: 1; font-weight: 700; color: #7e846b;">
            Made with  <span class="hover:animate-bounce">❤️</span>  by <a href="https://github.com/SuperNinjaCat5" style="margin-left: 0.2vw; margin-right: 0.2vw;"> Ben </a> & <a href="https://github.com/niiccoo2" style="margin-left: 0.2vw; margin-right: 0.2vw;"> Nico </a> 
        </div>  
        <div class="trash-wrapper trash-image">
          <img src="images/trash_piles.png" alt="Clutter at the bottom">
        </div>
    </div>
</body>
