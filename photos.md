---
layout: default
---
<div class="posts">
<h3> Photos </h3>
<div class="posts">
<br />
{% for item in site.data.photos %}
<figure>
	<img src="{{ site.baseurl }}/images/group_photos/{{ item.file }}" alt="{{ item.year }} {{ item.caption }}">
	<figcaption> {{ item.year }} {{ item.caption }} </figcaption>
</figure>
<br />
{% endfor %}
<br />
</div>
</div>
