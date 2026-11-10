# 日常写作流程 / Procedure

## A. 直接用 GitHub 网页端（不需要安装 Git）

**新日志：**

1. 找到 `_templates/journal.md`，复制其内容。
2. 在仓库点击 **Add file → Create new file**。
3. 文件名输入 `_journal/2026/2026-11-09-my-day.md`（改成当天日期与主题）。
4. 粘贴模板，修改 `title`、`date`、`tags` 和正文。
5. 点击 **Commit changes**，提交信息如 `journal: 2026-11-09`。

**新文章：**

1. 复制 `_templates/article.md` 的内容。
2. 新建 `_posts/2026-11-09-topic-title.md`。**Jekyll 文章必须采用 `YYYY-MM-DD-标题.md` 命名**。
3. 修改 YAML 信息与正文，提交如 `article: add topic title`。
4. 网站的日志/文章列表会自动更新，不需要手动修改首页目录。

> `date` 应与实际发表日期一致。`tags` 可以用英文短词，正文可以全部使用中文。

## B. 本地用 Git 更新（适合长期写作）

首次克隆（替换账户名和仓库名）：

```bash
git clone https://github.com/USERNAME/REPOSITORY.git
cd REPOSITORY
```

每次写作前同步（如果只有你一个人编辑，且没有未提交改动）：

```bash
git pull --ff-only
```

编辑后保存并发布：

```bash
git add .
git commit -m "journal: add 2026-11-09 entry"
git push
```

发布文章可以用：`git commit -m "article: add a new essay"`。

## C. 可持续维护的节奏

| 频率 | 做什么 | 所需时间（建议） |
|---|---|---|
| 每天或有感而发 | 记录 3–5 行日志 | 5–10 分钟 |
| 每周 | 回顾上周记录，填写下一周目标 | 15–20 分钟 |
| 每月 | 从日志整理一篇更完整的文章 | 视主题而定 |
| 每季度 | 更新 about 页，修订重要文章 | 视需要而定 |

## D. 公开发布与隐私

- 公共仓库的文件和提交历史对所有人可见。
- GitHub Pages 网站是公开网页，即使仓库在某些计划下为私有也是如此。
- 不要把密码、API Key、家庭住址、私人聊天或未获授权的内容写进仓库。
- 如果一篇文章仍是私密草稿，先放在**不公开的独立仓库**或本地目录。不要以为删除公开 commit 就足以抹去历史。

## E. GitHub Pages 配置

1. 进入 GitHub 仓库 **Settings → Pages**。
2. **Source → Deploy from a branch**。
3. **Branch → main → /(root) → Save**。
4. 打开 **Visit site** 查看发布后的网页。

网站通过 Jekyll 自动聚合 `_journal` 和 `_posts`，无需手动更新索引。

---

提示：如果不需要网站，GitHub 本身也可以阅读所有 Markdown 文件。`README.md` 就是你的仓库首页。
