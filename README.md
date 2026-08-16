# Hi, I'm PerryLink 👋

**15 DeepSeek Harness plugins, one goal: bring the best of Claude Code into DSH — checkpoints, permission rules, output styles, memory, and more.**

DeepSeek Harness turned "everything is a plugin" into an ecosystem. I build the plugins I wish existed: engineering-discipline guardrails, runtime management panels, cross-session memory, and the Claude Code features I missed most. Every project ships with a five-language README, CI, npm publishing, and a `dsh-plugin` topic.

---

## 🚀 Flagship trio (start here)

| Plugin | What it gives you | Install |
|---|---|---|
| [dsh-checkpoint-rewind](https://github.com/PerryLink/dsh-checkpoint-rewind) | Claude Code `/rewind` equivalent: git-first snapshots before every mutation, session forks, one-shot restore | `dsh plugin --profile web add dsh-checkpoint-rewind` |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Claude Code-style declarative allow/deny/ask rules with full audit | `dsh plugin --profile web add dsh-permission-rules` |
| [dsh-output-styles](https://github.com/PerryLink/dsh-output-styles) | Claude Code `outputStyles` equivalent: runtime-switchable styles | `dsh plugin --profile web add dsh-output-styles` |

## 📦 The full family (15 plugins)

| Plugin | One-liner | npm |
|---|---|---|
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | Read-only MCP runtime panel: `/mcp` + Settings tab | [npm](https://www.npmjs.com/package/dsh-mcp-panel) |
| [dsh-doublecheck](https://github.com/PerryLink/dsh-doublecheck) | Engineering-discipline guard: requirements grill, test gates, adversary review | [npm](https://www.npmjs.com/package/dsh-doublecheck) |
| [dsh-background-agents](https://github.com/PerryLink/dsh-background-agents) | Durable background child agents with a Web UI sidebar | [npm](https://www.npmjs.com/package/dsh-background-agents) |
| [dsh-lsp-actions](https://github.com/PerryLink/dsh-lsp-actions) | LSP diagnostics, formatting, completion, code actions, rename | [npm](https://www.npmjs.com/package/dsh-lsp-actions) |
| [dsh-output-styles](https://github.com/PerryLink/dsh-output-styles) | Runtime-switchable model output styles | [npm](https://www.npmjs.com/package/dsh-output-styles) |
| [dsh-checkpoint-rewind](https://github.com/PerryLink/dsh-checkpoint-rewind) | `/rewind` equivalent: snapshots, forks, restore | [npm](https://www.npmjs.com/package/dsh-checkpoint-rewind) |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Declarative allow/deny/ask permission rules | [npm](https://www.npmjs.com/package/dsh-permission-rules) |
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | Second-model auto-review on the approval chain | [npm](https://www.npmjs.com/package/dsh-auto-review) |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | Approval-gated cross-session memory (`ctx.memory` + SQLite) | [npm](https://www.npmjs.com/package/dsh-memento) |
| [dsh-skill-pack-security](https://github.com/PerryLink/dsh-skill-pack-security) | Security-audit skill pack (5 skills) | [npm](https://www.npmjs.com/package/@perrylink/dsh-skill-pack-security-provider) |
| [dsh-session-pin](https://github.com/PerryLink/dsh-session-pin) | Pin sessions in the Web sidebar | [npm](https://www.npmjs.com/package/dsh-session-pin) |
| [dsh-composer-history](https://github.com/PerryLink/dsh-composer-history) | Terminal-style input history for the web composer | [npm](https://www.npmjs.com/package/dsh-composer-history) |
| [dsh-github](https://github.com/PerryLink/dsh-github) | GitHub PR/issue integration, writes gated by approval | [npm](https://www.npmjs.com/package/@perrylink/dsh-github) |
| [dsh-plugin-guide](https://github.com/PerryLink/dsh-plugin-guide) | Plugin-development knowledge base as an agent skill | — |
| [dsh-claude-move](https://github.com/PerryLink/dsh-claude-move) | Migrate Claude Code sessions, memory, skills into DSH | GitHub Releases |

One-command starter pack: [PerryLink/dsh-kit](https://github.com/PerryLink/dsh-kit)

## 🌍 Where the plugins live

Listed on [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin), [Awesome DeepSeek Harness](https://github.com/0xsline/awesome-deepseek-harness), the [AdamPlatin123 radar](https://github.com/AdamPlatin123/awesome-dsh-plugins), and [dsh-market](https://github.com/dsh-market/dsh-market) (via the awesome-dsh-plugin registry).

## 中文介绍

我在 DeepSeek Harness 上把 Claude Code 里最好用的能力做成了平价插件：`/rewind` 式检查点回退、声明式权限规则、outputStyles 运行时风格、跨会话记忆、MCP 运行时面板……15 个插件全部开源（Apache-2.0），带五语文档、CI 与 npm 发布。旗舰三件套见上方表格，全家桶一键安装：`PerryLink/dsh-kit`。
