# Joker Make Blog

这是个人博客的免费部署版本，使用 Hexo 生成静态站点，并通过 GitHub Actions 发布到 GitHub Pages。

访问地址：

- https://joker-make.github.io/blog/

## 本地开发

```bash
npm install
npm run server
```

本地预览默认地址为 `http://localhost:4000/blog/`。

## 写作

```bash
npm run new -- "文章标题"
```

文章会生成在 `source/_posts/`。使用 Markdown 编写正文，通过 Front Matter 配置分类和标签。

示例：

```md
---
title: Spring Boot 学习笔记
date: 2026-07-05 10:00:00
categories:
  - 后端
tags:
  - Spring Boot
  - Java
---
```

## 构建

```bash
npm run build
```

构建产物输出到 `public/`，该目录不提交到仓库。

## 部署

推送到 `main` 分支后，`.github/workflows/pages.yml` 会自动安装依赖、生成静态文件，并发布 `public/` 到 GitHub Pages。

第一次使用前，请在 GitHub 仓库设置中确认 Pages 的 Source 选择为 **GitHub Actions**。
