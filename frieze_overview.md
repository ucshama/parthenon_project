---
title: Frieze Overview
layout: page
menuItem: Frieze Overview
menuPosition: 3
---
The Parthenon Frieze depicts a religious procession that takes place during the [Panathenaic](https://en.wikipedia.org/wiki/Panathenaea) which was one the most important festivals in ancient Athens. It is made of [Pentelic](https://en.wikipedia.org/wiki/Mount_Pentelicus#Pentelic_marble) Marble from Mount Pentelicus which is white with a uniform, slight yellow tint. During the [Morean](https://en.wikipedia.org/wiki/Parthenon#Destruction) War, Greece was under Ottoman rule and used the Parthenon as storage for gunpowder. A Venetian mortar round later blew up the gunpowder store and damaged the frieze, particularly the South Frieze.

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
