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


<img class="forsidefigur" src="{{ '/assets/figures/faste/HumWolfe.jpg' | relative_url }}" alt="Om Journalistik">


<h2 class="midt">Seneste anmeldelser</h2>

<ul class="anmeldelser">
{% for post in site.posts %}
<li><span class="kar">{{ post.karakter }}</span><span class="tit"><a href="{{ post.url | relative_url }}">{{ post.medie }}: “{{ post.title }}”</a>&nbsp;<span class="sep">|</span> <span class="dat">Anmeldt {{ post.anmeldt | date: "%d.%m.%Y" }}</span></span></li>
{% endfor %}
</ul>
