---
layout: single
title: ""
excerpt: "Homepage"
author_profile: true
permalink: /
twitter: true
---

I am a computational biophysicist at the University of California San Diego, pursuing my PhD in engineering physics with 4+ years of experience in managing projects, leading research teams and scientific communication. I am currently seeking opportunities to leverage technology, research, and/or management skills to
innovate product development.

I leverage interdisciplinary skills including computational biophysics, numerical analysis, algorithm development, applied mathematics, data science and high performance computing to address large scale complex biological problems.

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

