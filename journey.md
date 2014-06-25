---
layout: page
title: Journey
permalink: /journey/
---

<svg xmlns="http://www.w3.org/2000/svg" width="100%" height="360" viewBox="0 0 201 97">
{% include map.svg %}
{% for project in site.data.projects%}
{{ project.point_html }}
{% endfor %}	 
</svg>

<ul class="posts">
{% for post in site.posts %}
<li>
    <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
    <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
</li>
{% endfor %}
    
</ul>

<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>