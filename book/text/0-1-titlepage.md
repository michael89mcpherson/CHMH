---
title: Title page
type: title-page
---
{% include metadata %}
<img src="{{site.baseurl}}/images/image-cover.jpg" alt="" style="width:750px;height:auto;">
<div class="title-page-title">{{ title }}{% if subtitle %}: {{ subtitle }}{% endif %}</div>
<img src="{{site.baseurl}}/images/image-cover.jpg" alt="" style="width:750px;height:auto;">
<div class="title-page-creators">{% for creator in creators %}{{creator.firstName}} {{creator.lastName}}{% if forloop.last == true %}{% else %}, {% endif %}{% endfor %}</div>

<div class="title-page-bottom-wrapper">
  <div class="title-page-date">{{work.date|date: '%Y'}}</div>
  <div class="title-page-publisher">{{work.publisher.name}}</div>
  <img class="title-page-publisher-logo" src="{{ site.baseurl }}/images/{{work.publisher.logo}}">
</div>
