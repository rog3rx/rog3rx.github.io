# rog3rx.github.io

这是我的个人博客网站，使用Hugo和PaperMod主题构建。

## 技术栈

- [Hugo](https://gohugo.io/) - 静态网站生成器
- [PaperMod](https://github.com/adityatelange/hugo-PaperMod) - Hugo主题
- GitHub Pages - 托管服务

## 本地开发

1. 克隆仓库：
   ```bash
   git clone https://github.com/rog3rx/rog3rx.github.io.git
   cd rog3rx.github.io
   ```

2. 安装依赖：
   ```bash
   # 确保已安装Hugo
   hugo version
   ```

3. 启动本地服务器：
   ```bash
   hugo server -D
   ```

4. 在浏览器中访问 `http://localhost:1313`

## 创建新文章

```bash
hugo new posts/my-new-post.md
```

## 部署

网站通过GitHub Actions自动部署到GitHub Pages。
只需将更改推送到main分支，GitHub Actions将自动构建并部署网站。