---
layout: academic
title: "Sitemap"
permalink: /sitemap/
---
<div class="prose">
<h2>Explore</h2>
<ul>{% for link in site.data.navigation.main %}<li><a href="{{ link.url | relative_url }}">{{ link.title }}</a></li>{% endfor %}</ul>
<h2>Projects</h2>
<ul>{% for project in site.portfolio %}<li><a href="{{ project.url | relative_url }}">{{ project.title }}</a></li>{% endfor %}</ul>
<h2>Publications</h2>
<ul>{% assign papers = site.publications | sort: 'date' | reverse %}{% for paper in papers %}<li><a href="{{ paper.url | relative_url }}">{{ paper.title }}</a></li>{% endfor %}</ul>
</div>
