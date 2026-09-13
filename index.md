---
layout: default
title: Forside
---

<h1 class="sitetitel">Om Journalistik</h1>

<p class="undertitel">– anmeldelser af journalistik –</p>

![HumWolfe]({{ '/assets/figures/faste/HumWolfe.jpg' | relative_url }})

## Seneste anmeldelser

{% for post in site.posts %}
- **[{{ post.karakter }}]** [{{ post.medie }}: “{{ post.title }}”]({{ post.url | relative_url }}) — Anmeldt {{ post.anmeldt | date: "%d.%m.%Y" }}
{% endfor %}
