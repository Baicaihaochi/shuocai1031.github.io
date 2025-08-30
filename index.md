---
layout: home
title: Shuo Cai
author_profile: true
classes: wide
---

## 🔥 News
{% raw %}{% for post in site.posts limit:6 %}
- {{ post.date | date: "%Y.%m.%d" }} — {{ post.title }}{% if post.link %} ([link]({{ post.link }})){% endif %}
{% endfor %}{% endraw %}

## 📚 Selected Publications
{% raw %}{% for pub in site.publications limit:3 %}
- **{{ pub.title }}** ({{ pub.venue }} {{ pub.year }})  
  {{ pub.authors }}.{% if pub.paperurl %} [PDF]({{ pub.paperurl }}){% endif %}{% if pub.code %} · [Code]({{ pub.code }}){% endif %}
{% endfor %}{% endraw %}
