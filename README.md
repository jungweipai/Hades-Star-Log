# 我的长期日志与文章

这是一个用 **GitHub + Markdown** 管理的长期写作仓库，也可以通过 **GitHub Pages** 发布成个人网站。

> 用简洁的格式，持续记录学习、生活、研究、阅读和思考。

## 导航

- [网站首页](index.md)
- [日志列表（网站）](journal.md)
- [文章列表（网站）](articles.md)
- [关于](about.md)
- [完整使用流程](HOW_TO_WRITE.md)
- [日志模板](_templates/journal.md)
- [文章模板](_templates/article.md)

## 两种内容

| 类型 | 放在哪里 | 适合什么 |
| --- | --- | --- |
| 日志 Journal | `_journal/YYYY/YYYY-MM-DD-topic.md` | 每日/每周总结、学习进展、灵感和反思 |
| 文章 Article | `_posts/YYYY-MM-DD-topic.md` | 观点、随笔、技术文章、读书笔记、长文 |

**写日志：** 复制 `_templates/journal.md` 到 `_journal/年份/日期-主题.md`，修改标题、日期，填写正文。

**写文章：** 复制 `_templates/article.md` 到 `_posts/日期-标题.md`，修改标题、日期、标签，填写正文。

文件名建议全用英文小写和连字符，正文完全可以使用中文。

## 快速发布网站

1. 在 GitHub 创建一个新的 **Public** repository（如 `writing-archive`）。
2. 上传本文件夹中的全部内容到仓库根目录（不是再嵌套一层 `github-writing-archive` 文件夹）。
3. 打开仓库的 **Settings → Pages**。
4. 在 **Build and deployment** 中，将 **Source** 设为 **Deploy from a branch**。
5. 选择分支 **main** 和文件夹 **/(root)**，保存。
6. 等 GitHub 完成第一次部署后，在 Pages 设置页点击 **Visit site**，即可查看自己的文章和日志网站。

通常地址是 `https://你的用户名.github.io/仓库名称/`。如果仓库命名为 `你的用户名.github.io`，则通常是 `https://你的用户名.github.io/`。

> 注意：GitHub Pages 发布的站点对互联网公开。请勿上传日记中的隐私、口令、住址、API keys 等敏感内容。

## 长期写作建议

- **日常随手记：** 宁可写 5 行，也不必逼自己每天写 1000 字。
- **周度复盘：** 每周总结一次完成了什么、遇到哪些问题、下周做什么。
- **长期文章：** 用几篇日志中的线索，整理为结构完整的文章。
- **保留修改记录：** 用 Git commit 记录每一次修改和更新。

需要进一步的发布或 Git 操作说明，请看 [HOW_TO_WRITE.md](HOW_TO_WRITE.md)。
