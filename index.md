---
layout: default
title: Welcome to My Blog
---

# Welcome to My Blog! 🚀

Here you'll find all my latest thoughts, projects, and adventures in the world of computer science and technology.

## Latest Posts

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ site.baseurl }}{{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

## About Me

I'm a computer science enthusiast who loves building projects and attending hackathons. Follow my journey as I explore new technologies and share my experiences!

## Get in Touch

Feel free to reach out to me on [GitHub](https://github.com/deepanshu1422) or connect with me on other platforms (you can add links to your social media profiles here).

Happy reading!
