# Hi, I'm PerryLink 👋

[![Gitee mirror](https://img.shields.io/badge/Gitee-mirror-c71d23?logo=gitee)](https://gitee.com/perrylink)
[![DSH Desktop Market](https://img.shields.io/badge/DSH_Desktop_Market-source-0969da)](https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json)
[![npm packages](https://img.shields.io/badge/npm-packages-cb3837?logo=npm)](https://www.npmjs.com/search?q=perrylink)
![plugins](https://img.shields.io/badge/plugins-37-0969da)
![repos](https://img.shields.io/badge/repos-100%2B-green)
![stars](https://img.shields.io/badge/stars-755%2B-yellow)
![npm downloads](https://img.shields.io/badge/npm_downloads-73k%2B_AugSep-cb3837)
[![Certified dsh-auto-review](https://raw.githubusercontent.com/PerryLink/dsh-plugin-certification/main/badges/PerryLink__dsh-auto-review.svg)](https://github.com/PerryLink/dsh-plugin-certification)
[![awesome-dsh-plugin](https://awesome-dsh-plugin.com/badge.svg)](https://awesome-dsh-plugin.com)

**Building the DeepSeek Harness plugin ecosystem: 37 open-source plugins (Apache-2.0) across security, workflows, research, messaging bridges, and developer experience. Every project ships five-language READMEs, CI, npm publishing, and Gitee mirrors — 60.8k npm downloads in August plus 12.3k in the first 4 days of September.**

DeepSeek Harness turned "everything is a plugin" into an ecosystem. I build the plugins I wish existed — engineering-discipline guardrails, runtime panels, cross-session memory, and verifiable research engines — and publish them the way production software deserves.

---

## 📣 Latest — 2026-09-05 round

- **`0.1.3-alpha.1` wave closed (09-04)**: all 39 repos pushed + tagged + GitHub Released, npm publishes verified against the registry, Gitee mirrors re-synced — **449 versions live across 40 npm packages** (35 bare names + 5 scoped). Highlights: `dsh-claude-move 0.4.1` (dual-baseline handle shim, 236 tests) · `dsh-composer-history 0.7.0` (273 tests) · `dsh-permission-rules 0.6.10` · `dsh-auto-review 0.10.3` · `dsh-memento 0.5.5` · `dsh-session-pin 0.7.4`. 34 profile plugins re-validated end-to-end (D2 smoke v4 matrix).
- **New family members**: [dsh-wechat](https://github.com/PerryLink/dsh-wechat) — WeChat ↔ DSH bridge over the Tencent iLink bot protocol (text/image/file/voice, approval cards in chat; npm 0.8.0) · [dsh-ticktick](https://github.com/PerryLink/dsh-ticktick) — TickTick/Dida365 task bridge (`@perrylink/dsh-ticktick`, scoped after the bare name was taken) · [dsh-reach](https://github.com/PerryLink/dsh-reach) — multi-channel approval/question bridge (WeChat/Telegram/Feishu). Support repos: [dsh-catalog](https://github.com/PerryLink/dsh-catalog) (Market catalog source) + [dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) (certification MCP server).
- **Routine community audit (A-class mode 1, 09-04/05)**: 84-repo enumeration, every issue / PR / discussion thread checked per-thread — **zero unanswered community threads**; Discussions enabled on 23 repos (the 5 new product repos + 18 tool repos); metadata/badge fixes across 10 repos. [permission-rules AST command decomposition](https://github.com/PerryLink/dsh-permission-rules/issues/8) now **officially scheduled** (design = [discussion #10](https://github.com/PerryLink/dsh-permission-rules/discussions/10), fail-closed first); research-report #2 closed.
- **DSH Desktop Market**: the standard catalog source is live at [`perrylink-dsh-catalog.perrylink.workers.dev`](https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json) — now **36 packages** with curated summaries and same-origin icons, contract-validated and live-smoked by CI on every deploy. In DSH Desktop: **Market → Sources → add source → paste the `catalog-source.json` URL**.
- **Registry sprint**: **35 entries live** on [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) · omdsh hub: **113 [Submission] issues** filed · ecosystem PRs still open: official [awesome-deepseek-agent #410](https://github.com/deepseek-ai/awesome-deepseek-agent/pull/410), [Zhiyuan-Fan #59](https://github.com/Zhiyuan-Fan/Awesome-DeepSeek-Harness-Plugins/pull/59), [Herdeny #3](https://github.com/Herdeny/awesome-dsh-plugins-2026/pull/3), [AEI #732](https://github.com/deepseek-ai/awesome-deepseek-integration/pull/732).
- **W5 article published**: the full Chinese deep-dive on `dsh-auto-review` is live on the official Showcase post [#5016](https://github.com/deepseek-ai/deepseek-harness/discussions/5016) (second-model approval design, fail-closed chains, audit trail).
- **Adoption (2026-09-05 snapshot)**: **755★** across the family's 40 repos · topic top-100 threshold now **556** · **60.8k npm downloads in August** + **12.3k in Sep 1–4** (rolling-30d ≈ 60.4k) — top by downloads: dsh-wechat 5.0k · dsh-mcp-panel 3.6k · dsh-permission-rules 2.9k · dsh-memento 2.7k · dsh-checkpoint-rewind 2.6k. Per-package live badges on each repo.
- **Gitee mirrors**: **99 public repos** (verified via the public API; daily auto-sync via the `gitee-sync` workflow).
- Full audit (2026-08-27): 33/33 install · load · keyless-boot · uninstall — all green.
- **Supply chain**: OpenSSF Scorecard CI on all 40 repos (v2.4.4, green) · npm provenance on every publish · `funding` links and the 1024-store install channel on every README.
- **Certification**: [dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification) spec v1 published — five machine-checkable dimensions, A–D grades, independent registry + badges · **first registry entry live: dsh-auto-review Grade B** (snapshot: 0.10.0 · 276 tests · provenance) · proposal posted on the official security-audit discussion [#454](https://github.com/deepseek-ai/deepseek-harness/discussions/454).
- **Community**: **92 answered questions** across GitHub discussions (58 on the official repo) · community PR merged: dsh-memento #8 · 36 entries auto-listed on [deepseek1024.com](https://deepseek1024.com).

---

## 🚀 Flagship picks (start here)

| Plugin | What it gives you | Install |
|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | Second-model auto-review on the approval chain, fail-closed by default (134★) | `dsh plugin --profile web add dsh-auto-review` |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Claude Code-style declarative allow/deny/ask rules with session-log audit (113★) | `dsh plugin --profile web add dsh-permission-rules` |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | Approval-gated cross-session memory (`ctx.memory` + SQLite) (95★) | `dsh plugin --profile web add dsh-memento` |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | MCP management console: `/mcp` + Settings tab + trial calls (52★) | `dsh plugin --profile web add dsh-mcp-panel` |
| [dsh-checkpoint-rewind](https://github.com/PerryLink/dsh-checkpoint-rewind) | Claude Code `/rewind` equivalent: git-first snapshots, session forks, one-shot restore (15★) | `dsh plugin --profile web add dsh-checkpoint-rewind` |

One-command starter pack: **[dsh-kit](https://github.com/PerryLink/dsh-kit)** — installs the full 37-plugin family.

## 🔬 Research suite

| Plugin | What it gives you | npm |
|---|---|---|
| [dsh-research-report](https://github.com/PerryLink/dsh-research-report) | Verifiable research reports: content-addressed evidence ledger, manifest seal hash, byte-level citation checks, drift detection, disproof ledger | [npm](https://www.npmjs.com/package/dsh-research-report) |
| [dsh-fund-research](https://github.com/PerryLink/dsh-fund-research) | Chinese mutual-fund research with sealed, traceable snapshots — every number traces to a hashed source | [npm](https://www.npmjs.com/package/dsh-fund-research) |
| [dsh-industry-research](https://github.com/PerryLink/dsh-industry-research) | Industry/company research: chain-map SVG with bottleneck detection, timeline, company cards, adversarial review | [npm](https://www.npmjs.com/package/dsh-industry-research) |
| [dsh-data-quality](https://github.com/PerryLink/dsh-data-quality) | Deterministic data profiling/cleaning/verification: DAMA scorecard, content-hash dedupe, metric expectations | [npm](https://www.npmjs.com/package/dsh-data-quality) |

## 📦 The full family — 37 plugins by pillar

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
| [dsh-personal-directive](https://github.com/PerryLink/dsh-personal-directive) | Personal directive injector with top-bar toggle (framework edition; fork of liucaimao2026/dsh-personal-directive) | [npm](https://www.npmjs.com/package/dsh-personal-directive) |

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

### 🛠️ Developer experience (3)

| Plugin | One-liner | npm |
|---|---|---|
| [dsh-lsp-actions](https://github.com/PerryLink/dsh-lsp-actions) | LSP diagnostics/formatting/completion/actions | [npm](https://www.npmjs.com/package/dsh-lsp-actions) |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | MCP management console | [npm](https://www.npmjs.com/package/dsh-mcp-panel) |
| [dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) | Read-only MCP server over the certification registry | [npm](https://www.npmjs.com/package/@perrylink/dsh-cert-mcp) |

*Companion knowledge base:* [dsh-plugin-guide](https://github.com/PerryLink/dsh-plugin-guide) — plugin-development knowledge base + CLI toolchain | [npm](https://www.npmjs.com/package/dsh-plugin-guide)

### 📱 Messaging & bridges (3)

| Plugin | One-liner | npm |
|---|---|---|
| [dsh-wechat](https://github.com/PerryLink/dsh-wechat) | WeChat ↔ DSH bridge (Tencent iLink bot): text/image/file/voice, approvals in chat | [npm](https://www.npmjs.com/package/dsh-wechat) |
| [dsh-ticktick](https://github.com/PerryLink/dsh-ticktick) | TickTick/Dida365 task bridge: session-header panel + 11 tools | [npm](https://www.npmjs.com/package/@perrylink/dsh-ticktick) |
| [dsh-reach](https://github.com/PerryLink/dsh-reach) | Multi-channel approval/question bridge: WeChat/Telegram/Feishu, session console | [npm](https://www.npmjs.com/package/dsh-reach) |

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
- **[Gitee](https://gitee.com/perrylink)** — full mirror of every repo's branches and tags (99 public repos)
- **npm** — 40 packages published with CI provenance (449 versions)
- **DSH Desktop Market** — add the catalog source `https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json` under Market → Sources to browse all 36 family packages in-app (curated summaries + icons, contract-validated, CI-smoked)

Listed on [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) (35 entries), [Awesome DeepSeek Harness](https://github.com/0xsline/awesome-deepseek-harness), the [AdamPlatin123 radar](https://github.com/AdamPlatin123/dsh-plugin-radar), and [dsh-market](https://github.com/dsh-market/dsh-market) (via the awesome-dsh-plugin registry). Auto-indexed on [deepseek1024.com](https://deepseek1024.com) (36 entries). Certification: [dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification).

## 中文介绍

我在 DeepSeek Harness 上把 Claude Code / Codex 生态里最实用的能力做成了开源插件:检查点回退、声明式权限、输出风格、跨会话记忆、MCP 面板、微信/TickTick 桥接,以及可验证研究报告 / 基金研究 / 行业研究 / 数据质量「研究四件套」——共 **37 个插件**(Apache-2.0),全部带五语文档、CI、npm 发布与 Gitee 镜像。一键全家桶:[`dsh-kit`](https://github.com/PerryLink/dsh-kit)。

2026-09-05 轮:① **0.1.3-alpha.1 波次闭环**——39 仓 GitHub 推送+tag+Release、npm 发布 registry 全量核验、Gitee 镜像同步,全家桶 **40 个 npm 包累计 449 版本**(35 裸名 + 5 scoped);② **三个新成员上架**——dsh-wechat(微信桥接,npm 0.8.0)、@perrylink/dsh-ticktick(滴答清单桥接,scoped 命名决策已落地)、dsh-reach(多渠道审批桥);③ **例行社区盘点(A 类模式 1)**——84 仓枚举、全部 issue/PR/讨论线程逐条判定,**未回复 0 条**;23 仓开启 Discussions;permission-rules AST 命令分解正式排期(设计=discussion #10,fail-closed 优先);④ **收录推进**——awesome-dsh-plugin 主榜 **35 条**、omdsh hub [Submission] 累计 **113 条**、DSH Desktop 市场目录源 **36 项**;⑤ 家族 **755+ 星**;npm 8 月 **6.1 万** + 9 月前四日 **1.2 万**(滚动 30 天 6.0 万);Gitee **99 公开仓**;认证 auto-review B 级;官方仓 58 条、全 GitHub **92 条**问答;deepseek1024 自动收录 36 条。

近期需要安排一次体检，为减少熬夜，后续的更新迭代节奏会适当放缓——问题和缺陷修复不会停，只是发布频率会降低一些，还请大家谅解。
