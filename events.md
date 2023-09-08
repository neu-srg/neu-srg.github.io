---
layout: default
---
<h3> Events </h3>
<div class="event-table">
  {% for event in site.data.events %}
  <div class=event>
      <b>{{ event.title }}</b>
      <a href="{{ event.url }}">[event page]</a>
  </div>
{% endfor %}
</div>
