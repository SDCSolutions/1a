---
layout: default
title: Blog Tags
image: john-carlisle-539580.jpg
imagecredit: Photo by John Carlisle on Unsplash
header1: Blog Tags
---
{% for tag in site.tags %}
{% assign t = tag | first %}
{% assign posts = tag | last %}

<h2>{{ t | downcase }}</h2>

<ul>
{% for post in posts %}
  {% if post.tags contains t %}
  <li>
        <a href="{{ post.url | absolute_url}}">{{ post.title }}</a>
        &nbsp; 
        <span>{{ post.date | date: "%B %-d, %Y"  }}
        </span>
        
  </li>
  {% endif %}
{% endfor %}
</ul>

<hr>

{% endfor %}