---
layout: page
title: Blog
permalink: /blog/

---
<div class="blog">

  <h1 class="page-heading">Blog Posts</h1>

  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title | escape }}</a>
        </h2>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
      </li>
    {% endfor %}
  </ul>

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

</div>
