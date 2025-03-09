---
title: "GitHub Actions 部署测试"
date: 2024-03-09
draft: false
tags: ["博客", "Hugo", "GitHub Actions"]
categories: ["技术"]
---

## GitHub Actions 部署测试

这是一篇用于测试 GitHub Actions 自动部署 Hugo 网站的文章。

## GitHub Actions 的优势

使用 GitHub Actions 部署 Hugo 网站有以下优势：

1. **自动化部署** - 提交代码后自动构建和部署
2. **版本控制** - 网站内容和配置都在版本控制中
3. **零成本** - 对公开仓库免费
4. **高度可定制** - 可以根据需求自定义工作流

## 测试代码高亮

```yaml
name: Deploy Hugo site to Pages

on:
  push:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout
        uses: actions/checkout@v4
      
      - name: Setup Hugo
        uses: peaceiris/actions-hugo@v2
        with:
          hugo-version: '0.126.1'
          extended: true
```

## 成功部署后

如果您能看到这篇文章，说明 GitHub Actions 工作流已经成功部署！ 