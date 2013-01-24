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
      寒假计划
    </h2>
    <ul>
      <li><a href="http://blog.renren.com/blog/472085551/893264809" target="_blank">github相关</a></li>
      <li><a href="http://nodejs.org/">Node.js</a></li>
    </ul>
    </aside>
  </div>
    <div class="doing_list">
    <aside>
    <h2>
      寒假要看的书
    </h2>
    <ul>
      <li>
        <a href="http://book.douban.com/subject/4941558/" target="_blank">Crack the Code Interview</a>
      </li>
      <li>
        <a href="http://book.douban.com/subject/10430397/" target="_blank">艺术通史</a>
      </li>
    </ul>
    </aside>
  </div>
    
  <div class="friendlink">
    <p><strong>乡亲们的链接</strong></p>
    <ul>
    <li>
        <a href="http://oilbeater.com" target="_blank">Oilbeater</a>
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
