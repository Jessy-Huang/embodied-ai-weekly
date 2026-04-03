# embodied-ai-weekly Skill

> 具身智能周报自动化生成与发布 Skill，适用于 WorkBuddy / CodeBuddy。

## 功能

覆盖完整的具身智能周报工作流：

1. **Phase 1 — ArXiv 论文检索**：7 个方向关键词检索，生成论文摘要 `.md` + 可视化 `.html`
2. **Phase 2 — GitHub 开源追踪**：7 个方向仓库趋势追踪，生成 `.md` + `.html`
3. **Phase 3 — 综合报告生成**：整合双源数据，生成带导读、统计图表的暗色主题 HTML 报告
4. **Phase 4 — GitHub Pages 发布**：SSH 推送到 `YYYY-W{N}/` 文件夹，自动更新 `latest/` 与 `archive/`

## 安装方法

### 方法一：直接解压（推荐）

1. 下载本目录下的 [`embodied-ai-weekly.zip`](./embodied-ai-weekly.zip)
2. 解压到 WorkBuddy 用户级 skill 目录：

   **Windows：**
   ```
   解压至 C:\Users\<你的用户名>\.workbuddy\skills\
   确保目录结构为：
   ~/.workbuddy/skills/embodied-ai-weekly/SKILL.md
   ```

   **macOS / Linux：**
   ```
   解压至 ~/.workbuddy/skills/
   确保目录结构为：
   ~/.workbuddy/skills/embodied-ai-weekly/SKILL.md
   ```

3. 重启 WorkBuddy，skill 自动生效

### 方法二：手动复制

把本目录下的文件按如下结构放置：

```
~/.workbuddy/skills/embodied-ai-weekly/
├── SKILL.md
└── references/
    ├── arxiv_search_guide.md
    ├── github_search_guide.md
    └── html_template_guide.md
```

## 使用方式

安装后，在对话中说：

```
帮我生成具身智能 2026-W14 周报（2026-04-03 ~ 2026-04-09），推送到 Jessy-Huang/embodied-ai-weekly
```

Skill 会自动加载 SOP，按四个阶段执行完整流程。

## 前提条件

- 已配置 GitHub SSH 密钥（HTTPS 在部分网络环境下超时，推荐 SSH）
- GitHub 仓库已启用 GitHub Pages（`main` 分支 `/` 根目录）

## 文件说明

| 文件 | 说明 |
|------|------|
| `SKILL.md` | Skill 主文件，含完整 SOP 与执行指引 |
| `references/arxiv_search_guide.md` | 7 方向 ArXiv 检索关键词与 URL 模板 |
| `references/github_search_guide.md` | 7 方向 GitHub 检索策略与经典仓库清单 |
| `references/html_template_guide.md` | 暗色主题 HTML 报告风格规范（CSS 变量/组件/动画） |
| `embodied-ai-weekly.zip` | 完整 skill 打包文件，直接解压即可安装 |
