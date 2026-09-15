---
layout: default
title: Forside
---

<h1 class="sitetitel">Om Journalistik</h1>

<p class="undertitel">– anmeldelser af journalistik –</p>

<img id="banner"
     class="banner-march"
     src="{{ '/assets/figures/faste/banner_stick_march_loop.gif' | relative_url }}"
     alt="Journalist iagttager en samlet gruppe">


## Seneste anmeldelser

{% for post in site.posts %}
- **[{{ post.karakter }}]** [{{ post.medie }}: “{{ post.title }}”]({{ post.url | relative_url }}) — Anmeldt {{ post.anmeldt | date: "%d.%m.%Y" }}
{% endfor %}

<img class="forsidefigur" src="{{ '/assets/figures/faste/HumWolfe.jpg' | relative_url }}" alt="Om Journalistik">
