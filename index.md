---
layout: default
title: The People's Guide
---

# Welcome to the People's Guide. We are here for you!

The People’s Guide gives practical information about how to get food, money, housing, health care and other help from government programs and community services if you live in Los Angeles County and need help in hard times. You do not have to read the entire book, just and the topic you need in the table of contents. However, people who are eligible for one kind of help often qualify for other programs as well, so read the entire booklet. *[Read more...](topics/introduction.html)*

- - -

<div class="topics">

	{% assign data_collection = site.collections | where: "label", "topics" | first %}
	{% assign data_list = data_collection.docs | sort: "weight" %}

	{% for data in data_list %}

	<h2><a href="{{ data.url }}">{{ data['title'] }}</a></h2>
	{% if data['description'] %} 
		<p>{{ data['description'] }}</p>
	{% endif %}
	{% endfor %}

<!-- ## [Introduction](topics/introduction.html)

## [Free and Low Cost Food](topics/free-and-low-cost-food.html)
*Food pantries, meals for seniors, community gardens*
 -->
</div>