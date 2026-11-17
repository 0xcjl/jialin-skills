# Jialin Skills

**我在研究、写作和构建项目时使用的 Agent Skills 与工具。** 由 [Jialin / 0xcjl](https://github.com/0xcjl) 维护。

简体中文 · [English](README.en.md)

这里收录 **9 个可加载的 Agent Skill** 和 **1 个 Obsidian 插件**。按实际任务选择单个技能；`RecordNote` 需要在 Obsidian 中安装。每个目录都保留配套的脚本、参考资料、许可及原有说明，不只是一份 `SKILL.md`。

## 找到合适的技能

| 方向 | 项目 | 适合做什么 |
| --- | --- | --- |
| Agent 工作方式 | [anti-sycophancy](skills/anti-sycophancy/) | 检查迎合性回答；Claude Code / OpenClaw 有额外的安装层。 |
| Agent 工作方式 | [autoresearch-pro](skills/autoresearch-pro/) | 用有界、可回退的实验改进技能、提示词和工作流。 |
| Agent 工作方式 | [perfect-handoff](skills/perfect-handoff/) | 整理项目事实并制作可复制的新会话交接入口。 |
| 理解与表达 | [clear-view](skills/clear-view/) | 把复杂材料整理成文字概览和独立 HTML 信息图。 |
| 理解与表达 | [merge-drafts](skills/merge-drafts/) | 合并多份文章草稿，保留有价值的内容与作者意图。 |
| 理解与表达 | [md-pdf-report](skills/md-pdf-report/) | 将 Markdown 研究报告生成支持中日韩文字的 PDF。 |
| 理解与表达 | [resume-creator](skills/resume-creator/) | 用已核实的经历制作 Reactive Resume JSON 或单文件 HTML 简历。 |
| Crypto 与安全 | [onchain-security](skills/onchain-security/) | 审查外部技能、仓库、链接及链上标的和交易前风险。 |
| Crypto 与安全 | [crypto-research](skills/crypto-research/) | 用可追溯证据研究 Crypto 项目、协议和代币；支持单条事实核查。 |
| 配套工具 | [RecordNote](tools/RecordNote/) | Obsidian 录音转写、摘要、待办与 Markdown 笔记；[插件市场页面](https://community.obsidian.md/plugins/recordnote)。**它是插件，不是 Agent Skill**。 |

## 安装与使用

克隆仓库后，把**整个技能目录**放进所用 Agent 的技能目录。不同客户端的目录、发现和执行权限可能不同，请先查看所选技能的 `README.md` 与 `SKILL.md`。

```bash
git clone https://github.com/0xcjl/jialin-skills.git
# 示例：将 clear-view 安装到通用 Agent Skills 目录
cp -R jialin-skills/skills/clear-view ~/.agents/skills/clear-view
```

`crypto-research` 自带校验清单和安装器，请按 [专属安装说明](skills/crypto-research/README.md) 操作。`anti-sycophancy` 的自动 hook 只适用于其文档列出的客户端；复制目录本身不会启用所有防护层。

`RecordNote` 请在 Obsidian 的 **设置 → 第三方插件 → 浏览** 中搜索并安装，也可查看 [Obsidian 插件市场页面](https://community.obsidian.md/plugins/recordnote)；说明见 [插件文档](tools/RecordNote/README.md)。

## 来源与许可

各项目原本独立维护；本仓库是按 [SOURCES.md](SOURCES.md) 中的提交固定的合集快照。后续源仓库更新不会自动同步到这里。`onchain-security` 和 `perfect-handoff` 含有上游改编内容，保留了原有署名与许可文件。

各目录按自身许可文件处理，`crypto-research` 已以 MIT 许可开源。本仓库没有用一个总许可证覆盖所有目录。

使用前查看技能的权限、外部服务和运行环境要求；研究或安全审查结果应依据当次证据复核。
