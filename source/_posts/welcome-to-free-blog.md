---
title: 免费部署版博客上线
date: 2026-07-05 09:30:00
categories:
  - 博客建设
tags:
  - Hexo
  - GitHub Pages
  - 静态博客
---

这是个人博客的免费部署版本。

当前版本使用 Hexo 生成静态页面，并通过 GitHub Actions 自动发布到 GitHub Pages。相比原来的 Vue + Spring Boot 全栈版本，这个版本不依赖服务器、数据库或 Redis，更适合免费托管和长期展示。

后续写文章时，只需要在 `source/_posts/` 中新增 Markdown 文件，然后推送到 `main` 分支即可自动部署。
