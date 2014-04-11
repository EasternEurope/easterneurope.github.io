---
layout: default
title: Main
---



![](/images/logo200.png)


Nam suscipit vulputate quam. Integer feugiat massa at nisi bibendum, a tincidunt nisl sollicitudin. Etiam massa eros, interdum at dignissim nec, accumsan vel purus. In odio augue, scelerisque non ultricies in, sollicitudin eget sapien. Duis dictum pharetra augue a ultrices. Aliquam non mattis metus, ornare congue erat. Nulla est tortor, pretium eu dui vitae, dignissim rhoncus nulla. Suspendisse pharetra sed erat porttitor molestie.

----

Latest in the blog
-------------------------------

Blog RSS here: <a title="blog RSS" href="http://easterneurope.github.io/feed.xml">
                    <i class="fa fa-rss-square"></i></a>

<div id="posts">
    {% for post in site.posts offset: 0 limit: 3 %}
        <small style="color: #999;">{{ post.date | date: "%b %d, %Y" }}</small> 
        <a href="{{ post.url }}">{{ post.title }}</a>
        <br />
        {% if post.summary %}
            <small>{{ post.summary }}</small>
        {% endif %}
    {% endfor %}
    </div>
