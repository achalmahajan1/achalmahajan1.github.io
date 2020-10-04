---
layout: single
title: ""
excerpt: "Homepage"
author_profile: true
permalink: /
twitter: true
---

I am a doctoral student at the Department of Mechanical and Aerospace Engineering at University of California San Diego (UCSD).

Prior to coming to UCSD, I have obtained an M.S.(Engg). degree from Jawaharlal Nehru Centre for Advanced Scientific Research (Bangalore, India) and a B.Tech. degree in Chemical Engineering from National Institute of Technology Karnataka Surathkal.

<h1>Latest Posts</h1>
{% assign sorted = site.posts | sort:'date' | reverse %}
<ul>
{% for post in sorted limit:3%}
	<div class="{{ include.type | default: "list" }}__item">
	  <article class="archive__item" itemscope itemtype="http://schema.org/CreativeWork">
	    <li>
	      <h3 class="archive__item-title" itemprop="headline">
			 	  <a href="{{ root_url }}{{ post.url }}">{{ post.title }}</a>
	      </h3>
        <p class="archive__item-excerpt" itemprop="description">{{post.excerpt}}</p>
	    </li>
	 </article>
	</div>
{% endfor %}
<ul>
<a href="/blog/" class="back-to-top">More posts &rarr;</a>
