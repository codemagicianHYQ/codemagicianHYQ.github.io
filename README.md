# 胡永奇的技术博客

基于 `jekyll-theme-chirpy` 的 GitHub Pages 个人博客。  
内容以技术学习、实践复盘、个人思考为主。

## 我该在哪里写文章？

直接在仓库的 `_posts` 目录写 Markdown 文件，不需要后台管理系统。

文件名格式：

```text
YYYY-MM-DD-your-title.md
```

最小模板：

```markdown
---
title: 文章标题
date: 2026-05-18 12:00:00 +0800
categories: [技术, 分类]
tags: [标签1, 标签2]
description: 一句话摘要
---

这里写正文（Markdown）。
```

## 发布流程（无后台版）

1. 在 `_posts` 新建文章
2. 本地预览（可选）：`bundle exec jekyll s`
3. 提交并推送到 GitHub
4. GitHub Pages 自动构建上线

## 是否需要后台管理系统？

对于技术博客场景，**通常不需要**。  
你现在这套「Markdown + GitHub Pages」已经足够稳定，优势是：

- 成本低、长期可维护
- 版本可追溯（Git 天然版本管理）
- 可离线写作，迁移成本小

如果未来你需要多人协作或可视化编辑，再考虑接入 CMS（如 Netlify CMS/Decap CMS）即可。
