---
layout: default
title: Tag
image: john-carlisle-539580.jpg
imagecredit: Photo by John Carlisle on Unsplash
header1: Blog Tags
tags:
---
 
 <h3>Tags</h3>

{% for tag in site.tags %}
  {% assign t = tag | first %}
  {% assign posts = tag | last %}
{{site.tags}}
<h2>{{ t | downcase }}</h2>

<ul>
{% for post in posts %}
  {% if post.tags contains t %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    &nbsp;
    <span class="date">{{ post.date | date: "%B %-d, %Y"  }}</span>
  </li>
  {% endif %}
{% endfor %}
</ul>

<hr>

{% endfor %}