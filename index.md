---
layout: page
title: 方浩的新博客
tagline: 作为一个码奴，最好还是有个独立的博客
---
{% include JB/setup %}

我现在在 [北京大学](http://www.pku.edu.cn)

Complete usage and documentation available at: [Jekyll Bootstrap](http://jekyllbootstrap.com)

## 最近干的事情

In `_config.yml` remember to specify your own data:
    
    title : My Blog =)
    
    author :
      name : Name Lastname
      email : blah@email.test
      github : username
      twitter : username

The theme should reference these variables whenever needed.
    
## 之后想干的事情

别急，让我慢慢添么。。。。

    $ rm -rf _posts/core-samples

Here's a sample "posts list".

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

## 我的计划

   再说


