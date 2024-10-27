---
layout: home
title: Welcome to My Tech Journey
---

# Welcome to My Tech Journey! 🚀

Dive into the world of computer science, innovative projects, and exciting hackathons. Join me as I explore cutting-edge technologies and share my experiences in the ever-evolving tech landscape.

## Latest Posts

{% raw %}
{% for post in site.posts limit:3 %}
  <article class="post-preview">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</p>
    <p>{{ post.excerpt | strip_html | truncatewords: 50 }}</p>
    <a href="{{ post.url | relative_url }}" class="read-more">Read More</a>
  </article>
{% endfor %}
{% endraw %}

## About Me

I'm a passionate computer science enthusiast with a love for building innovative projects and participating in hackathons. Follow my journey as I tackle new challenges, learn cutting-edge technologies, and share insights from the world of tech.

[Learn more about me](/blogs/about/)

## Featured Projects

- **Project A**: A brief description of your first featured project.
- **Project B**: A brief description of your second featured project.
- **Project C**: A brief description of your third featured project.

[View all projects](/blogs/projects/)

## Get in Touch

Have a question or want to collaborate? I'd love to hear from you!

[Contact me](/blogs/contact/)
