---
layout: page
title: FangHow 的部落格
tagline: Stay hungry, Stay foolish
---
{% include JB/setup %}
<head>
  <link rel="stylesheet" href="/css/main.css" type="text/css" />
</head>
<body>
  <div class="sidebar">
    <div class="to_be_continue">
    <h2>即将推出</h2>
    <ul>
      <li>
        筹划之中
      </li>
    </ul>
  </div>
  <div class="to_do_list">
    <aside>
    <h2>
      最近的主要工作
    </h2>
    <ul>
      <li><a href="https://github.com/oilbeater/ACT" target="_blank">领域工程</a></li>
      <li><a href="http://pdos.csail.mit.edu/6.828/2011/">设计</a></li>
    </ul>
    </aside>
  </div>
    <div class="doing_list">
    <aside>
    <h2>
      想做的事情
    </h2>
    <ul>
      <li>
        <a href="http://book.douban.com/subject/2287506/" target="_blank">看书</a>
      </li>
    </ul>
    </aside>
  </div>
      <div class="done_list">
    <aside>
    <h2>
      做过的工作
    </h2>
    <ul>
      <li><a href="http://www.fanghow.com" target="_blank">再说</a></li>
    </ul>
    </aside>
  </div>
  <div class="friendlink">
    <p><strong>乡亲们的链接</strong></p>
    <ul>
     <li>
        <a href="http://oilbeater.com/" target="_blank">Oilbeater's Blog</a>
      </li>
      <li>
        <a href="http://itester.me" target="_blank">iTester</a>
      </li>
      <li>
        <a href="http://pinderpeng.org" target="_blank">Pinder's Blog</a>
      </li>
    </ul>
  </div>
  </div>
{% for post in site.posts %}
    {% if post.img != "secret" %}
      <div class="main">
        <ul>
          <li>
          <a href="{{ post.url }}">
            <img src="{{ post.img }}" alt="{{ post.title }}">
          </a>
          <div class="posts">
            <h3>
              <a href="{{ post.url }}">{{ post.title }}</a>
            </h3>
            <p>
              {{ post.date | date: "%B %e, %Y" }}
                &nbsp &nbsptag:
                {% for tag in post.tags %}
                 <a href="/tags.html#{{tag}}-ref">{{ tag }}</a>
                {% endfor %}
            </p>
            <span class="description">{{ post.description }}</span>
          </div>
          </li>
        </ul>
      </div>
    {% endif %}
  {% endfor %}
</body>
