# clear-view

[English](README.md) | 简体中文

> 一个 Agent skill：把任意对话、文章、论文、教程、产品说明或混乱的讨论，快速整理成「现在是什么情况」——一份结构化文字版，加一份轻量、自包含的 HTML 信息图。

## 它做什么

每次固定两件交付（除非你明确只要其中一种）：

1. **文字版**：主题、一句话现状、结构/流程、各方说了什么、话题线、共同点、争论点、未决问题和简短小结。材料里没有的栏目直接跳过。
2. **可视版**：单文件、可离线打开的 HTML 信息图，用角色标记和图例区分说话人，画出话题分叉、步骤或关系图。Mermaid 或树形图只在有帮助时追加，不替代 HTML。

忠实原文：观点归说话人；含糊处标「原文未明」（图上用虚线或问号）；不站队、不编造原文没有的事实。

## 适用场景

- 群聊或会议里分不清谁在争什么
- 长文或论文想按论点和证据画结构
- 教程目录不清
- 产品说明功能分散
- 任何「讲清楚 / 画清楚 / 理清一下」的需求

不适合：只要一句话摘要、只要翻译、只要改代码。

## 安装

把本目录复制到你的 Agent skills 目录即可。核心是一份可移植的 `SKILL.md`，适用于 Codex、Claude Code、Hermes、OpenClaw 等兼容 Agent Skills 的客户端。中文版位于 `zh-CN/SKILL.md`。

```bash
git clone https://github.com/0xcjl/clear-view.git
cp -r clear-view ~/.agents/skills/clear-view   # 按你的客户端调整路径
```

从 ClawHub 安装（英文版）：

```bash
clawhub install clear-view
```

## 用法

把材料交给 Agent，并说例如：

> 用 clear-view 理清这段讨论。

聊天里会拿到结构化文字版，另有一个 `clear-view-{short-slug}.html` 文件可打开查看。

## 致谢

「选最短够用的可视化」这一思路受 [humanlayer/skills](https://github.com/humanlayer/skills) 中 `show-me` skill 启发。clear-view 为独立重写，面向文本澄清而非代码，没有复制该项目的文件。

## 许可

MIT
