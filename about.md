---
title: "About me"
mathjax: true
layout: page
---

<style>
.about-quote {
  text-align: center;
  padding: 1.6em 2em;
  background: rgba(56, 189, 248, 0.04);
  border: 1px solid rgba(56, 189, 248, 0.15);
  border-radius: 8px;
  margin: 0.5em 0 2.5em;
  position: relative;
}

.about-quote::before {
  content: "\201C";
  display: block;
  font-size: 2.6em;
  line-height: 0.5;
  color: rgba(56, 189, 248, 0.55);
  margin-bottom: 0.25em;
  font-family: Georgia, serif;
}

.about-quote p {
  font-size: 1.08em;
  font-style: italic;
  color: #cfdce7;
  margin: 0;
  line-height: 1.7;
  text-align: center;
}

.about-row {
  display: grid;
  grid-template-columns: 1fr 230px;
  gap: 2.5em;
  align-items: center;
  margin: 0 0 2.5em;
}

.about-row.reverse {
  grid-template-columns: 200px 1fr;
}

.about-row figure {
  margin: 0;
}

.about-row img {
  display: block;
  width: 100%;
  margin: 0;
  border-radius: 8px;
  border: 1px solid rgba(56, 189, 248, 0.18);
  transition: border-color 0.2s, box-shadow 0.2s;
}

.about-row img:hover {
  border-color: rgba(56, 189, 248, 0.45);
  box-shadow: 0 0 16px rgba(56, 189, 248, 0.1);
}

.about-text {
  line-height: 1.75;
  color: #cfdce7;
}

.soundcloud-card {
  margin-top: 3em;
  padding-top: 1.5em;
  background: linear-gradient(to right, rgba(56, 189, 248, 0.45), rgba(56, 189, 248, 0.05)) no-repeat top / 100% 1px;
}

.soundcloud-container {
  width: 100%;
  border-radius: 8px;
  overflow: hidden;
  border: 1px solid rgba(56, 189, 248, 0.15);
}

@media (max-width: 700px) {
  .about-row,
  .about-row.reverse {
    grid-template-columns: 1fr;
    gap: 1.5em;
  }
  .about-row .about-text {
    order: 1;
  }
  .about-row figure {
    order: 2;
    max-width: 240px;
    margin: 0 auto;
  }
}
</style>

<div class="about-quote">
  <p>"Why is my nail on my finger?" - Spørge Jørgen</p>
</div>

<div class="about-row">
  <div class="about-text">
This was one of the many questions asked in the children's book "Spørge Jørgen" -- a tale of a boy whose endless questions drove his parents mad. I loved this book as a kid. I still love it today. "Spørge Jørgen" reminds me that the world is a weird place, and there is much to understand. Like Spørge Jørgen, I love to ask questions and I find myself drawn to everything from the synchronized movements of fish schools to the invisible dark matter that makes up most of our universe, from the unspoken rules that govern social interaction to the mysteries of human consciousness.
  </div>
  <figure>
    <img src="/assets/spgjrgn.png" alt="Spørge Jørgen illustration">
  </figure>
</div>

<div class="about-row reverse">
  <figure>
    <img src="/assets/mig_mat.png" alt="Personal photo">
  </figure>
  <div class="about-text">
The world offers a multitude of intellectual problems that demands critical thinking and analytical skills, leading me to create reader's letters, personal research projects, and various homemade experiments. For example, I sat on my terrace and tracked the movement of a harvestman carefully to understand its movement patterns through stochastic modeling. I made my own survey to identify how parents weight different criteria when naming their kids, and how this has changed over generations. I also made my (first) Python game -- a game based on a soccer variant invented during my summer vacation. Here on my homepage you can find a selected (tiny) fraction of my intellectual work.
  </div>
</div>

<div class="soundcloud-card">
  <div class="soundcloud-container">
    <iframe width="100%" height="166" scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/253856343&color=%2338bdf8&auto_play=false&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true&visual=false"></iframe>
    <div style="font-size: 10px; color: #cccccc;line-break: anywhere;word-break: normal;overflow: hidden;white-space: nowrap;text-overflow: ellipsis; font-family: Interstate,Lucida Grande,Lucida Sans Unicode,Lucida Sans,Garuda,Verdana,Tahoma,sans-serif;font-weight: 100;">
      <a href="https://soundcloud.com/kim-larsen-official" title="Kim Larsen" target="_blank" style="color: #cccccc; text-decoration: none;">Kim Larsen</a> · <a href="https://soundcloud.com/kim-larsen-official/sp-rge-j-rgen-1" title="Spørge Jørgen" target="_blank" style="color: #cccccc; text-decoration: none;">Spørge Jørgen</a>
    </div>
  </div>
</div>
