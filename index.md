---
layout: home
title: Welcome to Deepanshu's Tech Blog
---

<section class="all-posts">
  <h2>All Posts</h2>
  <ul class="post-list">
    {% for post in paginator.posts %}
      <li>
        <h3>
          <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
        </h3>
        <span class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</span>
        {% if site.show_excerpts %}
          {{ post.excerpt }}
        {% endif %}
      </li>
    {% endfor %}
  </ul>

  {% if paginator.total_pages > 1 %}
    <div class="pagination">
      {% if paginator.previous_page %}
        <a href="{{ paginator.previous_page_path | relative_url }}" class="btn">Previous</a>
      {% endif %}
      {% if paginator.next_page %}
        <a href="{{ paginator.next_page_path | relative_url }}" class="btn">Next</a>
      {% endif %}
    </div>
  {% endif %}
</section>
