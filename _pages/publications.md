---
layout: page
title: publications
permalink: /publications/
nav: false
banner_image: /assets/img/banner-publications.jpg
---
## Peer-reviewed articles

<div id="journal-articles" class="publications">
{% bibliography -f journal_articles %}
</div>

<div id="pub-toggle-container" style="text-align: center; margin-top: 1rem; margin-bottom: 1rem;">
  <button id="pub-toggle">Show all publications</button>
</div>

## Book chapters

<div class="publications">
{% bibliography -f book_chapters %}
</div>

<style>
.pub-hidden { display: none; }
#pub-toggle {
  border: 1px solid var(--global-divider-color);
  background: none;
  color: var(--global-theme-color);
  cursor: pointer;
  font-size: 0.9rem;
  padding: 0.3rem 1rem;
  border-radius: 4px;
}
#pub-toggle:hover {
  background-color: var(--global-theme-color);
  color: var(--global-hover-text-color);
}
</style>

<script>
document.addEventListener('DOMContentLoaded', function () {
  var SHOW_INITIALLY = 5;
  var container = document.getElementById('journal-articles');
  if (!container) return;
  var list = container.querySelector('ol') || container.querySelector('ul');
  if (!list) return;
  var items = list.querySelectorAll('li');
  if (items.length <= SHOW_INITIALLY) {
    document.getElementById('pub-toggle-container').style.display = 'none';
    return;
  }
  items.forEach(function (item, i) {
    if (i >= SHOW_INITIALLY) item.classList.add('pub-hidden');
  });
  var btn = document.getElementById('pub-toggle');
  var expanded = false;
  btn.addEventListener('click', function () {
    expanded = !expanded;
    items.forEach(function (item, i) {
      if (i >= SHOW_INITIALLY) {
        item.classList.toggle('pub-hidden', !expanded);
      }
    });
    btn.textContent = expanded ? 'Show fewer publications' : 'Show all publications';
  });
});
</script>
