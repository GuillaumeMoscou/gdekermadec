---
layout: default
title: Accueil
---

<div class="hero">
  <img src="{{ '/assets/img/profile.jpg' | relative_url }}" alt="Photo – Guillaume Huon de Kermadec" />
  <div>
    <h1>{{ site.author.name }}</h1>
    <p>Trader / Risk management · Produits dérivés · Données & process · FR / RU / EN</p>
    <p>
      <a class="btn" href="{{ '/cv/' | relative_url }}">Voir mon CV</a>
      · <a href="{{ site.author.socials.linkedin }}" target="_blank">LinkedIn</a>
      · <a href="{{ site.author.socials.github }}" target="_blank">GitHub</a>
    </p>
  </div>
</div>

### Derniers articles

<ul>
{% assign posts = site.posts | slice: 0, 5 %}
{% for post in posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span class="meta"> – {{ post.date | date: '%d %b %Y' }}</span>
  </li>
{% endfor %}
</ul>

<div class="cards">
  <div class="card">
    <h3>CV</h3>
    <p>Mon expérience et mes réalisations en 3 langues.</p>
    <p><a href="{{ '/cv/' | relative_url }}">Accéder au CV →</a></p>
  </div>
  <div class="card">
    <h3>Articles</h3>
    <p>Notes de marché, risk management, outils.</p>
    <p><a href="{{ '/blog/' | relative_url }}">Tous les articles →</a></p>
  </div>
</div>
