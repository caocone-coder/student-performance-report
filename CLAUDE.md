# 学情周报（学生表现报告）

## 项目说明
K12 学情周报 v2 移动端交互原型，面向家长展示孩子的学习进度、错题详情和推荐内容。

## 技术栈
- 单文件 HTML
- 纯 CSS（设计 token 来自 Figma）+ JavaScript
- 字体：Noto Sans SC、ABeeZee（Google Fonts CDN）
- 移动端适配：375px max-width

## 目录结构
```
index.html              # 主报告页面（7MB，图片 base64 内联）
index-dev.html          # 开发版（图片外链，296KB）
index-optimized.html    # 优化版（图片外链，296KB）
cuoti-detail.html       # 错题详情页
xuqing-report/          # 图片资源目录
```

## 部署
- 平台：GitHub Pages
- 仓库：caocone-coder/student-performance-report

## 注意事项
- 多页面通过 JS show/hide 切换，不是真正的路由
- PRD 文档：`student-performance-report-PRD.md`（本目录下）
- 开发时使用 index-dev.html（体积小），发布时用 inline-images.py 内联图片生成 index.html
- 始终以 375px 宽度测试移动端效果
