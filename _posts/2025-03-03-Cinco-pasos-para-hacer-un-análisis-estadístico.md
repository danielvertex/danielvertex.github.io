---
layout: post
title: Cinco pasos para hacer un análisis estadístico.
date: 2025-03-03 16:40:16
description: march & april, looking forward to summer
tags: formatting links
categories: sample-posts
giscus_comments: false
related_posts: false
---

{::nomarkdown}
{% assign jupyter_path = "assets/jupyter/estadistico.ipynb" | relative_url %}
{% capture notebook_exists %}{% file_exists assets/jupyter/estadistico.ipynb %}{% endcapture %}
{% if notebook_exists == "true" %}
{% jupyter_notebook jupyter_path %}
{% else %}

<p>Sorry, the notebook you are looking for does not exist.</p>
{% endif %}
{:/nomarkdown}
