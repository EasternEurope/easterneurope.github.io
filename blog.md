---
layout: default
title: Blog
---

Blog posts
========================================

<div class="posts">
    {% for post in site.posts %}
    {% assign author = site.authors[post.author] %}
    <div class="meta">
            <small style="color: #999;">{{ post.date | date: "%b %d, %Y" }}</small> 
            <a class="title" href="{{ post.url }}">{{ post.title }}</a>
            by <strong>{{ author.display_name }}</strong>
        </div>
        {{ post.excerpt }}
    {% endfor %}
</div>



<div style="margin: 15px 0; padding-top: 5px;">
<small>
    <a href="/blog_archive.html" title="an archive of all posts">&larr; More posts</a>
</small>
</div>

Blog RSS here: <a title="blog RSS" href="http://easterneurope.github.io/feed.xml">
                    <i class="fa fa-rss-square"></i></a>

