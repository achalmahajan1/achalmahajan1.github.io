---
layout: single
title: ""
excerpt: "Homepage"
author_profile: true
permalink: /
twitter: false
---

I am a senior application engineer at <a href="https://www.mathworks.com/">MathWorks</a> in the computational biology group focussed on Simbiology and bioinformatics. I am mostly interested in the intersection of biology, computation, modeling (statistical and first principle) and artifical intelligence. Before pivoting to industry, I had obtained a PhD at the University of California San Diego under the supervision of <a href="http://stokeslet.ucsd.edu/index.html">Prof. David Saintillan</a> in computational biophysics to understand how genome organizes insid the cell. 

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

