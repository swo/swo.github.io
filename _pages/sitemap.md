---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

A list of all the posts and pages found on the site.

<h2>Pages</h2>
<ul>
{% for post in site.pages %}
  {% if post.title and post.url %}
  <li><a href="{{ base_path }}{{ post.url }}">{{ post.title }}</a></li>
  {% endif %}
{% endfor %}
</ul>

<h2>Posts</h2>
<ul>
{% for post in site.posts %}
  <li><a href="{{ base_path }}{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
