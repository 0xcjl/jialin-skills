# Jialin Skills

**我在研究、写作和构建项目时使用的 Agent Skills 与工具。** 由 [Jialin / 0xcjl](https://github.com/0xcjl) 维护。

简体中文 · [English](README.en.md)

这里收录 **9 个可加载的 Agent Skill** 和 **1 个 Obsidian 插件**。按实际任务选择单个技能；`RecordNote` 需要在 Obsidian 中安装。每个目录都保留配套的脚本、参考资料、许可及原有说明，不只是一份 `SKILL.md`。

## 找到合适的技能

| 方向 | 项目 | 适合做什么 |
| --- | --- | --- |
| Agent 工作方式 | [anti-sycophancy](skills/anti-sycophancy/) | **介绍：**让 Agent 主动检验用户判断，减少未经核查的附和。<br>**用途：**方案评估、反例检查和风险讨论；Claude Code / OpenClaw 另有可选的 hook 与持久规则。 |
| Agent 工作方式 | [autoresearch-pro](skills/autoresearch-pro/) | **介绍：**用有界、可回退的实验改进现有内容和工作流。<br>**用途：**优化技能、提示词或文章时设定基线、试验小改动，并根据可验证结果保留或回退。 |
| Agent 工作方式 | [perfect-handoff](skills/perfect-handoff/) | **介绍：**把项目当前状态整理成下一次会话能接续的短交接。<br>**用途：**长任务收尾时核对项目事实、记录未完成事项，并给出可复制的新会话开场提示词。 |
| 理解与表达 | [clear-view](skills/clear-view/) | **介绍：**把难读的材料变成文字结构图和独立 HTML 信息图。<br>**用途：**梳理长对话、文章、论文或产品说明中的人物观点、主题关系、分歧与待确认问题。 |
| 理解与表达 | [merge-drafts](skills/merge-drafts/) | **介绍：**将多份文章草稿合成一份连贯成稿。<br>**用途：**不同版本各有亮点时，去重、补齐逻辑、保留事实与作者意图，并整理可审阅的文章结构。 |
| 理解与表达 | [md-pdf-report](skills/md-pdf-report/) | **介绍：**从同一份 Markdown 生成可分享的排版 PDF。<br>**用途：**制作多语言调研报告、事实核查和方案文档；表格、引用及混排文字通过已安装的系统字体渲染。 |
| 理解与表达 | [resume-creator](skills/resume-creator/) | **介绍：**把已核实的经历做成可编辑、可展示的简历。<br>**用途：**整理求职材料，生成 Reactive Resume JSON 或可离线打开、打印的单文件 HTML，并明确选择语言与版式。 |
| Crypto 与安全 | [onchain-security](skills/onchain-security/) | **介绍：**给外部输入和链上行动加一套可审查的风险检查。<br>**用途：**安装技能或 MCP 前、打开可疑链接、审查仓库、分析合约与代币，以及交易前记录证据和风险等级。 |
| Crypto 与安全 | [crypto-research](skills/crypto-research/) | **介绍：**用带来源和时间戳的证据研究 Crypto 项目与代币。<br>**用途：**了解产品进展、链上变化、流动性、注意力和筹码结构，也可核查单条说法并复盘既有判断。 |
| 配套工具 | [RecordNote](tools/RecordNote/) | **介绍：**把 Obsidian 中的录音整理为可检索的 Markdown 笔记。<br>**用途：**会议或语音速记的转写、摘要、待办提取与导出；它是 [Obsidian 插件市场中的插件](https://community.obsidian.md/plugins/recordnote)，不是 Agent Skill。 |

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
