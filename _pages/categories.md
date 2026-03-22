---
layout: single
title: "カテゴリ別アーカイブ"
permalink: /categories/
author_profile: true
toc: true
toc_label: "カテゴリ"
header:
  overlay_image: /assets/images/header-bg.png
  overlay_filter: 0.3
---

{% assign all_posts = site.posts | where: "categories", "monthly-summary" %}

## 🏗️ 3D再構成・SLAM

Gaussian Splatting, NeRF, SLAM, Visual Odometry, Point Cloud など

{% for post in all_posts %}
{% if post.content contains "3D再構成・SLAM" %}
- **[{{ post.title }}]({{ post.url | relative_url }})** <small>{{ post.date | date: "%Y/%m/%d" }}</small>
{% endif %}
{% endfor %}

---

## 🚗 自動運転

Autoware, LiDAR, Perception, Planning, BEV など

{% for post in all_posts %}
{% if post.content contains "自動運転" %}
- **[{{ post.title }}]({{ post.url | relative_url }})** <small>{{ post.date | date: "%Y/%m/%d" }}</small>
{% endif %}
{% endfor %}

---

## 🤖 ロボティクス

ROS 2, Manipulation, Drone, Legged Robot など

{% for post in all_posts %}
{% if post.content contains "ロボティクス" %}
- **[{{ post.title }}]({{ post.url | relative_url }})** <small>{{ post.date | date: "%Y/%m/%d" }}</small>
{% endif %}
{% endfor %}

---

## 🧠 VLA・Foundation Model

Vision-Language-Action, LLM, Embodied AI など

{% for post in all_posts %}
{% if post.content contains "VLA・Foundation Model" %}
- **[{{ post.title }}]({{ post.url | relative_url }})** <small>{{ post.date | date: "%Y/%m/%d" }}</small>
{% endif %}
{% endfor %}

---

## 📄 論文紹介

ICRA, CVPR, NeurIPS, CoRL, RA-L など

{% for post in all_posts %}
{% if post.content contains "論文紹介" %}
- **[{{ post.title }}]({{ post.url | relative_url }})** <small>{{ post.date | date: "%Y/%m/%d" }}</small>
{% endif %}
{% endfor %}

---

## 🔧 OSS・ツール

GitHub公開プロジェクト、ライブラリ など

{% for post in all_posts %}
{% if post.content contains "OSS・ツール" %}
- **[{{ post.title }}]({{ post.url | relative_url }})** <small>{{ post.date | date: "%Y/%m/%d" }}</small>
{% endif %}
{% endfor %}
