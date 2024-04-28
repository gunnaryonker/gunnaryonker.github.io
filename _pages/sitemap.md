---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

A list of all the posts and pages found on the site.

{% for post in site.pages %}
  {% unless post.title == "publications" or post.title == "talks" or post.title == "teaching" or post.title == "Jupyter notebook markdown generator" or post.title == "Education" %}
    {% include archive-single.html %}
  {% endunless %}
{% endfor %}

{% for post in site.posts %}
  {% unless post.title == "portfolio" %}
    {% include archive-single.html %}
  {% endunless %}
{% endfor %}
