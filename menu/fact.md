---
layout: page
title: Интересные факты
---
<ul class="posts">
  {% for post in site.categories.fact %}
    <li itemscope>
      <a href="{{ site.github.url }}{{ post.url }}">{{ post.title }}</a><br>
	  {{post.description}}<br><hr>
      <p class="post-date"><span><i class="fa fa-calendar" aria-hidden="true"></i> {{ post.date | date: "%B %-d" }} - <i class="fa fa-clock-o" aria-hidden="true"></i> {% include read-time.html %}</span></p>
    </li>

  {% endfor %}
</ul>
