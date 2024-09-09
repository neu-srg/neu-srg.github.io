---
layout: default
---
<div class="posts">
<h3> Internal Paper Reading Group Meetings </h3>
<article class="post">
<br />
{% for item in site.data.readinggroups %}
  <div class="titles">
{% if forloop.index == 1 %}
  <b>
  <a href="{{ item.url }}" target="_blank">{{ item.year-semester }}: {{ item.topic }}</a>

  </b>
{% else %}
  <a href="{{ item.url }}" target="_blank">{{ item.year-semester }}: {{ item.topic }}</a>
{% endif %}
  </div>
{% endfor %}
</article>
</div>
<p><p/>


<h3> Seminars with External Speakers</h3>
<div class="posts">
<br />
  {% assign sorted = site.seminars | sort: 'date' | reverse %}
  {% for post in sorted %}
    <article class="post">
      <div class="titles">
	<br/>
        <b>
	Time: {{ post.date | date: "%b %d (%a), %Y"}}
	@ {{ post.time }},
        Location: {{ post.location }}
        {% if post.location %} {% if post.online %} and {% endif %}{% endif %}
        {% if post.online %} online {% endif %}
        </b>
        <br/>
	{{ post.speaker }} ({{ post.affiliation }}),
	"{{ post.talk-title }}"
      </div>
      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Abstract and bio</a>
    </article>
  {% endfor %}
</div>
