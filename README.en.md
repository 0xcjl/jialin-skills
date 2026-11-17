# Jialin Skills

**Agent Skills and tools I use for research, writing, and building projects.** Maintained by [Jialin / 0xcjl](https://github.com/0xcjl).

[简体中文](README.md) · English

This collection contains **9 loadable Agent Skills** and **1 Obsidian plugin**. Choose the item that fits your task. `RecordNote` is installed through Obsidian. Each directory includes its supporting scripts, references, license notices, and original documentation where applicable.

## Explore

| Area | Project | Use it for |
| --- | --- | --- |
| Agent practice | [anti-sycophancy](skills/anti-sycophancy/) | Prompts an agent to test assumptions instead of agreeing too quickly. Use it for proposal reviews, counterexamples, and risk discussions; Claude Code and OpenClaw have optional hook and persistent-rule layers. |
| Agent practice | [autoresearch-pro](skills/autoresearch-pro/) | Improves existing work through bounded, reversible experiments. Use it to baseline a skill, prompt, article, or workflow, try a small change, and keep or revert it based on observable results. |
| Agent practice | [perfect-handoff](skills/perfect-handoff/) | Turns current project state into a short handoff for the next session. Use it at the end of long tasks to reconcile facts, record unfinished work, and prepare a ready-to-paste opening prompt. |
| Understanding & writing | [clear-view](skills/clear-view/) | Converts dense material into a structured explanation and standalone HTML infographic. Use it to map speakers, arguments, topic relationships, disagreements, and open questions in conversations, papers, or briefs. |
| Understanding & writing | [merge-drafts](skills/merge-drafts/) | Combines several article drafts into one coherent version. Use it when different drafts contain useful passages that need deduplication, clearer logic, and an editor-ready structure without losing author intent. |
| Understanding & writing | [md-pdf-report](skills/md-pdf-report/) | Produces a shareable, styled PDF from one editable Markdown source. Use it for multilingual research reports, fact checks, and proposals with tables, citations, and mixed scripts rendered through installed system fonts. |
| Understanding & writing | [resume-creator](skills/resume-creator/) | Builds presentable résumés from verified career facts. Use it to create Reactive Resume JSON or an offline, printable single-file HTML résumé after choosing its language and visual style. |
| Crypto & security | [onchain-security](skills/onchain-security/) | Adds an auditable risk review before trusting external inputs or on-chain actions. Use it before installing skills or MCP servers, opening suspicious links, reviewing repositories or contracts, and recording pre-trade evidence. |
| Crypto & security | [crypto-research](skills/crypto-research/) | Studies crypto projects and tokens with timestamped, traceable evidence. Use it to examine product progress, on-chain changes, liquidity, attention, and holder structure, or to fact-check a claim and revisit earlier judgments. |
| Companion tool | [RecordNote](tools/RecordNote/) | Turns Obsidian recordings into searchable Markdown notes. Use it for meeting or voice-note transcription, summaries, action items, and export; it is an [Obsidian Community Plugin](https://community.obsidian.md/plugins/recordnote), not an Agent Skill. |

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
