---
layout: page
title: Projects
---
<p class="message">
	Hey there! This is my Projects page. I will be updating it with any programming projects I am working on or have finished.
</p>


<div class="posts">
    {% for post in site.projects %}
    <div class="post">
        <a href="{{ post.url | prepend: site.baseurl }}">
          <h1 class="post-title">
            {{ post.title }}
          </h1>
        </a>

    <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>

      {{ post.content }}
    </div>
    {% endfor %}
</div>

