---
layout: page
title: Blog
---
<div class="posts">
  {% for post in site.posts %}
  <div class="post">
    <h1 class="post-title">
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h1>
    <p><em>All posts reflect the opinions of the author, not The National Security Archive or Swarthmore College.</em></p>
    <span class="post-date">{{ post.date | date_to_string }}</span>

    {{ post.content }}
  </div>
  {% endfor %}
</div>
