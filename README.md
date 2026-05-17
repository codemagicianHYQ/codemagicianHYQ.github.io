# 胡永奇的技术博客

基于 `jekyll-theme-chirpy` 的 GitHub Pages 个人博客。  
内容以技术学习、实践复盘、个人思考为主。

## 我该在哪里写文章？

你有两种方式：

- 直接在仓库的 `_posts` 目录写 Markdown
- 使用网站后台：`/admin/`

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

## 网页后台写作（已接入 Sveltia CMS）

后台地址：

```text
https://codemagicianhyq.github.io/admin/
```

支持能力：

- 新建/编辑/删除 `_posts` 文章
- 可视化填写标题、时间、分类、标签、摘要
- 支持图片上传到 `assets/uploads`
- 使用编辑流（草稿 -> 审核 -> 发布）

### 首次登录（推荐 Token 方式）

1. 打开 `/admin/` 页面
2. 点击 `Sign in with Token`
3. 按页面提示到 GitHub 生成 Personal Access Token
4. 勾选仓库写权限后，复制粘贴回后台即可登录

> 这个方式最适合「个人单作者博客」：不需要额外部署 OAuth 服务。

### 可选：OAuth 登录（多人协作再考虑）

如果后续你要给多人使用，再补 OAuth 代理（如 Sveltia CMS Auth + Cloudflare Worker）即可。

## 是否需要后台管理系统？

对于技术博客场景，**通常不需要**。  
你现在这套「Markdown + GitHub Pages」已经足够稳定，优势是：

- 成本低、长期可维护
- 版本可追溯（Git 天然版本管理）
- 可离线写作，迁移成本小

如果你主要是自己写技术文章，其实本地 Markdown 已经够用；  
如果你更偏好网页可视化编辑，就使用现在已接入的 `/admin/`。
