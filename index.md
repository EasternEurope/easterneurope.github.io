---
layout: default
title: Main
---

</br>

![](/images/logo200shadow.png)

----

Latest in the blog
-------------------------------

RSS here: <a title="blog RSS" href="http://easterneurope.github.io/feed.xml">
                    <i class="fa fa-rss-square"></i></a>


<div class="posts">
    {% for post in site.posts offset: 0 limit: 3 %}
    {% assign author = site.authors[post.author] %}
    <div class="meta">
            <small style="color: #999;">{{ post.date | date: "%b %d, %Y" }}</small> 
            <a class="title" href="{{ post.url }}">{{ post.title }}</a>
            by <strong>{{ author.display_name }}</strong>
        </div>
        {{ post.excerpt }}
    {% endfor %}
</div>
