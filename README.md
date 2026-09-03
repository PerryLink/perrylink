# Hi, I'm PerryLink 👋

[![Gitee mirror](https://img.shields.io/badge/Gitee-mirror-c71d23?logo=gitee)](https://gitee.com/perrylink)
[![npm packages](https://img.shields.io/badge/npm-packages-cb3837?logo=npm)](https://www.npmjs.com/search?q=perrylink)
![plugins](https://img.shields.io/badge/plugins-34-0969da)
![repos](https://img.shields.io/badge/repos-100%2B-green)
![stars](https://img.shields.io/badge/stars-680%2B-yellow)
![npm downloads](https://img.shields.io/badge/npm_downloads-60k%2FAug-cb3837)

**Building the DeepSeek Harness plugin ecosystem: 34 open-source plugins (Apache-2.0) across security, workflows, research, and developer experience. Every project ships five-language READMEs, CI, npm publishing, and Gitee mirrors — 60k+ npm downloads in August across the family.**

DeepSeek Harness turned "everything is a plugin" into an ecosystem. I build the plugins I wish existed — engineering-discipline guardrails, runtime panels, cross-session memory, and verifiable research engines — and publish them the way production software deserves.

---

## 📣 Latest — 2026-09-03 ecosystem round

- **Registry sprint**: 27 entries live on [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) · new PRs [#4175](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin/pull/4175)/[#4176](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin/pull/4176) adding dsh-budget / dsh-click / dsh-draw / dsh-plugin-kit (re-submission PRs for dsh-fast / dsh-session-sync / dsh-talk still open) · ecosystem PRs: [AdamPlatin123 radar #440](https://github.com/AdamPlatin123/dsh-plugin-radar/pull/440) **merged 08-31** · [Zhiyuan-Fan #59](https://github.com/Zhiyuan-Fan/Awesome-DeepSeek-Harness-Plugins/pull/59) · [Herdeny #3](https://github.com/Herdeny/awesome-dsh-plugins-2026/pull/3) · official [DeepSeek Harness guide PR](https://github.com/deepseek-ai/awesome-deepseek-agent/pull/410) on awesome-deepseek-agent · omdsh hub: 31 [Submission] issues filed ([#94–#124](https://github.com/omdsh-dev/dsh-hub-workshop/issues)).
- **Brand protection**: official-repository declaration merged into 11 repos (same-name repository defense, including the 68-star name collision on dsh-github).
- **Adoption (2026-09-03 snapshot)**: **680★** across 35 repos (up from 643 on 09-02; topic top-100 threshold now **548**) · **60.8k npm downloads in August** (September rolling in — 2.9k on Sep 1; npm daily stats lag) — top by downloads: dsh-mcp-panel 3.9k · dsh-permission-rules 3.1k · dsh-memento 2.8k · dsh-checkpoint-rewind 2.7k · dsh-auto-review 2.7k · dsh-lsp-actions 2.5k. Per-package live badges on each repo.
- Full audit (2026-08-27): 33/33 install · load · keyless-boot · uninstall — all green.
- **Supply chain**: OpenSSF Scorecard CI on all 35 repos (action upgraded to v2.4.4 — upstream gcr.io billing failure cleared, green again) · npm provenance on every publish · `funding` links and the 1024-store install channel on every README.
- **Certification**: [dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification) spec v1 published — five machine-checkable dimensions, A–D grades, independent registry + badges · **first registry entry live: dsh-auto-review Grade B** (refreshed 2026-09-02 snapshot: 0.10.0 · 276 tests · provenance) · proposal posted on the official security-audit discussion [#454](https://github.com/deepseek-ai/deepseek-harness/discussions/454).
- **Community**: official [Showcase post](https://github.com/deepseek-ai/deepseek-harness/discussions/5016) updated for the alpha.5 wave · **92 answered questions** across GitHub discussions (58 on the official repo) · community PR merged today: dsh-memento #8 · 36 entries auto-listed on [deepseek1024.com](https://deepseek1024.com).
- **New releases**: **0.1.2-alpha.5 wave landed on 09-02** — 34 repos pushed + tagged + GitHub Released, 33 npm publishes plus a 22-package docs-patch follow-up wave (23/23 released), 2× Gitee sync (both success) · **351 versions live across 33 published packages** (116 shipped since the 08-30 npm unlock). Latest: dsh-auto-review 0.10.1 · dsh-doublecheck 0.9.4 · dsh-mcp-panel 0.6.5 · dsh-permission-rules 0.6.8 (today: #13 watcher fix) · dsh-memento 0.5.3 · dsh-session-pin 0.7.3. dsh-library 0.2.3 live (search-scoring fix).

---

## 🚀 Flagship picks (start here)

| Plugin | What it gives you | Install |
|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | Second-model auto-review on the approval chain, fail-closed by default (130★) | `dsh plugin --profile web add dsh-auto-review` |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | Approval-gated cross-session memory (`ctx.memory` + SQLite) (85★) | `dsh plugin --profile web add dsh-memento` |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Claude Code-style declarative allow/deny/ask rules with session-log audit (104★) | `dsh plugin --profile web add dsh-permission-rules` |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | MCP management console: `/mcp` + Settings tab + trial calls (53★) | `dsh plugin --profile web add dsh-mcp-panel` |
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

2026-09-03 生态轮:0.1.2-alpha.5 全量波 09-02 落地——34 仓推送+tag+Release、33 次 npm 发布 + 22 包文档 patch 次波(23/23 Release)、Gitee 两轮同步均 success,33 个已发布包累计 **351 个版本**(自 08-30 解锁以来 116 版;最新 auto-review 0.10.1 / doublecheck 0.9.4 / mcp-panel 0.6.5 / permission-rules 0.6.8);今日另修 permission-rules #13 并发布 0.6.8、合并社区 PR memento #8;家族合计 **680+ 星**(门槛升至 548);npm 8 月下载 **6.1 万**(9 月滚动中,9/1 = 2.9k);主榜 27 条 + 新 PR #4175/#4176 再添 budget/click/draw/plugin-kit;认证 auto-review B 级快照刷新至 09-02(0.10.0);官方仓 58 条、全 GitHub **92 条**问答;deepseek1024 自动收录 36 条。
