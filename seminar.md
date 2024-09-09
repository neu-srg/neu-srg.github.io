---
layout: default
---
<div class="posts">
<h3> Internal Paper Reading Group Meetings </h3>
<div class="post">
<br />
<div class="titles">
Current [<b>
<a href="https://naizhengtan.notion.site/SIGPAPER-FA-2024-9bd146ecf75047788e26fce58367453a">2024FA</a>
</b>]
</div>
<br/>
<div class="titles">
Past [
<a href="https://naizhengtan.notion.site/SIGPAPER-SP-2024-fffa52714baf48778c31b9754e3ca796">2024SP</a> |
<a href="https://naizhengtan.notion.site/SIGPAPER-FA-2023-1e8896455cf74b39ba14271a38726a37">2023FA</a> |
<a href="https://naizhengtan.notion.site/SIGPAPER-SP-2023-b1a87e4eb20e49e795aaa345b98820c8">2023SP</a> |
<a href="https://naizhengtan.notion.site/SIGPAPER-FA-2022-029b420e270348069d04865c086974ed">2022FA</a> 
]
</div>
<br />
</div>
</div>

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
