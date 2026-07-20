---
layout: default
title: Thoughts
favicon: /assets/favicon-thoughts.svg
---
<style>
.thoughts-intro {
  font-size: 1.05em;
  line-height: 1.65;
  color: rgba(196, 212, 224, 0.8);
  margin-bottom: 8px;
  margin-top: 24px;
  text-align: center;
  padding: 0 20px;
}
.thought-bubble-wrap {
  display: flex;
  flex-direction: column;
  align-items: center;
  max-width: 640px;
  margin: 32px auto 0;
  padding: 0 20px;
}
.thought-bubble {
  background: rgba(13, 17, 23, 0.85);
  border: 1px solid rgba(255, 255, 255, 0.8);
  border-radius: 32px;
  padding: 2em 2.2em;
  box-shadow: 0 8px 32px rgba(56, 189, 248, 0.08);
  text-align: center;
  opacity: 1;
  transition: opacity .2s ease;
  width: 100%;
  box-sizing: border-box;
}
.quote-en {
  font-size: 1.25em;
  line-height: 1.55;
  color: #f1f5f9;
  font-weight: 500;
  margin: 0;
}
.quote-da {
  font-size: .85em;
  line-height: 1.5;
  color: #f87171;
  margin: .7em 0 0;
}
.thought-trail {
  display: flex;
  align-items: center;
  gap: 10px;
  align-self: flex-start;
  margin: 14px 0 28px 15%;
}
.thought-trail span {
  display: block;
  border-radius: 50%;
  background: rgba(13, 17, 23, 0.85);
  border: 1px solid rgba(255, 255, 255, 0.8);
}
.thought-trail span:nth-child(1) { width: 20px; height: 20px; }
.thought-trail span:nth-child(2) { width: 13px; height: 13px; }
.thought-trail span:nth-child(3) { width: 7px; height: 7px; }
.new-thought-btn {
  border-radius: 6px;
  border: 1px solid rgba(56, 189, 248, 0.45);
  background: transparent;
  padding: .55em 1.4em;
  color: #38bdf8;
  font-size: .95em;
  font-weight: 500;
  font-family: inherit;
  cursor: pointer;
  transition: .2s background, .2s color, .2s border-color;
}
.new-thought-btn:hover {
  color: #07090f;
  background: #38bdf8;
  border-color: #38bdf8;
}
</style>
<article>
  <header><h1>Thoughts</h1></header>

  <p class="thoughts-intro">Since 2024, I have been formulating some of my thoughts and reflections about life in one-liners. These can be found here.</p>

  <div class="thought-bubble-wrap">
    <div class="thought-bubble" id="thought-bubble">
      <p class="quote-en" id="quote-en"></p>
      <p class="quote-da" id="quote-da"></p>
    </div>
    <div class="thought-trail" aria-hidden="true">
      <span></span><span></span><span></span>
    </div>
    <button type="button" class="new-thought-btn" id="new-thought-btn">New thought</button>
  </div>
</article>

<script>
(function () {
  var quotes = {{ site.data.quotes | jsonify }};
  var bubble = document.getElementById('thought-bubble');
  var quoteEn = document.getElementById('quote-en');
  var quoteDa = document.getElementById('quote-da');
  var btn = document.getElementById('new-thought-btn');
  var current = -1;

  function pickIndex() {
    if (quotes.length <= 1) return 0;
    var i;
    do { i = Math.floor(Math.random() * quotes.length); } while (i === current);
    return i;
  }

  function showQuote(i) {
    current = i;
    quoteEn.textContent = quotes[i].en;
    quoteDa.textContent = quotes[i].da;
  }

  function newThought() {
    bubble.style.opacity = '0';
    setTimeout(function () {
      showQuote(pickIndex());
      bubble.style.opacity = '1';
    }, 200);
  }

  showQuote(pickIndex());
  btn.addEventListener('click', newThought);
})();
</script>
