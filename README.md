# Hi, I'm PerryLink 👋

[![Gitee mirror](https://img.shields.io/badge/Gitee-mirror-c71d23?logo=gitee)](https://gitee.com/perrylink)
[![DSH Desktop Market](https://img.shields.io/badge/DSH_Desktop_Market-source-0969da)](https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json)
[![npm packages](https://img.shields.io/badge/npm-packages-cb3837?logo=npm)](https://www.npmjs.com/search?q=perrylink)
![plugins](https://img.shields.io/badge/plugins-37-0969da)
![repos](https://img.shields.io/badge/repos-100%2B-green)
![stars](https://img.shields.io/badge/stars-770%2B-yellow)
![npm downloads](https://img.shields.io/badge/npm_downloads-82k%2B_AugSep-cb3837)
[![Certified dsh-auto-review](https://raw.githubusercontent.com/PerryLink/dsh-plugin-certification/main/badges/PerryLink__dsh-auto-review.svg)](https://github.com/PerryLink/dsh-plugin-certification)
[![awesome-dsh-plugin](https://awesome-dsh-plugin.com/badge.svg)](https://awesome-dsh-plugin.com)

**Building the DeepSeek Harness plugin ecosystem: 37 open-source plugins (Apache-2.0) across security, workflows, research, messaging bridges, and developer experience — plus the DSH Desktop Market catalog and a plugin-certification registry. Every project ships five-language READMEs, CI, npm provenance, and Gitee mirrors — 60.8k npm downloads in August plus 21.5k in the first 5 days of September.**

DeepSeek Harness turned "everything is a plugin" into an ecosystem. I build the plugins I wish existed — engineering-discipline guardrails, runtime panels, cross-session memory, and verifiable research engines — and publish them the way production software deserves.

---

## 📣 Latest — 2026-09-06 round

- **Cordis upstream** (the framework layer, 8.1k★): reported the `applyPatches` insert-index bug as [issue #112](https://github.com/cordiverse/cordis/issues/112) → core maintainer **shigma opened PR [#121](https://github.com/cordiverse/cordis/pull/121)** with an architecture-level journal fix (**Fixes #112**, supersedes my PR [#116](https://github.com/cordiverse/cordis/pull/116) — now closed as superseded) · opened PR **[#122](https://github.com/cordiverse/cordis/pull/122)** `ci: test on Windows` with node 22/24/26 all-green evidence · offered a **45-patch downstream semantic regression suite** for #121 · first errata batch for the [Cordis paper](https://arxiv.org/abs/2608.25512): 18 verified items, author-email draft ready · rc.9 compatibility matrix: 43/45 family patches pass against upstream.
- **`0.1.2-rc.1` stabilization**: found and fixed a family-wide peer-range defect — `>=0.1.0-rc.8 <0.2.0` silently matched only one prerelease under npm's prerelease-tuple rules — rolled **`>=0.1.2-rc.1 <0.2.0`** across 35 repos and republished **`dsh-auto-review 0.10.4`** (bare-install verified) · `dsh-background-agents` CI repinned to the 0.1.3-alpha.1 master seam · **all 35 plugin-repo CI suites green** · five-language READMEs re-synced in 12 repos (peer ranges, market notes on the new repos).
- **DSH Desktop Market**: catalog now lists **37 packages** — `dsh-reach` added and 9 curated summaries refreshed against current features (composer-history / fast / click / draw / library / budget / defend / data-quality / output-styles); deploy workflow live-smoke green.
- **Ecosystem listings**: **36 entries** on [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) · omdsh hub: **112 open [Submission] entries** (the hub's intake pipeline has been broken since 08-31 — I filed the root-cause diagnosis [issue #166](https://github.com/omdsh-dev/dsh-hub-workshop/issues/166) and paused resubmission until it is fixed) · radar [#674](https://github.com/AdamPlatin123/dsh-plugin-radar/pull/674) **merged** · whalehub: 38 entries ingested · [dsh-handbook](https://github.com/Electricitysheep/dsh-handbook) PR [#67](https://github.com/Electricitysheep/dsh-handbook/pull/67) (15 chapters zh/en) · [pan17/dsh-wechat PR #4](https://github.com/pan17/dsh-wechat/pull/4): cross-session waterfall port, 384/384 tests, awaiting maintainer CI approval.
- **dsh-cert-mcp on Glama**: published with an **A-grade TDQS 3.64** (three tools: get_certification / list_certified / certification_spec) · [punkpeye PR #13535](https://github.com/punkpeye/awesome-mcp-servers/pull/13535) in final maintainer review.
- **Community hygiene**: 34 mojibake posts across GitHub repaired in place with apologies + readable replacements (posting charset discipline now codified in the prompt library) · **zero unanswered community threads** maintained · 23 repos have Discussions enabled.
- **Adoption (2026-09-06 snapshot)**: **770★** across the family's 40 repos (up from 755) · **449 versions live across 39 npm packages** (34 bare + 5 scoped — the bare `dsh-ticktick` name belongs to another account, so the family's TickTick package is scoped) · **60.8k npm downloads in August** + **21.5k in Sep 1–5** (rolling-30d ≈ 61.9k) — top by downloads: dsh-wechat 5.0k · dsh-mcp-panel 3.6k · dsh-permission-rules 2.9k · dsh-memento 2.7k · dsh-checkpoint-rewind 2.6k · topic:dsh-plugin top-100 threshold now **558** · **99 public Gitee mirrors** · 36 entries auto-listed on deepseek1024.com.
- **Certification**: [dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification) spec v1 — five machine-checkable dimensions, A–D grades, registry + badges · **dsh-auto-review Grade B** live · proposal on the official discussion [#454](https://github.com/deepseek-ai/deepseek-harness/discussions/454).

---

## 🚀 Flagship picks (start here)

| Plugin | What it gives you | Install |
|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | Second-model auto-review on the approval chain, fail-closed by default (136★) | `dsh plugin --profile web add dsh-auto-review` |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Claude Code-style declarative allow/deny/ask rules with session-log audit (113★) | `dsh plugin --profile web add dsh-permission-rules` |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | Approval-gated cross-session memory (`ctx.memory` + SQLite) (97★) | `dsh plugin --profile web add dsh-memento` |
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
- **npm** — 39 packages published with CI provenance (449 versions)
- **DSH Desktop Market** — add the catalog source `https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json` under Market → Sources to browse all 37 family packages in-app (curated summaries + icons, contract-validated, CI-smoked)

Listed on [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) (36 entries), [Awesome DeepSeek Harness](https://github.com/0xsline/awesome-deepseek-harness), the [AdamPlatin123 radar](https://github.com/AdamPlatin123/dsh-plugin-radar), and [dsh-market](https://github.com/dsh-market/dsh-market) (via the awesome-dsh-plugin registry). Auto-indexed on [deepseek1024.com](https://deepseek1024.com) (36 entries). Certification: [dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification).

## 中文介绍

我在 DeepSeek Harness 上把 Claude Code / Codex 生态里最实用的能力做成了开源插件:检查点回退、声明式权限、输出风格、跨会话记忆、MCP 面板、微信/TickTick 桥接,以及可验证研究报告 / 基金研究 / 行业研究 / 数据质量「研究四件套」——共 **37 个插件**(Apache-2.0),全部带五语文档、CI、npm 发布与 Gitee 镜像。一键全家桶:[`dsh-kit`](https://github.com/PerryLink/dsh-kit)。

2026-09-06 轮:① **Cordis 上游贡献**——报告的 applyPatches 插入索引 bug(#112)被维护者以架构级 journal 修复 PR #121 收口(Fixes #112,我们的 #116 已按 supersede 关闭),Windows CI PR #122 在途,论文勘误 18 条就绪,rc.9 兼容矩阵 43/45 通过;② **rc.1 稳定化**——全家桶 peer 范围缺陷(旧范围裸解析只匹配一个预发布版)在 35 仓批量修复,`dsh-auto-review 0.10.4` 重发,bg-agents CI 转绿,**35 插件仓 CI 全绿**;12 仓五语 README 同步;③ **市场目录 37 项**——dsh-reach 入列 + 9 条策展摘要按现行功能刷新,部署 CI live smoke 通过;④ **收录推进**——awesome-dsh-plugin 主榜 **36 条**、omdsh hub 开放投稿 **112 条**(hub intake 管线故障已提交诊断 #166,暂停重投)、whalehub 38 条、dsh-handbook PR #67、pan17/dsh-wechat PR #4(384/384 测试);⑤ **cert-mcp 上 Glama**——TDQS 3.64 = A 级,punkpeye 终审中;⑥ 乱码修复 34 处 + 道歉;未回复社区帖保持 **0**;⑦ 家族 **770+ 星**;npm 8 月 **6.1 万** + 9 月 1–5 日 **2.1 万**(滚动 30 天 6.2 万);Gitee **99 公开仓**;认证 auto-review B 级;deepseek1024 自动收录 36 条。

近期需要安排一次体检，为减少熬夜，后续的更新迭代节奏会适当放缓——问题和缺陷修复不会停，只是发布频率会降低一些，还请大家谅解。
