---
title: "Projecten"
lead: "Hier zijn we mee bezig. Zelf een goed idee? Zoek dan zeker contact!"
layout: page
order: 3.5
header: "/assets/img/content/research_page_header.jpg"
---

{% for project in site.projects %}
## [{{ project.title }} &raquo;]({{ project.url | relative_url }})
{{ project.lead }}
{% endfor %}
