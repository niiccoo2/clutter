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

.handwritten {
  font-family: "Permanent Marker";
  font-weight: 400;
  font-style: normal;
}

.handwritten-big {
  font-family: "Permanent Marker";
  font-weight: 500;
  font-style: normal;
}

.drab-dark-brown-2 {
  color: #594e36; 
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

@media (max-width: 768px) {
  .names {
    margin-left: 0.4vw !important;  
    margin-right: 0.4vw !important;
  }
  .y_tag {
    margin-right: 0.4vw !important;  
  }
}

body {
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

<body style="background-color: #594e36;">
    <div style="background-color: #594e36; overflow: hidden;">
        <div style="transform: rotate(10deg); overflow-x: hidden; padding: 1rem 0;">
            <img 
                src="images/clutter_banner_website.png" 
                alt="Clutter logo" 
                class="logo-image" 
            />
        </div>

        <div style="position: relative; text-align: center; transform: rotate(-5deg); overflow-x: hidden; overflow: hidden;">
            <img src="images/notebook_paper.png" alt="Notebook paper" style="max-width: 100%; height: auto; display: block; margin: 0 auto;">
            <h1 class="text-center handwritten drab-dark-brown-2" style="color: #334195; font-size: 1.6rem; position: absolute; top: 50%; left: 50%; transform: translate(-50%, -41%); font-weight: 200; max-width: 600px; text-align: center; overflow-wrap: break-word;">
            <span class="rounded-lg inline-block drab-dark-brown-2" style="text-decoration: none; display: block; width: 100%; line-height: 1.1; ">You ship a script <br/>that organizes your<br> digital life, <br> we ship you stuff to <br>organize your<br> physical life! <br><br> ‎‎‎‎‎‎‎  ‎  ‎  ‎  ‎ </span>
            </h1>
        </div>
        
        <br>
        <br>

        <div style="position: relative; text-align: center; padding: 1rem; display: flex; justify-content: center; gap: 2rem;">
          <button style="background-color: #e9e7d9" class="handwritten-big drab-dark-brown-2 p-4 rounded hover:scale-105">
            <a href="/RSVP">RSVP</a>
          </button>
          <button style="background-color: #e9e7d9" class="handwritten-big drab-dark-brown-2 p-4 rounded hover:scale-105">
            <a href="/rewards">REWARDS</a>
          </button>
        </div>



        <div class="text-center p-10 flex justify-center made_with_heart" style="position: relative; z-index: 1; font-weight: 700; color: #7e846b; overflow: hidden;">
            Made with  <span class="hover:animate-bounce">❤️</span>  b<a href="/3.14" class="y_tag">y</a> <a href="https://github.com/SuperNinjaCat5" style="margin-left: 0.2vw; margin-right: 0.2vw;" class="names"> Ben </a> & <a href="https://github.com/niiccoo2" style="margin-left: 0.2vw; margin-right: 0.2vw;" class="names"> Nico </a> 
        </div>  
        <div class="trash-wrapper trash-image" style="overflow: hidden;">
          <img src="images/trash_piles.png" alt="Clutter at the bottom">
        </div>
    </div>
</body>
