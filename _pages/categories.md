---
layout: single
title: "カテゴリ別アーカイブ"
permalink: /categories/
author_profile: true
header:
  overlay_image: /assets/images/header-bg.png
  overlay_filter: 0.3
---

{% assign cats = "3D再構成・SLAM,自動運転,ロボティクス,VLA・Foundation Model,論文紹介,OSS・ツール,その他" | split: "," %}

{% for cat in cats %}
## {{ cat }}

{% for post in site.posts %}
{% if post.categories contains "monthly-summary" %}
{% if post.content contains cat %}
- [{{ post.title }}]({{ post.url | relative_url }})
{% endif %}
{% endif %}
{% endfor %}

{% endfor %}
