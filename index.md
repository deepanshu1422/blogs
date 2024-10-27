---
layout: home
title: Welcome to Deepanshu's Tech Blog
---

<div class="hero">
  <h1>Welcome to My Tech Journey! 🚀</h1>
  <p>Dive into the world of computer science, innovative projects, and exciting hackathons.</p>
</div>

<section class="featured-posts">
  <h2>Featured Posts</h2>
  <div class="post-grid">
    {% raw %}{% for post in site.posts limit:3 %}
      <article class="post-card">
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        <p class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</p>
        <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
        <a href="{{ post.url | relative_url }}" class="read-more">Read More</a>
      </article>
    {% endfor %}{% endraw %}
  </div>
</section>

<section class="about-section">
  <h2>About Me</h2>
  <p>I'm a passionate computer science enthusiast with a love for building innovative projects and participating in hackathons. Follow my journey as I tackle new challenges, learn cutting-edge technologies, and share insights from the world of tech.</p>
  <a href="/blogs/about/" class="btn">Learn More About Me</a>
</section>

<section class="projects-section">
  <h2>Featured Projects</h2>
  <ul class="project-list">
    <li><strong>Project A:</strong> A brief description of your first featured project.</li>
    <li><strong>Project B:</strong> A brief description of your second featured project.</li>
    <li><strong>Project C:</strong> A brief description of your third featured project.</li>
  </ul>
  <a href="/blogs/projects/" class="btn">View All Projects</a>
</section>

<section class="cta-section">
  <h2>Get in Touch</h2>
  <p>Have a question or want to collaborate? I'd love to hear from you!</p>
  <a href="/blogs/contact/" class="btn">Contact Me</a>
</section>
