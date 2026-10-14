# 王东威 · Dongwei Wang

[![Build and deploy Hugo site](https://github.com/dwdyy/dwdyy.github.io/actions/workflows/hugo.yaml/badge.svg)](https://github.com/dwdyy/dwdyy.github.io/actions/workflows/hugo.yaml)

个人学术主页：[dwdyy.github.io](https://dwdyy.github.io/)。
使用 [Minimal Light](https://github.com/yaoyao-liu/minimal-light) 的本地 Hugo 适配版，主题来源与许可见 `themes/minimal-light/README.md` 和 `LICENSE`。

## 修改内容

- `data/resume.toml`：姓名、邮箱、教育、奖项、项目、技能。
- `content/_index.md`：个人介绍正文。
- `hugo.toml`：网站信息、导航、数学公式配置。
- `themes/minimal-light/assets/css/resume.css`：本地排版、配色和打印样式。

奖项按本人提供的简历录入。项目源代码链接和 PDF 简历可在准备好后添加；当前没有占位链接。页面不展示头像或手机号。

## 本地预览与发布

使用 Hugo 0.166.0，在项目目录运行 `hugo server -D`，访问 http://localhost:1313/。
正式构建运行 `hugo --gc --minify`。推送 `main` 后由 GitHub Actions 发布。
原博客文章保留其地址，但不在学术主页导航中显示。旧版主题保留在 Git 历史和源码目录中，不参与当前站点构建。

## LaTeX 公式

行内使用 `\( ... \)`，块级使用 `\[ ... \]` 或 `$$ ... $$`。
Hugo 在构建时使用内置 KaTeX 生成 HTML 和 MathML。
