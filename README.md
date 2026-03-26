# 具身智能周报 (Embodied AI Weekly)

[![Weekly Archive](https://github.com/Jessy-Huang/embodied-ai-weekly/actions/workflows/weekly-archive.yml/badge.svg)](https://github.com/Jessy-Huang/embodied-ai-weekly/actions/workflows/weekly-archive.yml)

📊 每周自动追踪具身智能领域的前沿动态，包括 Arxiv 论文、GitHub 热门仓库及各大公司/实验室进展。

## 🌐 在线访问

- **最新周报**: https://jessy-huang.github.io/embodied-ai-weekly/latest/
- **历史归档**: https://jessy-huang.github.io/embodied-ai-weekly/archive/

## 📁 目录结构

```
.
├── .github/workflows/    # GitHub Actions 自动化配置
├── archive/              # 历史归档（按日期命名）
│   ├── index.html        # 归档索引页
│   └── 2026-03-26.html   # 具体日期周报
├── latest/               # 最新周报
│   └── index.html        # 当前最新版
└── README.md             # 本文件
```

## 🔄 自动化流程

### 每周自动归档

- **触发时间**: 每周一早上 8 点 (UTC 00:00)
- **执行内容**:
  1. 将 `latest/index.html` 归档到 `archive/YYYY-MM-DD.html`
  2. 更新归档索引页面
  3. 自动部署到 GitHub Pages

### 手动触发

在 GitHub 仓库页面 → Actions → Weekly Archive and Deploy → Run workflow

## 📝 更新周报

1. 将新的周报 HTML 文件保存为 `latest/index.html`
2. 提交并推送到 GitHub:
   ```bash
   git add latest/index.html
   git commit -m "Update weekly report for $(date +%Y-%m-%d)"
   git push
   ```
3. GitHub Actions 会自动部署到 Pages

## 🚀 首次设置

1. 开启 GitHub Pages:
   - 进入仓库 Settings → Pages
   - Source 选择 "GitHub Actions"

2. 完成！等待 Actions 运行完成即可访问

## 📄 License

MIT License
