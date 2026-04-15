---
layout: default
---

<div class="home">
  <h2>Welcome</h2>
  <p>Hi, I'm <strong>weiwei</strong>. This is my personal blog where I share thoughts, experiences, and things I've learned.</p>

  <h3>Recent Posts</h3>
  <ul>
    {% for post in site.posts limit: 5 %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <span class="post-date">— {{ post.date | date: "%b %d, %Y" }}</span>
    </li>
    {% endfor %}
  </ul>

  <p class="more-link"><a href="{{ '/posts/' | relative_url }}">View all posts →</a></p>
</div>
