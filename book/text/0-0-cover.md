---
title: Cover
type: cover
---
{% include metadata %}
<img src="{{site.baseurl}}/images/image-cover.jpg" alt="" style="width:750px;height:auto;">
<div class="cover-header">
	<div class="cover-creators">{% for creator in creators %}{{creator.firstName}} {{creator.lastName}}{% if forloop.last == true %}{% else %}, {% endif %}{% endfor %}</div>
	<div class="cover-book-title">{{title}}</div>
	<div class="cover-book-subtitle">{{subtitle}}</div>
</div>
<div class="cover-image-container"><img class="cover-image" src="{{ site.baseurl }}/images/image-cover.jpg}}" alt="Book image cover"></div>
<div class="cover-meta">
	<div class="cover-date">{{work.date|date: '%Y'}}</div>
	<div class="cover-publisher">{{work.publisher.name}}</div>
	<div class="cover-version">{{work.status}} – {{ work.version}}</div>
</div>
