---
title: 2015
layout: default
category: categories
permalink: /categories/ml/
---

<h1 class="page-heading">Category: {{ page.title | upcase}}</h1>

<div class="home">
  <ul class="post-list">
		{% for post in site.posts %}
	    {% if post.tags contains 'ml' %}
				<li onclick="location.href='{{ post.url | prepend: site.baseurl }}'">
          <h2>
            <a class="post-link" >{{ post.title }}</a>
            <a class="post-sublink" >{{ post.sub-title }}</a>
          </h2>
          <hr class="division">

        </li>
			{% endif %}
		{% endfor %}
	</ul>
</div>
