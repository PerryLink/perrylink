# Hi, I'm PerryLink 👋

[![Gitee mirror](https://img.shields.io/badge/Gitee-mirror-c71d23?logo=gitee)](https://gitee.com/perrylink)
[![DSH Desktop Market](https://img.shields.io/badge/DSH_Desktop_Market-source-0969da)](https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json)
[![npm packages](https://img.shields.io/badge/npm-packages-cb3837?logo=npm)](https://www.npmjs.com/search?q=perrylink)
![plugins](https://img.shields.io/badge/plugins-34-0969da)
![repos](https://img.shields.io/badge/repos-100%2B-green)
![stars](https://img.shields.io/badge/stars-710%2B-yellow)
![npm downloads](https://img.shields.io/badge/npm_downloads-72k%2B_AugSep-cb3837)
[![Certified dsh-auto-review](https://raw.githubusercontent.com/PerryLink/dsh-plugin-certification/main/badges/PerryLink__dsh-auto-review.svg)](https://github.com/PerryLink/dsh-plugin-certification)
[![awesome-dsh-plugin](https://awesome-dsh-plugin.com/badge.svg)](https://awesome-dsh-plugin.com)

**Building the DeepSeek Harness plugin ecosystem: 34 open-source plugins (Apache-2.0) across security, workflows, research, and developer experience. Every project ships five-language READMEs, CI, npm publishing, and Gitee mirrors — 60.8k npm downloads in August plus 11.9k in the first 3 days of September.**

DeepSeek Harness turned "everything is a plugin" into an ecosystem. I build the plugins I wish existed — engineering-discipline guardrails, runtime panels, cross-session memory, and verifiable research engines — and publish them the way production software deserves.

---

## 📣 Latest — 2026-09-04 round

- **Ecosystem outreach wave** (last night's execution): PR [#732](https://github.com/deepseek-ai/awesome-deepseek-integration/pull/732) filed on the 39k★ official `awesome-deepseek-integration` (harness section) · friend-link request [#798](https://github.com/anywhere-labs/dsh-desktop/issues/798) + Fabric RFC discussion [**#799**](https://github.com/anywhere-labs/dsh-desktop/discussions/799) on dsh-desktop · listing issues [#41](https://github.com/vvlife/whalehub-dsh/issues/41)–44 (whalehub) · [#100](https://github.com/libukai/awesome-deepseek-harness/issues/100) (libukai) · PR [#109](https://github.com/Alex-Yanggg/awesome-DSH-plugin/pull/109) (Alex-Yanggg) — all verified open · [`FUNDING.yml`](https://github.com/PerryLink/.github) now live (GitHub Sponsors ready).
- **DSH Desktop Market**: the PerryLink **standard catalog source is live** at [`perrylink-dsh-catalog.perrylink.workers.dev`](https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json) — all **34 packages** with curated English summaries and same-origin icons, validated against the public v1 provider contract and live-smoked by CI on every deploy. In DSH Desktop: **Market → Sources → add source → paste the `catalog-source.json` URL** to browse the whole family in-app (installation still goes through the Market's npm-identity verification). A five-language "Install from the DSH Desktop Market" note shipped to all **33 npm-published plugin repos**.
- **W5 article published**: the full Chinese deep-dive on `dsh-auto-review` is live on the official Showcase post [#5016](https://github.com/deepseek-ai/deepseek-harness/discussions/5016) (second-model approval design, fail-closed chains, audit trail).
- **Registry sprint**: **31 entries live** on [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) — PR [#4175](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin/pull/4175) **merged** (dsh-budget / dsh-click / dsh-draw / dsh-plugin-kit added); #4176 closed per the one-plugin-per-maintainer preference · ecosystem PRs: [AdamPlatin123 radar #440](https://github.com/AdamPlatin123/dsh-plugin-radar/pull/440) **merged 08-31** · [Zhiyuan-Fan #59](https://github.com/Zhiyuan-Fan/Awesome-DeepSeek-Harness-Plugins/pull/59) · [Herdeny #3](https://github.com/Herdeny/awesome-dsh-plugins-2026/pull/3) · official [DeepSeek Harness guide PR](https://github.com/deepseek-ai/awesome-deepseek-agent/pull/410) · omdsh hub: **76 [Submission] issues** filed (latest batch [#93–#124](https://github.com/omdsh-dev/dsh-hub-workshop/issues)).
- **Brand protection**: official-repository declaration merged into 11 repos (same-name repository defense, including the 68-star name collision on dsh-github).
- **Adoption (2026-09-04 snapshot)**: **710★** across the 34 plugin repos (up from 701 last night; topic top-100 threshold now **548**) · **60.8k npm downloads in August** + **11.9k in Sep 1–3** (Sep 4 not yet in npm's daily stats) — top by downloads: dsh-mcp-panel 3.9k · dsh-permission-rules 3.1k · dsh-memento 2.8k · dsh-checkpoint-rewind 2.7k · dsh-auto-review 2.7k · dsh-lsp-actions 2.5k. Per-package live badges on each repo.
- **Gitee mirrors**: **97 public repos** (verified via the public API; 4 new mirrors — personal-directive / reach / catalog / cert-mcp — opened and filled; daily auto-sync via the `gitee-sync` workflow).
- Full audit (2026-08-27): 33/33 install · load · keyless-boot · uninstall — all green.
- **Supply chain**: OpenSSF Scorecard CI on all 35 repos (action upgraded to v2.4.4 — upstream gcr.io billing failure cleared, green again) · npm provenance on every publish · `funding` links and the 1024-store install channel on every README.
- **Certification**: [dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification) spec v1 published — five machine-checkable dimensions, A–D grades, independent registry + badges · **first registry entry live: dsh-auto-review Grade B** (refreshed 2026-09-02 snapshot: 0.10.0 · 276 tests · provenance) · proposal posted on the official security-audit discussion [#454](https://github.com/deepseek-ai/deepseek-harness/discussions/454).
- **Community**: official [Showcase post #5016](https://github.com/deepseek-ai/deepseek-harness/discussions/5016) now carries the published article · **92 answered questions** across GitHub discussions (58 on the official repo) · community PR merged: dsh-memento #8 · 36 entries auto-listed on [deepseek1024.com](https://deepseek1024.com).
- **New releases**: **0.1.2-alpha.5 wave landed on 09-02** — 34 repos pushed + tagged + GitHub Released, 33 npm publishes plus a 22-package docs-patch follow-up wave (23/23 released), 2× Gitee sync (both success) · **366 versions live across 34 published plugin packages** (registry count; `dsh-personal-directive@0.2.1` shipped 09-03 11:03Z with provenance — the family's 34th plugin package) · plus **`@perrylink/dsh-cert-mcp@0.1.1`** (the certification MCP server, published 09-03 16:28Z) — **35 npm packages** across the family. Latest: dsh-auto-review 0.10.1 · dsh-doublecheck 0.9.4 · dsh-mcp-panel 0.6.5 · dsh-permission-rules 0.6.8 · dsh-memento 0.5.3 · dsh-session-pin 0.7.3 · dsh-personal-directive 0.2.1. · official **MCP Registry** metadata for dsh-cert-mcp validated (2025-12-11 schema + stdio) — publish pending device login.

---

## 🚀 Flagship picks (start here)

| Plugin | What it gives you | Install |
|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | Second-model auto-review on the approval chain, fail-closed by default (131★) | `dsh plugin --profile web add dsh-auto-review` |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | Approval-gated cross-session memory (`ctx.memory` + SQLite) (87★) | `dsh plugin --profile web add dsh-memento` |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Claude Code-style declarative allow/deny/ask rules with session-log audit (109★) | `dsh plugin --profile web add dsh-permission-rules` |
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
| [dsh-personal-directive](https://github.com/PerryLink/dsh-personal-directive) | Personal directive injector with top-bar toggle (framework edition; fork of liucaimao2026/dsh-personal-directive, upstream: Minglink/dsh-infinite-gen-1) | [npm](https://www.npmjs.com/package/dsh-personal-directive) |

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
- **[Gitee](https://gitee.com/perrylink)** — full mirror of every repo's branches and tags (97 public repos)
- **npm** — every plugin published with CI provenance (34 packages)
- **DSH Desktop Market** — add the catalog source `https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json` under Market → Sources to browse all 34 plugins in-app (curated summaries + icons, contract-validated, CI-smoked)

Listed on [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin), [Awesome DeepSeek Harness](https://github.com/0xsline/awesome-deepseek-harness), the [AdamPlatin123 radar](https://github.com/AdamPlatin123/dsh-plugin-radar), and [dsh-market](https://github.com/dsh-market/dsh-market) (via the awesome-dsh-plugin registry). Auto-indexed on [deepseek1024.com](https://deepseek1024.com) (36 entries). Certification: [dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification).

## 中文介绍

我在 DeepSeek Harness 上把 Claude Code / Codex 生态里最实用的能力做成了开源插件:检查点回退、声明式权限、输出风格、跨会话记忆、MCP 面板,以及可验证研究报告 / 基金研究 / 行业研究 / 数据质量「研究四件套」——共 **34 个插件**(Apache-2.0),全部带五语文档、CI、npm 发布与 Gitee 镜像。一键全家桶:[`dsh-kit`](https://github.com/PerryLink/dsh-kit)。

2026-09-04 生态轮:① **生态收录波落地**——39k★ 官方 awesome-deepseek-integration PR [#732](https://github.com/deepseek-ai/awesome-deepseek-integration/pull/732)、dsh-desktop 友情链接 issue [#798](https://github.com/anywhere-labs/dsh-desktop/issues/798) + Fabric RFC 讨论、whalehub [#41](https://github.com/vvlife/whalehub-dsh/issues/41)–44、libukai [#100](https://github.com/libukai/awesome-deepseek-harness/issues/100)、Alex-Yanggg PR [#109](https://github.com/Alex-Yanggg/awesome-DSH-plugin/pull/109) 全部实测 open;`FUNDING.yml` 上线(GitHub Sponsors 就绪);② **主榜 31 条**——PR #4175 已合并(budget/click/draw/plugin-kit 进榜),#4176 关闭;omdsh [Submission] 累计 **76 条**;③ **DSH Desktop 市场目录源在线**(34 包 + 同源图标,CI 实测),33 仓 README 五语市场指引;W5 文章已发布于官方 Showcase #5016;④ **@perrylink/dsh-cert-mcp@0.1.1 上架**(认证体系 MCP server,09-03 16:28Z)——全家桶 npm 包达 **35 个**,34 插件包累计 **366 版本**(registry 实测);⑤ 家族 **710+ 星**(昨晚 701 起续涨);npm 8 月 **6.1 万** + 9 月前三日 **1.2 万**;Gitee **97 公开仓**;认证 auto-review B 级不变;官方仓 58 条、全 GitHub **92 条**问答;deepseek1024 自动收录 36 条。

近期需要安排一次体检，为减少熬夜，后续的更新迭代节奏会适当放缓——问题和缺陷修复不会停，只是发布频率会降低一些，还请大家谅解。
