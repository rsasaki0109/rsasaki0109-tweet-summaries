---
layout: single
title: "年別アーカイブ"
permalink: /yearly/
author_profile: true
toc: true
toc_label: "年別"
header:
  overlay_image: /assets/images/header-bg.png
  overlay_filter: 0.3
---

{% assign all_posts = site.posts %}

## 年別サマリー

| 年 | 投稿数 |
|---|---|
{% assign posts_2026 = all_posts | where_exp: "post", "post.date >= '2026-01-01'" | where_exp: "post", "post.date < '2027-01-01'" %}| [2026年]({{ "/yearly/2026/" | relative_url }}) | {{ posts_2026.size }} 件 |
{% assign posts_2025 = all_posts | where_exp: "post", "post.date >= '2025-01-01'" | where_exp: "post", "post.date < '2026-01-01'" %}| [2025年]({{ "/yearly/2025/" | relative_url }}) | {{ posts_2025.size }} 件 |
{% assign posts_2024 = all_posts | where_exp: "post", "post.date >= '2024-01-01'" | where_exp: "post", "post.date < '2025-01-01'" %}| [2024年]({{ "/yearly/2024/" | relative_url }}) | {{ posts_2024.size }} 件 |
{% assign posts_2023 = all_posts | where_exp: "post", "post.date >= '2023-01-01'" | where_exp: "post", "post.date < '2024-01-01'" %}| [2023年]({{ "/yearly/2023/" | relative_url }}) | {{ posts_2023.size }} 件 |
{% assign posts_2022 = all_posts | where_exp: "post", "post.date >= '2022-01-01'" | where_exp: "post", "post.date < '2023-01-01'" %}| [2022年]({{ "/yearly/2022/" | relative_url }}) | {{ posts_2022.size }} 件 |

---

## 全投稿数

合計: **{{ all_posts.size }}** 件
