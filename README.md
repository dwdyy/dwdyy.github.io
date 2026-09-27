# Dongwei 的技术笔记

这是 [dwdyy.github.io](https://dwdyy.github.io/) 的 Hugo 源码，使用
[Austere](https://github.com/tomwrw/austere-theme-hugo) 主题，并由 GitHub Actions 自动发布。

## 本地预览

需要 Hugo 0.166.0 或更新版本：

```bash
hugo server -D
```

浏览器打开 `http://localhost:1313/`。

## 新建文章

```bash
hugo new content posts/my-post.md
```

将文章 front matter 中的 `draft` 改为 `false` 后提交并推送到 `main`，GitHub Pages 会自动构建和发布。

## 数学公式

行内公式使用 `\( ... \)`，例如 `\(O(n \log n)\)`。

块级公式使用 `\[ ... \]` 或 `$$ ... $$`。公式由 Hugo 内置的 KaTeX 引擎在构建时渲染，无需浏览器端 JavaScript。

