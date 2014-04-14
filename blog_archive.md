---
layout: default
title: Blog archive
---


Blog archive
========================================

<div id="posts">

{% for post in site.posts offset: 0 %}
    <div style="border-bottom: 1px solid gray; padding: 5px 0;">
    <small style="color: #999;">{{ post.date | date: "%b %d, %Y" }}</small> 
    <a href="{{ post.url }}">{{ post.title }}</a>
    </br>{{ post.excerpt }}
    <br />
    {% if post.summary %}
        <small>{{ post.summary }}</small>
    {% endif %}
    </div>
{% endfor %}

</div>
