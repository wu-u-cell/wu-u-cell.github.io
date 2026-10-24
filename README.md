# wu-u-cell · 个人博客

基于 Jekyll 的纯 HTML、CSS 与 Markdown 个人博客，发布到 GitHub Pages。写作和页面维护不需要 Node.js、npm、前端框架、外部 CDN 或本地构建工具；GitHub Actions 负责在 GitHub 上构建 Jekyll 并发布。

## 内容位置

- `_posts/`：文章，文件名使用 `YYYY-MM-DD-title.md`，保留文章 Front Matter。
- `index.html`：首页介绍与项目卡片。
- `about.md`：关于页面。
- `assets/style.css`：颜色、排版和响应式样式。
- `_config.yml`：站点标题、简介、语言、时区和文章链接格式。
- `.github/workflows/pages.yml`：GitHub Pages 的 Jekyll 构建与部署工作流。

## 发布

将变更提交并推送到 `main` 分支后，`Build and deploy Jekyll site` 工作流会构建网站并发布到 GitHub Pages。工作流使用 GitHub 官方 Actions，不需要在本机安装 Ruby 或 Jekyll。

仓库设置中的 Pages 发布来源应为 **GitHub Actions**。个人站点网址为 <https://wu-u-cell.github.io/>。

## 本地编辑

可使用任意文本编辑器修改 HTML、CSS、YAML 和 Markdown。文章正文在 `_posts/` 中编写。提交前先查看 `git status` 和 `git diff`，确认改动后再提交。
