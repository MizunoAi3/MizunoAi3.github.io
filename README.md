# Mizuno AI Blog

已设置一个最小的 Jekyll 博客样板，部署到 GitHub Pages（通过 Actions 自动构建并发布到 gh-pages 分支）。

写博客：
- 在 `_posts/` 文件夹中创建 Markdown 文件，文件名格式：`YYYY-MM-DD-your-title.md`
- 每个文章顶部加上 front matter，例如：
```
---
layout: post
title: "文章标题"
date: 2026-06-24 14:08:00 +0800
---
```

发布：
- 将修改 push 到 `main` 分支，Actions 会自动构建并把静态站点发布到 `gh-pages` 分支。

注意：
- 打开 `_config.yml`，把 `url` 替换成你的 GitHub Pages 地址（例如 `https://your-username.github.io`）。
- 如果需要本地预览，需安装 Ruby / Bundler，然后运行：
  - `bundle install`
  - `bundle exec jekyll serve`

如果需要把站点主题或样式改成你喜欢的样子，可以告诉我想要的样式，我来帮你调整。