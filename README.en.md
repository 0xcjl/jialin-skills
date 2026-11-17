# Jialin Skills

**Agent Skills and tools I use for research, writing, and building projects.** Maintained by [Jialin / 0xcjl](https://github.com/0xcjl).

[简体中文](README.md) · English

This collection contains **9 loadable Agent Skills** and **1 Obsidian plugin**. Choose the item that fits your task. `RecordNote` is installed through Obsidian. Each directory includes its supporting scripts, references, license notices, and original documentation where applicable.

## Explore

| Area | Project | Use it for |
| --- | --- | --- |
| Agent practice | [anti-sycophancy](skills/anti-sycophancy/) | Challenge agreeable answers; extra installation layers are available for Claude Code and OpenClaw. |
| Agent practice | [autoresearch-pro](skills/autoresearch-pro/) | Improve existing skills, prompts, and workflows with bounded, reversible experiments. |
| Agent practice | [perfect-handoff](skills/perfect-handoff/) | Reconcile project facts and prepare a compact, reusable session handoff. |
| Understanding & writing | [clear-view](skills/clear-view/) | Turn dense material into a structured overview and standalone HTML infographic. |
| Understanding & writing | [merge-drafts](skills/merge-drafts/) | Combine article drafts while retaining useful material and author intent. |
| Understanding & writing | [md-pdf-report](skills/md-pdf-report/) | Convert Markdown research reports to PDFs with CJK text support. |
| Understanding & writing | [resume-creator](skills/resume-creator/) | Build fact-grounded Reactive Resume JSON or a single-file HTML résumé. |
| Crypto & security | [onchain-security](skills/onchain-security/) | Review external skills, repositories, links, on-chain assets, and pre-trade risks. |
| Crypto & security | [crypto-research](skills/crypto-research/) | Research crypto projects, protocols, and tokens with traceable evidence and focused fact checks. |
| Companion tool | [RecordNote](tools/RecordNote/) | Transcribe and organize Obsidian recordings into summaries, actions, and Markdown notes; [Obsidian plugin listing](https://community.obsidian.md/plugins/recordnote). **An Obsidian plugin, not an Agent Skill**. |

## Install and use

Clone this repository and copy the **entire skill directory** into your agent's skills location. Discovery rules and permissions differ by client; read that skill's `README.md` and `SKILL.md` first.

```bash
git clone https://github.com/0xcjl/jialin-skills.git
# Example: install clear-view in a common Agent Skills location
cp -R jialin-skills/skills/clear-view ~/.agents/skills/clear-view
```

For `crypto-research`, use its [integrity-checked installer](skills/crypto-research/README.md). Copying `anti-sycophancy` alone does not activate its optional hooks or persistent rules; follow its client-specific instructions.

Install `RecordNote` through **Obsidian → Settings → Community plugins → Browse** or view its [Obsidian plugin listing](https://community.obsidian.md/plugins/recordnote). See its [plugin documentation](tools/RecordNote/README.md).

## Sources and licenses

These projects are maintained separately. This collection is a snapshot pinned to the commits in [SOURCES.md](SOURCES.md); updates to source repositories do not appear here automatically. `onchain-security` and `perfect-handoff` include adapted upstream work and retain their attribution and license files.

Each directory keeps its own license terms; `crypto-research` is now open source under MIT. No repository-wide license is intended to override package-specific terms.

Check each skill's permission, service, and runtime requirements before use. Verify research and security conclusions against current evidence.
