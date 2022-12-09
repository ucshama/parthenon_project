---
title: Frieze Overview
layout: page
menuItem: Frieze Overview
menuPosition: 3
---

<ol>
{% assign syllabus = (site.syllabus | sort: "class") %}
{% for class in syllabus %}
  <li>
  	<a href="{{ site.baseurl }}{{ class.url }}">{{ class.title }}</a> 
  	{% for tag in class.tags %}
  		<b>#{{ tag }}</b>
  	{% endfor %}
  	({{ class.day }})</li>
{% endfor %}
</ol>
