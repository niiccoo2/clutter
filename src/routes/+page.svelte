<svelte:head><link rel="icon" type="image/png" href="/favicon.png" /></svelte:head>
<head>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous" />
    <link href="https://fonts.googleapis.com/css2?family=Londrina+Shadow&family=Orbitron:wght@400;900&display=swap" rel="stylesheet" />

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous">
    <link href="https://fonts.googleapis.com/css2?family=Londrina+Shadow&family=Nata+Sans:wght@100..900&family=Orbitron:wght@400..900&display=swap" rel="stylesheet">

    <title>Clutter - YSWS</title>
    <link rel="icon" type="image/jpeg" href="/favicon.jpg" />
</head>

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

img {
  position: relative;
  z-index: -1; 
}

</style>

<body style="background-color: #594e36; overflow: hidden;"> <!-- Remove overflow hidden maybe later not for rsvp -->
    <div style="color: #7e846b; width: 102%; padding: 1rem 0; transform: rotate(10deg); box-sizing: border-box;">
        <h1 class="text-center my-nata" style="font-size: 8rem; margin: 0; text-shadow: 2px 2px 4px #000; font-weight: 700;">
            <span class="rounded-lg inline-block" style="color: #7e846b;">Clutter</span>
        </h1>
    </div>
    
    <div style="position: relative; text-align: center; transform: rotate(-5deg)">
        <img src="images/notebook_paper.png" alt="Notebook paper" style="max-width: 100%; height: auto; display: block; margin: 0 auto;">
        <!-- <h1 class="Orbitron" style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); font-size: 2rem; color: #2f2504; margin: 0;"> -->
        <h1 class="text-center londrina drab-dark-brown-2" style="text-align: center; font-size: 4rem; position: absolute; top: 50%; left: 50%; transform: translate(-50%, -160%); text-shadow: 2px 2px 4px #000; font-weight: 700; width: 80%; max-width: 600px;">
        <a href="/RSVP" class="rounded-lg inline-block" style="text-decoration: none;">RSVP here!</a>
        </h1>
        <h1 class="text-center londrina drab-dark-brown-2" style="font-size: 2rem; position: absolute; top: 50%; left: 50%; transform: translate(-50%, -33%); text-shadow: 2px 2px 4px #000; font-weight: 200; max-width: 600px; text-align: center; overflow-wrap: break-word;">
        <span class="rounded-lg inline-block" style="text-decoration: none; display: block; width: 100%;">You ship a script that <br>organizes your<br> computer, we ship you <br>something to <br>organize your desk!</span>
        </h1>
    </div>

    <div style="text-align: center; transform: rotate(0deg); margin-top: -13vh;">
        <img src="images/trash_piles.png" alt="Clutter at the bottom" style="width: 100%; height: auto; display: block; margin: 0 auto;">
    </div>
    
    <div class="text-center p-10 flex justify-center" style="margin-top: -15vh; position: relative; z-index: 1; my-nata text-shadow: 2px 2px 4px #000; font-weight: 700; color: #7e846b;">
        Made with <span class="hover:animate-bounce">❤️</span> by <a href="https://github.com/SuperNinjaCat5" style="margin-left: 0.2vw;">SuperNinjaCat5</a> 
    </div>  

    <!-- <div style="text-align: center;">
        <h1 class="text-center Orbitron" style="font-size: 4rem;">
            <a href="/RSVP" class="rounded-lg inline-block">RSVP HERE</a>
        </h1>
    </div>

    <img src="images/notebook_paper.png" alt="Notebook paper" style="display: block; margin-left: auto; margin-right: auto; max-width: 100%; height: auto;"/> -->
</body>
