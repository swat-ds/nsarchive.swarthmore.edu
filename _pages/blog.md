---
layout: page
title: Blog
---
<div class="disclaimer">
  <p><em>All posts reflect the opinions of the author, not The National Security Archive or Swarthmore College.</em></p>
</div>
<div class="posts">
  {% for post in site.posts %}
  <div class="post">
    <h1 class="post-title">
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h1>
    <h3>by {{post.authors}}</h3>
    <span class="post-date">{{ post.date | date_to_string }}</span>
    {{ post.content }}
  </div>
  {% endfor %}
</div>
