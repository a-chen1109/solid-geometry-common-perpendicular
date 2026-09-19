# 立体几何交互教学 · 公垂线

以佛山一模立体几何题为背景，用 Three.js 做 3D 可视化，交互式演示异面直线公垂线的两种解法。

## 在线访问

推送到 `main` 分支后由 GitHub Actions 自动部署到 GitHub Pages，地址形如：

```
https://<用户名>.github.io/solid-geometry-common-perpendicular/
```

首次部署需约 1–2 分钟，可在仓库 **Actions** 标签页查看进度。

## 目录结构

```
.
├── index.html          # 单文件页面：HTML + CSS + JS 全部内联
├── docs/               # 参考论文（多角度探究立体几何公垂线问题）
└── .github/workflows/
    └── deploy-pages.yml  # Pages 自动部署工作流
```

## 外部依赖

页面通过 CDN 加载以下库，无需本地安装：

- [Three.js](https://unpkg.com/three) — 3D 渲染
- [MathJax 3.2.2](https://cdnjs.cloudflare.com/ajax/libs/mathjax/3.2.2/es5/tex-mml-chtml.min.js) — 公式排版

## 本地预览

直接用浏览器打开 `index.html` 即可，或起一个静态服务：

```bash
python -m http.server 8000
```

## 启用 GitHub Pages

首次推送后需手动确认一次：

1. 仓库 **Settings → Pages**
2. **Source** 选择 `GitHub Actions`
3. 保存

若是通过 API 创建并配置，此步已自动完成，无需再操作。
