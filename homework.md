---
layout: default
title: Weekly Readings and Homework
---

<ul>
    {% assign sorted-posts = site.posts | where: "categories","homework" %}
    {% for post in sorted-posts limit: 5 %}
    <li>
        <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
	    <p>{{ post.excerpt }}</p>
    </li>
	{% endfor %}
</ul>
