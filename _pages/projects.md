---
layout: page
title: projects
permalink: /projects/
description:
nav: true
nav_order: 3
---

## Research

{% assign research_projects = site.projects | where: "category", "research" | sort: "importance" %}
{% for project in research_projects %}
<div class="publications">
<ol class="bibliography">
<li>
<div class="row">
<div class="col-sm-2 abbr">
<abbr class="badge rounded w-100">{{ project.date_range }}</abbr>
</div>
<div class="col-sm-10">
<div class="title"><a href="{{ project.url | relative_url }}">{{ project.title }}</a></div>
<div class="author">{{ project.venue }}</div>
<div class="periodical"><em>{{ project.description }}</em></div>
<div class="links">
{% if project.github %}
<a href="{{ project.github }}" class="btn btn-sm z-depth-0" role="button">code</a>
{% endif %}
{% if project.paper %}
<a href="{{ project.paper }}" class="btn btn-sm z-depth-0" role="button">paper</a>
{% endif %}
{% if project.video %}
<a href="{{ project.video }}" class="btn btn-sm z-depth-0" role="button">video</a>
{% endif %}
</div>
</div>
</div>
</li>
</ol>
</div>
{% endfor %}

## Course & Other Projects

{% assign course_projects = site.projects | where: "category", "course" | sort: "importance" %}
{% for project in course_projects %}
<div class="publications">
<ol class="bibliography">
<li>
<div class="row">
<div class="col-sm-2 abbr">
<abbr class="badge rounded w-100">{{ project.date_range }}</abbr>
</div>
<div class="col-sm-10">
<div class="title"><a href="{{ project.url | relative_url }}">{{ project.title }}</a></div>
<div class="author">{{ project.venue }}</div>
<div class="periodical"><em>{{ project.description }}</em></div>
<div class="links">
{% if project.github %}
<a href="{{ project.github }}" class="btn btn-sm z-depth-0" role="button">code</a>
{% endif %}
</div>
</div>
</div>
</li>
</ol>
</div>
{% endfor %}
