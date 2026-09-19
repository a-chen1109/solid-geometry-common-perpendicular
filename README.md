# 立体几何交互教学 · 公垂线

以佛山一模立体几何题为背景，用 Three.js 做 3D 可视化，交互式演示异面直线公垂线的解法。

## 在线访问

https://a-chen1109.github.io/solid-geometry-common-perpendicular/

## 目录结构

```
.
├── index.html   # 单文件页面：HTML + CSS + JS 全部内联
└── docs/        # 参考论文（多角度探究立体几何公垂线问题）
```

## 部署方式

GitHub Pages **分支部署**：`Settings → Pages → Source` 选择 `main` 分支 + 根目录 `/`。

页面是纯静态单文件，无需构建步骤，推送到 `main` 后 GitHub 会自动重新发布（约 1 分钟生效）。

> 若后续需要构建流程（压缩、预处理等），可改用 Actions 部署：在 `.github/workflows/` 加工作流即可。
> 注意：推送工作流文件要求 Personal Access Token 带 `workflow` 权限，仅有 `repo` 权限会被拒绝。

## 外部依赖

页面通过 CDN 加载以下库，无需本地安装：

- [Three.js](https://unpkg.com/three) — 3D 渲染
- [MathJax 3.2.2](https://cdnjs.cloudflare.com/ajax/libs/mathjax/3.2.2/es5/tex-mml-chtml.min.js) — 公式排版

## 本地预览

直接用浏览器打开 `index.html` 即可，或起一个静态服务：

```bash
python -m http.server 8000
```
