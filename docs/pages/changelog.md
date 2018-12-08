---
title: Changelog
permalink: /about/changelog
description: We've built an amazing team of developers, marketers, designers and sales people.
---
<ul class="staff">
	{% for person in site.team %}
		<li>
			<div class="square-image"><img src="{% include relative-src.html src=person.image_path %}" alt="{{ person.name }}"/></div>
			<div class="name"><a target="_blank" href="https://twitter.com/{{ person.twitter }}">{{ person.name }}</a></div>
			<div class="position">{{ person.position }}</div>
		</li>
	{% endfor %}
</ul>
