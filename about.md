---
title: "About me"
mathjax: true
layout: page
---

<style>
/* Import crisp web font */
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&display=swap');

/* Global font settings for crisp text */
body {
  font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-rendering: optimizeLegibility;
}

/* Mobile-first responsive styles */
.soundcloud-container {
  width: 100%;
  margin-bottom: 20px;
}

.quote-container {
  text-align: center;
  padding: 20px;
  background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
  border-radius: 10px;
  margin: 20px 0;
}

.quote-container p {
  font-size: 1.1em;
  font-style: italic;
  color: #2c3e50;
  margin: 0;
  line-height: 1.6;
  font-weight: 500; /* Make quotes slightly bolder for better readability */
}

.image-right {
  float: right;
  margin-left: 20px;
  margin-bottom: 20px;
  border-radius: 8px;
  max-width: 100%;
  height: auto;
}

.image-left {
  float: left;
  margin-right: 20px;
  margin-bottom: 20px;
  border-radius: 8px;
  max-width: 100%;
  height: auto;
}

.content-text {
  text-align: justify;
  line-height: 1.6;
  font-weight: 450; /* Slightly heavier than normal for better readability */
}

/* Desktop styles */
@media (min-width: 768px) {
  .quote-container {
    margin-right: 320px;
    padding: 30px;
  }
  
  .quote-container p {
    font-size: 1.2em;
  }
  
  .image-right {
    width: 300px;
  }
  
  .image-left {
    width: 200px;
  }
}

/* Mobile styles */
@media (max-width: 767px) {
  .quote-container {
    margin-right: 140px; /* Leave space for larger image */
    padding: 15px;
  }
  
  .image-right {
    width: 130px;
    margin-left: 10px;
  }
  
  .image-left {
    width: 110px;
    margin-right: 10px;
  }
  
  .content-text {
    text-align: left;
  }
}

/* Very small screens */
@media (max-width: 480px) {
  .quote-container {
    padding: 10px;
    margin: 15px 0;
    margin-right: 110px; /* Adjust for larger image */
  }
  
  .quote-container p {
    font-size: 0.9em;
  }
  
  .image-right {
    width: 100px;
    margin-left: 8px;
  }
  
  .image-left {
    width: 85px;
    margin-right: 8px;
  }
}
</style>

<div class="soundcloud-container">
  <iframe width="100%" height="300" scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/253856343&color=%23ff5500&auto_play=false&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true&visual=true"></iframe>
  <div style="font-size: 10px; color: #cccccc;line-break: anywhere;word-break: normal;overflow: hidden;white-space: nowrap;text-overflow: ellipsis; font-family: Interstate,Lucida Grande,Lucida Sans Unicode,Lucida Sans,Garuda,Verdana,Tahoma,sans-serif;font-weight: 100;">
    <a href="https://soundcloud.com/kim-larsen-official" title="Kim Larsen" target="_blank" style="color: #cccccc; text-decoration: none;">Kim Larsen</a> · <a href="https://soundcloud.com/kim-larsen-official/sp-rge-j-rgen-1" title="Spørge Jørgen" target="_blank" style="color: #cccccc; text-decoration: none;">Spørge Jørgen</a>
  </div>
</div>

<img class="image-right" src="/assets/spgjrgn.png" alt="Spørge Jørgen illustration">

<div class="quote-container">
  <p>"Why is my nail on my finger? If it were on my nose, it would be fun." - Spørge Jørgen</p>
</div>

<div class="content-text">
This was one of the many questions asked in the children's book "Spørge Jørgen" - a tale of a boy whose endless questions drove his parents mad. I loved this book as a kid. And I love it even more as an adult. It turns out I never outgrew being the person who needs to know how everything works, and "Spørge Jørgen" reminds me that the most interesting questions are often about the ordinary things we're used to taking for granted.
And there's no shortage of things to question. I find myself drawn to everything from the synchronized movements of fish schools to the invisible dark matter that makes up most of our universe, from the unspoken rules that govern social interaction to the mysteries of human consciousness.
</div>

<img class="image-left" src="/assets/mig_mat.png" alt="Personal photo">

<div class="content-text">
What I particularly love about our world is that it offers a multitude of intellectual problems waiting to be solved or better understood. This draws on critical thinking and analytical skills, leading me to create reader's letters, research-based projects, and other creative experiments. For example, I sat on my terrace and tracked the movement of a harvestman carefully to understand its movement patterns through stochastic modeling. I made my own survey to understand which criteria parents value when they choose their kids names, and how this has changed over generations. I also made my own Python-based game (using PyGame) during my summer vacation - a game inspired by a soccer variant we came up with in the summerhouse. A full list of my projects and reader's letters can be found <a href="https://docs.google.com/document/d/1HXOMjqJpiRDGu4M3EIVrFs6nKMEAouZK_JijJE5TLFg/edit?usp=sharing">here</a>, with selected projects presented on the homepage. You can find my CV <a src="/assets/pdfs/CurriculumVitae_LarsReiter.pdf">here</a>.

</div>
