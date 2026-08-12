# 许鹏的技术博客

基于 [Hugo](https://gohugo.io/) 与 [PaperMod](https://github.com/adityatelange/hugo-PaperMod) 构建，并通过 GitHub Pages 自动发布。

## 写文章

在 `content/posts/` 下新建 Markdown 文件，例如：

```markdown
---
title: "文章标题"
date: 2026-04-13
draft: false
tags: ["工程"]
summary: "一句摘要"
---

正文。
```

推送至 `main` 后，GitHub Actions 会自动构建并发布。

## 互动反馈

评论和 reaction 由 [Giscus](https://giscus.app/zh-CN) 提供，内容保存在本仓库的 GitHub Discussions。

首次启用前，需要以仓库管理员身份访问 [giscus GitHub App](https://github.com/apps/giscus)，将它安装并授权给本仓库；当前配置已关联 `General` 分类。访客须登录 GitHub 才能评论或添加 reaction。

## 访问统计（可选）

注册 [Umami Cloud](https://cloud.umami.is/)，创建网站后，将站点 ID 填入 `hugo.toml` 的 `params.umami.websiteID`。它会收集访问量、热门页面和来源等匿名统计数据。

## 本地预览

安装 Hugo Extended 后运行：

```bash
git submodule update --init --recursive
hugo server -D
```
