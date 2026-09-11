---
layout: default
title: Forside
---

# Om Journalistik

<p class="undertitel">– anmeldelser af journalistik –</p>

## Seneste anmeldelser

{% for post in site.posts %}
- **[{{ post.karakter }}]** [{{ post.medie }}: “{{ post.title }}”]({{ post.url | relative_url }}) — Anmeldt {{ post.anmeldt | date: "%d.%m.%Y" }}
{% endfor %}
