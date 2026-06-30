# Topo 链 DApp 开发者文档

这是 Topo 链 DApp 开发者最佳实践文档的 GitHub Pages 站点源码，基于 Jekyll 和 Just the Docs。文档结构参考 `just-the-docs/just-the-docs` 主分支的站点组织方式：根目录首页、`docs/` 文档目录、front matter 驱动的左侧导航，以及页面内 Kramdown TOC。

## 文档结构

- `index.md`：站点首页。
- `docs/index.md`：开发者文档总目录。
- `docs/01-overview-architecture.md` 到 `docs/06-launch-antipatterns-roadmap.md`：按工程主题聚合后的 6 个章节。
- 每个聚合章节保留原始章节标题、表格、检查清单和 Mermaid 图，减少 GitHub Pages 左侧导航层级。
- 站内页面链接使用 `{% link ... %}`，适配 Just the Docs 的 `permalink: pretty` 配置。

## 本地预览

安装 Ruby 和 Bundler 后运行：

```bash
bundle install
bundle exec jekyll serve
```

站点默认可在 `http://localhost:4000` 预览。GitHub Pages 发布时使用 `.github/workflows/pages.yml` 构建。
