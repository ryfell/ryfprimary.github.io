---
layout: default
---

<div class="posts">
  {% for post in site.tags.news limit:5 %}
  <div class="post">
    <h1>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h1>

    <span class="post-date">{{ post.date | date_to_string }}</span>

    {{ post.content }}
    {% include letusknow.html %}
  </div>
  {% endfor %}
</div>
