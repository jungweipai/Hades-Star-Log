---
layout: page
title: 首页
permalink: /
---

# 我的长期日志与文章

欢迎来到我的长期写作空间。这里收集每日/每周日志，以及持续修改、逐步成熟的文章。

[浏览全部日志]({{ '/journal/' | relative_url }}) · [浏览全部文章]({{ '/articles/' | relative_url }}) · [关于我]({{ '/about/' | relative_url }})

## 最新日志

{% assign recent_journal = site.journal | sort: 'date' | reverse %}
{% for entry in recent_journal limit: 5 %}
- **{{ entry.date | date: '%Y-%m-%d' }}** — [{{ entry.title }}]({{ entry.url | relative_url }})
{% else %}
暂时没有日志。
{% endfor %}

## 最新文章

{% for post in site.posts limit: 5 %}
- **{{ post.date | date: '%Y-%m-%d' }}** — [{{ post.title }}]({{ post.url | relative_url }})
{% else %}
暂时没有文章。
{% endfor %}
