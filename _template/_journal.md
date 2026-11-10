---
layout: page
title: 日志 Journal
permalink: /journal/
---

这里按时间倒序整理每一篇日志。

{% assign sorted_journal = site.journal | sort: 'date' | reverse %}
{% for entry in sorted_journal %}
- **{{ entry.date | date: '%Y-%m-%d' }}** — [{{ entry.title }}]({{ entry.url | relative_url }}){% if entry.tags.size > 0 %} · `{{ entry.tags | join: '`, `' }}`{% endif %}
{% else %}
目前还没有日志。你可以复制 `_templates/journal.md` 开始记录。
{% endfor %}
