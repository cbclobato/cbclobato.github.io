---
layout: home
title: Research
order: 5
---

<br>
  <!-- <h1 class="pageTitle">Research</h1> -->
  <!-- <h1>Research</h1> -->
  
<div id="articles">

  <ul class="posts noList">
    {% for post in site.posts %}
      <li>
      	<!-- <span class="date">{{ post.date | date_to_string }}</span> -->
      	<h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      	<p class="description">{% if post.description %}{{ post.description  | strip_html | strip_newlines | truncate: 120 }}{% else %}{{ post.content | strip_html | strip_newlines | truncate: 120 }}{% endif %}</p>
      </li>
    {% endfor %}
  </ul>
</div>
