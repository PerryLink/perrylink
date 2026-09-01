# Hi, I'm PerryLink 👋

[![Gitee mirror](https://img.shields.io/badge/Gitee-mirror-c71d23?logo=gitee)](https://gitee.com/perrylink)
[![npm packages](https://img.shields.io/badge/npm-packages-cb3837?logo=npm)](https://www.npmjs.com/search?q=perrylink)
![plugins](https://img.shields.io/badge/plugins-34-0969da)
![repos](https://img.shields.io/badge/repos-100%2B-green)
![stars](https://img.shields.io/badge/stars-603%2B-yellow)
![npm downloads](https://img.shields.io/badge/npm_downloads-60k%2Fmonth-cb3837)

**Building the DeepSeek Harness plugin ecosystem: 34 open-source plugins (Apache-2.0) across security, workflows, research, and developer experience. Every project ships five-language READMEs, CI, npm publishing, and Gitee mirrors — 60k+ monthly npm downloads across the family.**

DeepSeek Harness turned "everything is a plugin" into an ecosystem. I build the plugins I wish existed — engineering-discipline guardrails, runtime panels, cross-session memory, and verifiable research engines — and publish them the way production software deserves.

---

## 📣 Latest — 2026-09-01 ecosystem round

- **Registry sprint**: 27 entries live on [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) · re-submission PRs open for dsh-fast / dsh-session-sync / dsh-talk (one-plugin per maintainer preference; dsh-budget / dsh-click / dsh-draw up next) · ecosystem PRs open: [AdamPlatin123 radar #440](https://github.com/AdamPlatin123/dsh-plugin-radar/pull/440) · [Zhiyuan-Fan #59](https://github.com/Zhiyuan-Fan/Awesome-DeepSeek-Harness-Plugins/pull/59) · [Herdeny #3](https://github.com/Herdeny/awesome-dsh-plugins-2026/pull/3) · official [DeepSeek Harness guide PR](https://github.com/deepseek-ai/awesome-deepseek-agent/pull/410) on awesome-deepseek-agent.
- **Brand protection**: official-repository declaration merged into 11 repos (same-name repository defense, including the 68-star name collision on dsh-github).
- **Adoption (2026-09-01 snapshot)**: **603★** across 35 repos (up from 574 on 08-31; topic top-100 threshold now 500) · **60.8k npm downloads in August** (23.0k in the last 7 days — release-week surge) — top by downloads: dsh-mcp-panel 3.9k · dsh-permission-rules 3.1k · dsh-memento 2.8k · dsh-checkpoint-rewind 2.7k · dsh-auto-review 2.7k · dsh-lsp-actions 2.5k. Per-package live badges on each repo.
- Full audit (2026-08-27): 33/33 install · load · keyless-boot · uninstall — all green.
- **Supply chain**: OpenSSF Scorecard CI on all 35 repos · npm provenance on every publish (Trusted Publishing verified with a live release) · `funding` links and the 1024-store install channel on every README.
- **Certification**: [dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification) spec v1 published — five machine-checkable dimensions, A–D grades, independent registry + badges · **first registry entry live: dsh-auto-review Grade B** (2026-08-31 snapshot) · proposal posted on the official security-audit discussion [#454](https://github.com/deepseek-ai/deepseek-harness/discussions/454).
- **Community**: official [Showcase post](https://github.com/deepseek-ai/deepseek-harness/discussions/5016) + 37 answered questions across the official repo and the ecosystem · 36 entries auto-listed on [deepseek1024.com](https://deepseek1024.com).
- **New releases**: npm channel fully unlocked on 08-30 — 21 publishes in one day, 26 versions now live on npm, including @perrylink/dsh-github 0.7.1 · dsh-session-pin 0.7.0 · dsh-composer-history 0.6.2 · dsh-draw 0.2.2 · dsh-talk 0.3.0 · dsh-defend 0.3.0 · dsh-budget 0.4.0 · dsh-library 0.2.1 · @perrylink/dsh-plugin-kit 0.1.2. **mcp-panel 0.6.2 is live on npm via the OIDC Trusted Publishing path.**

---

## 🚀 Flagship picks (start here)

| Plugin | What it gives you | Install |
|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | Second-model auto-review on the approval chain, fail-closed by default (125★) | `dsh plugin --profile web add dsh-auto-review` |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | Approval-gated cross-session memory (`ctx.memory` + SQLite) (79★) | `dsh plugin --profile web add dsh-memento` |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Claude Code-style declarative allow/deny/ask rules with session-log audit (87★) | `dsh plugin --profile web add dsh-permission-rules` |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | MCP management console: `/mcp` + Settings tab + trial calls (52★) | `dsh plugin --profile web add dsh-mcp-panel` |
| [dsh-checkpoint-rewind](https://github.com/PerryLink/dsh-checkpoint-rewind) | Claude Code `/rewind` equivalent: git-first snapshots, session forks, one-shot restore | `dsh plugin --profile web add dsh-checkpoint-rewind` |

One-command starter pack: **[dsh-kit](https://github.com/PerryLink/dsh-kit)** — installs the full family.

## 🔬 Research suite

| Plugin | What it gives you | npm |
|---|---|---|
| [dsh-research-report](https://github.com/PerryLink/dsh-research-report) | Verifiable research reports: content-addressed evidence ledger, manifest seal hash, byte-level citation checks, drift detection, disproof ledger | [npm](https://www.npmjs.com/package/dsh-research-report) |
| [dsh-fund-research](https://github.com/PerryLink/dsh-fund-research) | Chinese mutual-fund research with sealed, traceable snapshots — every number traces to a hashed source | [npm](https://www.npmjs.com/package/dsh-fund-research) |
| [dsh-industry-research](https://github.com/PerryLink/dsh-industry-research) | Industry/company research: chain-map SVG with bottleneck detection, timeline, company cards, adversarial review | [npm](https://www.npmjs.com/package/dsh-industry-research) |
| [dsh-data-quality](https://github.com/PerryLink/dsh-data-quality) | Deterministic data profiling/cleaning/verification: DAMA scorecard, content-hash dedupe, metric expectations | [npm](https://www.npmjs.com/package/dsh-data-quality) |

## 📦 The full family — 34 plugins by pillar

### 🔒 Security (4)

| Plugin | One-liner | npm |
|---|---|---|
| [dsh-defend](https://github.com/PerryLink/dsh-defend) | Injection/jailbreak/secret detection + destructive-delete gate | [npm](https://www.npmjs.com/package/dsh-defend) |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Declarative allow/deny/ask permission rules | [npm](https://www.npmjs.com/package/dsh-permission-rules) |
| [dsh-mask](https://github.com/PerryLink/dsh-mask) | PII masking/sanitization | [npm](https://www.npmjs.com/package/dsh-mask) |
| [dsh-skill-pack-security](https://github.com/PerryLink/dsh-skill-pack-security) | Security-audit skill pack + supply-chain gate | [npm](https://www.npmjs.com/package/@perrylink/dsh-skill-pack-security-provider) |

### 🔁 Workflows (7)

| Plugin | One-liner | npm |
|---|---|---|
| [dsh-background-agents](https://github.com/PerryLink/dsh-background-agents) | Durable background child agents with a Web UI sidebar | [npm](https://www.npmjs.com/package/dsh-background-agents) |
| [dsh-checkpoint-rewind](https://github.com/PerryLink/dsh-checkpoint-rewind) | Snapshots, forks, one-shot restore | [npm](https://www.npmjs.com/package/dsh-checkpoint-rewind) |
| [dsh-github](https://github.com/PerryLink/dsh-github) | GitHub PR/issue integration + Action, writes approval-gated | [npm](https://www.npmjs.com/package/@perrylink/dsh-github) |
| [dsh-claude-move](https://github.com/PerryLink/dsh-claude-move) | Migrate Claude Code/Codex/OpenCode/Hermes into DSH | [npm](https://www.npmjs.com/package/dsh-claude-move) |
| [dsh-click](https://github.com/PerryLink/dsh-click) | Desktop control tools (Windows/macOS) | [npm](https://www.npmjs.com/package/dsh-click) |
| [dsh-session-sync](https://github.com/PerryLink/dsh-session-sync) | Git-backed session synchronization | [npm](https://www.npmjs.com/package/dsh-session-sync) |
| [dsh-test-drive](https://github.com/PerryLink/dsh-test-drive) | Install→smoke→uninstall test driver for plugins | [npm](https://www.npmjs.com/package/dsh-test-drive) |

### ✨ Experience & UX (5)

| Plugin | One-liner | npm |
|---|---|---|
| [dsh-composer-history](https://github.com/PerryLink/dsh-composer-history) | Terminal-style input history for the web composer | [npm](https://www.npmjs.com/package/dsh-composer-history) |
| [dsh-output-styles](https://github.com/PerryLink/dsh-output-styles) | Runtime-switchable model output styles | [npm](https://www.npmjs.com/package/dsh-output-styles) |
| [dsh-session-pin](https://github.com/PerryLink/dsh-session-pin) | Pin sessions in the Web sidebar | [npm](https://www.npmjs.com/package/dsh-session-pin) |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | Approval-gated cross-session memory protocol | [npm](https://www.npmjs.com/package/dsh-memento) |
| [dsh-personal-directive](https://github.com/PerryLink/dsh-personal-directive) | Personal directive injector with top-bar toggle (framework edition; fork of liucaimao2026/dsh-personal-directive, upstream: Minglink/dsh-infinite-gen-1) | — |

### 🧪 Evaluation (3)

| Plugin | One-liner | npm |
|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | Second-model auto-review on the approval chain | [npm](https://www.npmjs.com/package/dsh-auto-review) |
| [dsh-doublecheck](https://github.com/PerryLink/dsh-doublecheck) | Engineering-discipline guard: grill, gates, adversary review | [npm](https://www.npmjs.com/package/dsh-doublecheck) |
| [dsh-score](https://github.com/PerryLink/dsh-score) | Plugin quality scoring across git/gh/npm | [npm](https://www.npmjs.com/package/dsh-score) |

### 📊 Observability & cost (3)

| Plugin | One-liner | npm |
|---|---|---|
| [dsh-budget](https://github.com/PerryLink/dsh-budget) | Token metering and budget governance | [npm](https://www.npmjs.com/package/dsh-budget) |
| [dsh-observe](https://github.com/PerryLink/dsh-observe) | OTel/Langfuse telemetry export | [npm](https://www.npmjs.com/package/dsh-observe) |
| [dsh-fast](https://github.com/PerryLink/dsh-fast) | Performance diagnostics | [npm](https://www.npmjs.com/package/dsh-fast) |

### 🎨 Content & knowledge (5)

| Plugin | One-liner | npm |
|---|---|---|
| [dsh-draw](https://github.com/PerryLink/dsh-draw) | Image-generation routing | [npm](https://www.npmjs.com/package/dsh-draw) |
| [dsh-translate](https://github.com/PerryLink/dsh-translate) | Translation + JSON repair | [npm](https://www.npmjs.com/package/dsh-translate) |
| [dsh-talk](https://github.com/PerryLink/dsh-talk) | Speech recognition and voice I/O | [npm](https://www.npmjs.com/package/dsh-talk) |
| [dsh-library](https://github.com/PerryLink/dsh-library) | Local knowledge-base RAG | [npm](https://www.npmjs.com/package/dsh-library) |
| [dsh-local-ai](https://github.com/PerryLink/dsh-local-ai) | Ollama LLM provider and routing | [npm](https://www.npmjs.com/package/dsh-local-ai) |

### 🛠️ Developer experience (2)

| Plugin | One-liner | npm |
|---|---|---|
| [dsh-lsp-actions](https://github.com/PerryLink/dsh-lsp-actions) | LSP diagnostics/formatting/completion/actions | [npm](https://www.npmjs.com/package/dsh-lsp-actions) |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | MCP management console | [npm](https://www.npmjs.com/package/dsh-mcp-panel) |

*Companion knowledge base:* [dsh-plugin-guide](https://github.com/PerryLink/dsh-plugin-guide) — plugin-development knowledge base + CLI toolchain | [npm](https://www.npmjs.com/package/dsh-plugin-guide)

### 🔬 Research (4)

| Plugin | One-liner | npm |
|---|---|---|
| [dsh-data-quality](https://github.com/PerryLink/dsh-data-quality) | Data profiling/cleaning/verification | [npm](https://www.npmjs.com/package/dsh-data-quality) |
| [dsh-fund-research](https://github.com/PerryLink/dsh-fund-research) | Mutual-fund research, sealed traceable snapshots | [npm](https://www.npmjs.com/package/dsh-fund-research) |
| [dsh-industry-research](https://github.com/PerryLink/dsh-industry-research) | Industry/company research domain pack | [npm](https://www.npmjs.com/package/dsh-industry-research) |
| [dsh-research-report](https://github.com/PerryLink/dsh-research-report) | Verifiable research-report engine | [npm](https://www.npmjs.com/package/dsh-research-report) |

---

## 🌍 Where the plugins live

- **GitHub** (this profile) — source, CI, releases
- **[Gitee](https://gitee.com/perrylink)** — full mirror of every repo's branches and tags
- **npm** — every plugin published with CI provenance

Listed on [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin), [Awesome DeepSeek Harness](https://github.com/0xsline/awesome-deepseek-harness), the [AdamPlatin123 radar](https://github.com/AdamPlatin123/dsh-plugin-radar), and [dsh-market](https://github.com/dsh-market/dsh-market) (via the awesome-dsh-plugin registry). Auto-indexed on [deepseek1024.com](https://deepseek1024.com) (36 entries). Certification: [dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification).

## 中文介绍

我在 DeepSeek Harness 上把 Claude Code / Codex 生态里最实用的能力做成了开源插件:检查点回退、声明式权限、输出风格、跨会话记忆、MCP 面板,以及可验证研究报告 / 基金研究 / 行业研究 / 数据质量「研究四件套」——共 **34 个插件**(Apache-2.0),全部带五语文档、CI、npm 发布与 Gitee 镜像。一键全家桶:[`dsh-kit`](https://github.com/PerryLink/dsh-kit)。

2026-09-01 生态轮:主榜 27 条在线收录,重提 PR 覆盖 fast / session-sync / talk(budget/click/draw 下一轮)、生态榜 PR(radar #440 / Zhiyuan-Fan #59 / Herdeny #3)与官方指南 PR 在审;认证首条落地:dsh-auto-review **B 级**(2026-08-31 快照);npm 通道全解锁:08-30 一天 21 次发布、累计 26 个版本上线 npm(OIDC 直发已验证);供应链 35 仓 Scorecard + provenance + 11 仓品牌声明不变;官方 Showcase 帖 + 37 条社区问答;deepseek1024 自动收录 36 条;家族合计 **603+ 星**、npm 8 月下载 **6.1 万**(近 7 天 2.3 万,Top:mcp-panel/permission-rules/memento)。
