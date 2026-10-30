# 野球鹿

个人文学博客，基于 [Interleaf](https://github.com/DRAG0NM/astro-theme-interleaf) 构建，使用 GitHub Pages 发布。

## 添加文章

在 `src/content/posts/` 中新建一个 Markdown 文件，例如 `雨夜.md`：

```md
---
title: 雨夜
published: 2026-10-30
description: 一段关于雨夜的文字。
tags:
  - 散文
lang: zh
abbrlink: rainy-night
---

从这里开始写正文。
```

将文件提交并推送到 `main` 分支后，GitHub Actions 会重新发布网站。`draft: true` 可把文章暂存为草稿，不在正式网站上显示。修改站名、副标题、作者和网址请编辑 `src/config.ts`；修改关于页请编辑 `src/content/about/about-zh.md`。

## 本地预览

需要 Node.js 22.12 或更新版本。安装依赖并预览：

```sh
corepack enable
pnpm install --frozen-lockfile
pnpm dev
```

构建检查：`pnpm build`。

## 主题与许可

网站代码基于 Interleaf，保留其 [MIT 许可](LICENSE)与 [NOTICE](NOTICE.md)。文章版权归各自作者所有。
