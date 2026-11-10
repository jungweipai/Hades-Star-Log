---
layout: page
title: 文章 Articles
permalink: /articles/
---

长文、随笔、读书笔记与技术文章会按发布日期倒序显示在这里。

{% for post in site.posts %}
- **{{ post.date | date: '%Y-%m-%d' }}** — [{{ post.title }}]({{ post.url | relative_url }}){% if post.tags.size > 0 %} · `{{ post.tags | join: '`, `' }}`{% endif %}
{% else %}
目前还没有文章。你可以复制 `_templates/article.md` 开始写作。
{% endfor %}
