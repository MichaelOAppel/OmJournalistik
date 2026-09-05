---
layout: default
title: Forside
---

# Om Journalistik

– anmeldelser af journalistik –

## Seneste anmeldelser

{% for post in site.posts %}
- **[{{ post.karakter }}]** [{{ post.medie }}: “{{ post.title }}”]({{ post.url | relative_url }})
  Anmeldt {{ post.anmeldt }}
{% endfor %}
