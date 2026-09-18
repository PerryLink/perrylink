# Hi, I'm PerryLink 👋

[![Gitee mirror](https://img.shields.io/badge/Gitee-mirror-c71d23?logo=gitee)](https://gitee.com/perrylink)
[![DSH Desktop Market](https://img.shields.io/badge/DSH_Desktop_Market-source-0969da)](https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json)
[![npm packages](https://img.shields.io/badge/npm-packages-cb3837?logo=npm)](https://www.npmjs.com/search?q=perrylink)
![plugins](https://img.shields.io/badge/plugins-40-0969da)
![repos](https://img.shields.io/badge/repos-147-green)
![stars](https://img.shields.io/badge/stars-1060-yellow)
![npm downloads](https://img.shields.io/badge/npm_downloads-129k_30d-cb3837)
[![Certified dsh-auto-review](https://raw.githubusercontent.com/PerryLink/dsh-plugin-certification/main/badges/PerryLink__dsh-auto-review.svg)](https://github.com/PerryLink/dsh-plugin-certification)
[![awesome-dsh-plugin](https://awesome-dsh-plugin.com/badge.svg)](https://awesome-dsh-plugin.com)
[![Listed on DSH Directory](https://dsh.directory/badges/listed.svg)](https://dsh.directory/plugins?q=perrylink)

**Building the [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness) plugin ecosystem: 40 open-source plugins (`dsh.bundle` plugins) — 45 repos in the family (Apache-2.0) across security, workflows, research, messaging bridges, and developer experience — plus the DSH Desktop Market catalog, a plugin-certification registry, and the dsh-plugin-doctor CI checker. 39 of the 45 repos ship five-language READMEs, every plugin ships CI, npm provenance, and a Gitee mirror, and 42 of the repos declare the `dsh.bundle` contract — 69.1k npm downloads in August plus 72.5k in September through the 16th (128.9k over the trailing 30 days, npm window 08-18..09-16, measured 2026-09-17). I also contribute upstream to [Cordis](https://github.com/cordiverse/cordis) — the plugin-core framework DeepSeek Harness itself is built on — and to [deepseek-ai](https://github.com/deepseek-ai) projects, with a merged [FlashMLA](https://github.com/deepseek-ai/FlashMLA) fix among them.**

DeepSeek Harness turned "everything is a plugin" into an ecosystem. I build the plugins I wish existed — engineering-discipline guardrails, runtime panels, cross-session memory, and verifiable research engines — and publish them the way production software deserves.

---

<!-- Round rotation: keep only the newest two rounds (current + one previous). Older rounds live in git history and can be restored on request. Rounds are narrative only — no Snapshot/counter lines: live counts belong to the badge row and "Where the plugins live", and per-edition copies go stale. GHSA/long-lived references belong in "Upstream & community contributions". -->

## 📣 Latest — 2026-09-18 round

- **The 0.1.6-alpha.2 wave — 23 plugins released in one serial pass.** The whole family moved onto the alpha.2 tuple: every peer range gained the `>=0.1.6-0 <0.2.0` clause, manifests now declare `dsh.manifestVersion: 1` + `engines.dsh`, and 23 packages shipped to npm with provenance in a single tag-by-tag run — [dsh-local-ai](https://github.com/PerryLink/dsh-local-ai) 0.2.11, [dsh-score](https://github.com/PerryLink/dsh-score) 0.2.12, [dsh-memento](https://github.com/PerryLink/dsh-memento) 0.5.13, [dsh-talk](https://github.com/PerryLink/dsh-talk) 0.3.11, [dsh-fast](https://github.com/PerryLink/dsh-fast) 0.2.13, [dsh-observe](https://github.com/PerryLink/dsh-observe) 0.2.13, [dsh-click](https://github.com/PerryLink/dsh-click) 0.3.11, [dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) 0.1.7, and the rest of the family in the same pass.
- **The gates themselves turned out to be the story.** A family-wide audit found that **18 repos' published-line typecheck had never run in CI**, and that **11 JavaScript repos' "second ruler" measured the same type universe as the first** (a no-op `paths: {}`). Both classes are fixed or scheduled, and the newly honest rulers immediately caught real defects: a renamed request-image contract, four stale transitive peers that left a built entry unimportable, and a duplicated `typert-protocol` generation that only `skipLibCheck: false` could see.
- **The release path needed repairs too:** stale `NPM_TOKEN` secrets across the fleet (npm answers **404**, not 401, for an unauthorized publish), lockfiles left behind by the peer-range edits, and a compat pin that predated the `agent/created` payload gaining `source`/`signal`.
- **Held for the browser round:** twelve client-facing plugins stay unpublished until the manual checklist marks them verified.

### 2026-09-16 round

- **The 0.1.6-alpha.1 compatibility wave** — 8 commits across 6 repos, pushed this morning: [dsh-ticktick](https://github.com/PerryLink/dsh-ticktick) carrying both Typert strict-codec faces for the new checkout, [dsh-click](https://github.com/PerryLink/dsh-click) and [dsh-score](https://github.com/PerryLink/dsh-score) implementing the scripted subprocess providers, [dsh-background-agents](https://github.com/PerryLink/dsh-background-agents) listening on `agent/created` instead of the removed `agent/session-start`, and UTF-8 BOM hygiene on the Portuguese READMEs of [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) and [dsh-background-agents](https://github.com/PerryLink/dsh-background-agents).
- **One release worth opening — [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) 0.6.15**, fixing [#27](https://github.com/PerryLink/dsh-mcp-panel/issues/27): both renderers now emit the loader's real patch dialect (`- id:` + `name:` + `disabled:`/`config:`) instead of the unimplemented `- set:`, and it can browse upstream Resources through the shipped `mcp-resources` tools.
- **Ledger watch:** [dsh-plugin-guide](https://github.com/PerryLink/dsh-plugin-guide) grew its unfixed-issues ledger with the third community verification batch (now 32+7, with the fs-ext desktop item adopted as #27).

---

## 🚀 Flagship picks (start here)

| Plugin | What it gives you | Install |
|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | Second-model auto-review on the approval chain, fail-closed by default (175★) | `dsh plugin --profile web add dsh-auto-review` |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Claude Code-style declarative allow/deny/ask rules plus a process-level network policy (112★) | `dsh plugin --profile web add dsh-permission-rules` |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | Approval-gated cross-session memory (`ctx.memory` + SQLite) (97★) | `dsh plugin --profile web add dsh-memento` |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | MCP management console: `/mcp` + Settings tab + trial calls (61★) | `dsh plugin --profile web add dsh-mcp-panel` |
| [dsh-checkpoint-rewind](https://github.com/PerryLink/dsh-checkpoint-rewind) | Claude Code `/rewind` equivalent: git-first snapshots, session forks, one-shot restore (17★) | `dsh plugin --profile web add dsh-checkpoint-rewind` |
| [dsh-autotier](https://github.com/PerryLink/dsh-autotier) | Automatic strong/cheap model-tier routing with deterministic risk guards and a `/tier` command (new) | `dsh plugin --profile web add dsh-autotier` |

One-command starter pack: **[dsh-kit](https://github.com/PerryLink/dsh-kit)** — installs the core family in one command.

## 🔬 Research suite

| Plugin | What it gives you | npm |
|---|---|---|
| [dsh-research-report](https://github.com/PerryLink/dsh-research-report) | Verifiable research reports: content-addressed evidence ledger, manifest seal hash, byte-level citation checks, drift detection, disproof ledger | [npm](https://www.npmjs.com/package/dsh-research-report) |
| [dsh-fund-research](https://github.com/PerryLink/dsh-fund-research) | Chinese mutual-fund research with sealed, traceable snapshots — every number traces to a hashed source | [npm](https://www.npmjs.com/package/dsh-fund-research) |
| [dsh-industry-research](https://github.com/PerryLink/dsh-industry-research) | Industry/company research: chain-map SVG with bottleneck detection, timeline, company cards, adversarial review | [npm](https://www.npmjs.com/package/dsh-industry-research) |
| [dsh-data-quality](https://github.com/PerryLink/dsh-data-quality) | Deterministic data profiling/cleaning/verification: DAMA scorecard, content-hash dedupe, metric expectations | [npm](https://www.npmjs.com/package/dsh-data-quality) |

## 📦 The full family — 40 plugins + 5 support repos

### 🔒 Security (4)

| Plugin | One-liner | npm |
|---|---|---|
| [dsh-defend](https://github.com/PerryLink/dsh-defend) | Injection/jailbreak/secret detection + destructive-delete gate | [npm](https://www.npmjs.com/package/dsh-defend) |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Declarative allow/deny/ask rules + a local HTTP/CONNECT network policy | [npm](https://www.npmjs.com/package/dsh-permission-rules) |
| [dsh-mask](https://github.com/PerryLink/dsh-mask) | PII masking/sanitization | [npm](https://www.npmjs.com/package/dsh-mask) |
| [dsh-skill-pack-security](https://github.com/PerryLink/dsh-skill-pack-security) | Security-audit skill pack + supply-chain gate | [npm](https://www.npmjs.com/package/@perrylink/dsh-skill-pack-security-provider) |

### 🔁 Workflows (8)

| Plugin | One-liner | npm |
|---|---|---|
| [dsh-background-agents](https://github.com/PerryLink/dsh-background-agents) | Durable background child agents with a Web UI sidebar, messaging and interrupt | [npm](https://www.npmjs.com/package/dsh-background-agents) |
| [dsh-team-rooms](https://github.com/PerryLink/dsh-team-rooms) | Cross-session team rooms: shared message bus, task board, approval-gated handoffs and a timeline that survive restarts | [npm](https://www.npmjs.com/package/dsh-team-rooms) |
| [dsh-checkpoint-rewind](https://github.com/PerryLink/dsh-checkpoint-rewind) | Snapshots, forks, one-shot restore | [npm](https://www.npmjs.com/package/dsh-checkpoint-rewind) |
| [dsh-github](https://github.com/PerryLink/dsh-github) | GitHub PR/issue integration + Action, writes approval-gated | [npm](https://www.npmjs.com/package/@perrylink/dsh-github) |
| [dsh-claude-move](https://github.com/PerryLink/dsh-claude-move) | Migrate Claude Code/Codex/OpenCode/Hermes into DSH | [npm](https://www.npmjs.com/package/dsh-claude-move) |
| [dsh-click](https://github.com/PerryLink/dsh-click) | Desktop control tools (Windows/macOS) | [npm](https://www.npmjs.com/package/dsh-click) |
| [dsh-session-sync](https://github.com/PerryLink/dsh-session-sync) | Git-backed session synchronization | [npm](https://www.npmjs.com/package/dsh-session-sync) |
| [dsh-test-drive](https://github.com/PerryLink/dsh-test-drive) | Install→smoke→uninstall test driver for plugins | [npm](https://www.npmjs.com/package/dsh-test-drive) |

### ✨ Experience & UX (4)

| Plugin | One-liner | npm |
|---|---|---|
| [dsh-composer-history](https://github.com/PerryLink/dsh-composer-history) | Terminal-style input history for the web composer | [npm](https://www.npmjs.com/package/dsh-composer-history) |
| [dsh-output-styles](https://github.com/PerryLink/dsh-output-styles) | Runtime-switchable model output styles | [npm](https://www.npmjs.com/package/dsh-output-styles) |
| [dsh-session-pin](https://github.com/PerryLink/dsh-session-pin) | Pin sessions in the Web sidebar | [npm](https://www.npmjs.com/package/dsh-session-pin) |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | Approval-gated cross-session memory protocol | [npm](https://www.npmjs.com/package/dsh-memento) |

### 🧪 Evaluation (3)

| Plugin | One-liner | npm |
|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | Second-model auto-review on the approval chain | [npm](https://www.npmjs.com/package/dsh-auto-review) |
| [dsh-doublecheck](https://github.com/PerryLink/dsh-doublecheck) | Engineering-discipline guard: grill, gates, adversary review | [npm](https://www.npmjs.com/package/dsh-doublecheck) |
| [dsh-score](https://github.com/PerryLink/dsh-score) | Plugin quality scoring across git/gh/npm | [npm](https://www.npmjs.com/package/dsh-score) |

### 📊 Observability & cost (4)

| Plugin | One-liner | npm |
|---|---|---|
| [dsh-autotier](https://github.com/PerryLink/dsh-autotier) | Automatic strong/cheap model-tier routing with deterministic risk guards | [npm](https://www.npmjs.com/package/dsh-autotier) |
| [dsh-budget](https://github.com/PerryLink/dsh-budget) | Token/cost metering, budget caps, carbon estimate, latency benchmarks | [npm](https://www.npmjs.com/package/dsh-budget) |
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

### 🛠️ Developer experience (4)

| Plugin | One-liner | npm |
|---|---|---|
| [dsh-lsp-actions](https://github.com/PerryLink/dsh-lsp-actions) | LSP diagnostics/formatting/completion/actions | [npm](https://www.npmjs.com/package/dsh-lsp-actions) |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | MCP management console | [npm](https://www.npmjs.com/package/dsh-mcp-panel) |
| [dsh-plugin-guide](https://github.com/PerryLink/dsh-plugin-guide) | Plugin-dev knowledge base + CLI toolchain + release-engineering guide | [npm](https://www.npmjs.com/package/dsh-plugin-guide) |
| [dsh-plugin-upgrade-015](https://github.com/PerryLink/dsh-plugin-upgrade-015) | Merged plugin-author upgrade corridor (`0.1.3-alpha.1 → 0.1.5-rc.1`): evidence-bound version card + zero-dependency 20-seam scanner (bundle skill + npx CLI) | [npm](https://www.npmjs.com/package/dsh-plugin-upgrade-015) |

*Support repos:* [dsh-plugin-kit](https://github.com/PerryLink/dsh-plugin-kit) (review-rule meta package) · [dsh-catalog](https://github.com/PerryLink/dsh-catalog) (DSH Desktop Market catalog source) · [dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) (certification MCP server) · [dsh-kit](https://github.com/PerryLink/dsh-kit) (one-command installer) · [dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) (plugin health checker)

### 📱 Messaging & bridges (3)

| Plugin | One-liner | npm |
|---|---|---|
| [dsh-wechat](https://github.com/pan17/dsh-wechat) | WeChat ↔ DSH bridge (Tencent iLink bot): text/image/file/voice, approvals in chat — developed with [pan17](https://github.com/pan17/dsh-wechat), who now hosts the repo and publishes the npm package | [npm](https://www.npmjs.com/package/dsh-wechat) |
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

## 🔧 Upstream & community contributions

- **[Cordis](https://github.com/cordiverse/cordis)** — the upstream plugin-core framework that powers DeepSeek Harness. Contributor: merged [PR #122](https://github.com/cordiverse/cordis/pull/122) (Windows + macOS CI, contributor badge) · 45-patch real-world regression suite + verification for the merged include-journal fix [PR #121](https://github.com/cordiverse/cordis/pull/121) · reported [issue #112](https://github.com/cordiverse/cordis/issues/112) with an initial fix ([PR #116](https://github.com/cordiverse/cordis/pull/116), superseded by #121) · open [issue #124](https://github.com/cordiverse/cordis/issues/124) (NodeNext type declarations, evidence + local fix) · open [PR #126](https://github.com/cordiverse/cordis/pull/126) (ship `src` in core/loader/timer tarballs, CI green) · 18-item errata for the [Cordis paper](https://arxiv.org/abs/2608.25512).
- **[cordiverse/http](https://github.com/cordiverse/http)** — open [issue #14](https://github.com/cordiverse/http/issues/14): the README documents a `Response` wrapper that `ctx.http()` no longer returns, with repo-verified line references and a README-only fix.
- **[schemastery](https://github.com/shigma/schemastery)** — the schema framework used across the DSH stack: filed [issue #77](https://github.com/shigma/schemastery/issues/77) (ESM/NodeNext consumption gap, full evidence) and two open PRs — [#78](https://github.com/shigma/schemastery/pull/78) (exports map + dual declarations) and [#79](https://github.com/shigma/schemastery/pull/79) (repair the test-runner flag and a stale i18n expectation).
- **[dsh-handbook](https://github.com/Electricitysheep/dsh-handbook)** — the official DSH handbook: two merged PRs ([#67](https://github.com/Electricitysheep/dsh-handbook/pull/67), [#68](https://github.com/Electricitysheep/dsh-handbook/pull/68)).
- **Security** — published advisory [GHSA-j922-p6h6-p255](https://github.com/PerryLink/dsh-permission-rules/security/advisories/GHSA-j922-p6h6-p255) for dsh-permission-rules (medium, patched in 0.6.16).
- **Official harness repo** — it does not accept external pull requests (verified: `GET /repos/deepseek-ai/deepseek-harness/pulls` returns 404 and CONTRIBUTING.md says so), so that line runs through issues, Discussions (the Show Your Plugins! post [#6104](https://github.com/deepseek-ai/deepseek-harness/discussions/6104)) and the plugin ecosystem instead — while the wider deepseek-ai org is open to fixes (FlashMLA #224 merged).
- **[deepseek-ai](https://github.com/deepseek-ai)** — contributor to [FlashMLA](https://github.com/deepseek-ai/FlashMLA): merged [PR #224](https://github.com/deepseek-ai/FlashMLA/pull/224) (2026-09-15), switching the 128-bit `st.async` PTX transport from `long2` to `longlong2` — on Windows (LLP64) the pair silently carried two 32-bit halves into an instruction expecting two 64-bit values.
- **Directory & hub submissions** — 35 plugins published on [DSH Directory](https://dsh.directory) (29 submission issues authored via [alexchenzl/dsh-plugin-directory](https://github.com/alexchenzl/dsh-plugin-directory)) · 150 open [Submission] issues tracked on the [omdsh hub](https://github.com/omdsh-dev/dsh-hub-workshop) · curated entries merged into [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin), [0xsline/awesome-deepseek-harness](https://github.com/0xsline/awesome-deepseek-harness), the [AdamPlatin123 radar](https://github.com/AdamPlatin123/dsh-plugin-radar), and [Zhiyuan-Fan's list](https://github.com/Zhiyuan-Fan/Awesome-DeepSeek-Harness-Plugins).

## 🌍 Where the plugins live

- **GitHub** (this profile) — source, CI, releases; **1,089★ across the 45 family repos** (40 `dsh.bundle` plugins + 5 support repos), 42 of them declaring the `dsh.bundle` contract
- **[Gitee](https://gitee.com/perrylink)** — 105 public repos, with all 45 family repos mirrored (branches + tags; the upgrade-corridor mirror lives under its former name `dsh-plugin-upgrade`)
- **npm** — 41 packages published with CI provenance (35 bare + 6 scoped), plus 3 legacy names on the registry (2 deprecated corridor packages and the withdrawn `dsh-personal-directive`), 682 versions across the 44 PerryLink-published names (716 with pan17's dsh-wechat) — 69.1k downloads in August plus 72.5k in September through the 16th (128.9k over the trailing 30 days, npm window 08-18..09-16)
- **DSH Desktop Market** — add the catalog source `https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json` under Market → Sources to browse all 40 family packages in-app (curated summaries + icons, contract-validated, CI-smoked)

Listed on [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) (36 entries), [DSH Directory](https://dsh.directory/plugins?q=perrylink) (35 published), [Awesome DeepSeek Harness](https://github.com/0xsline/awesome-deepseek-harness), [awesome-deepseekharness](https://github.com/awesome-deepseekharness/awesome-deepseek-harness), [Zhiyuan-Fan's list](https://github.com/Zhiyuan-Fan/Awesome-DeepSeek-Harness-Plugins), the [AdamPlatin123 radar](https://github.com/AdamPlatin123/dsh-plugin-radar), [dsh-market](https://github.com/dsh-market/dsh-market) (via the awesome-dsh-plugin registry), [dsh-suite](https://github.com/whyihaveyou/dsh-suite), and [ZeroPointRepo's list](https://github.com/ZeroPointRepo/awesome-dsh-plugins). Auto-indexed on [deepseek1024.com](https://deepseek1024.com) (36 entries). Certification: [dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification).

## 中文介绍

我在 DeepSeek Harness 上把 Claude Code / Codex 生态里最实用的能力做成了开源插件:检查点回退、声明式权限、输出风格、跨会话记忆、MCP 面板、模型档位路由、微信/TickTick 桥接,以及可验证研究报告 / 基金研究 / 行业研究 / 数据质量「研究四件套」——共 **40 个插件**(Apache-2.0),全部带五语文档、CI、npm 发布与 Gitee 镜像(45 个家族仓中有 39 个带五语文档,42 个声明 `dsh.bundle` 契约)。npm:已发布 **41 个包**(35 个非 scoped + 6 个 scoped),另有 3 个历史名称(两个弃用的走廊包,以及已撤回的 `dsh-personal-directive`),44 个 PerryLink 名称累计 682 个版本(含 pan17 的 dsh-wechat 为 716 个)。下载量:8 月 69.1k + 9 月截至 16 日 72.5k(近 30 天 128.9k,统计窗口 08-18..09-16)。一键全家桶:[`dsh-kit`](https://github.com/PerryLink/dsh-kit)。同时我也是 DeepSeek Harness 上游核心框架 **Cordis**([cordiverse/cordis](https://github.com/cordiverse/cordis))的贡献者:Windows/macOS CI 已合并(#122),为 include-journal 修复(#121)提供了 45 个真实补丁文件的回归套件与验证,tarball 打包修复 PR(#126)与 NodeNext 类型声明 issue(#124)在途,并向 schemastery 提交了 ESM 消费面 issue(#77)与两枚 PR(#78/#79)。同时我已成为 [deepseek-ai](https://github.com/deepseek-ai) 官方仓贡献者:[FlashMLA](https://github.com/deepseek-ai/FlashMLA) #224 已合并(修复 Windows 下 sm90 st.async PTX 传输的 128 位宽度静默截断)。

2026-09-18 轮:① **0.1.6-alpha.2 升级波——23 个插件一次串行发完**：全族 peer 区间补上第三段 `>=0.1.6-0 <0.2.0`,清单统一声明 `dsh.manifestVersion: 1` + `engines.dsh`,23 个包带 provenance 依次发布到 npm([dsh-local-ai](https://github.com/PerryLink/dsh-local-ai) 0.2.11、[dsh-score](https://github.com/PerryLink/dsh-score) 0.2.12、[dsh-memento](https://github.com/PerryLink/dsh-memento) 0.5.13、[dsh-talk](https://github.com/PerryLink/dsh-talk) 0.3.11、[dsh-fast](https://github.com/PerryLink/dsh-fast) 0.2.13、[dsh-observe](https://github.com/PerryLink/dsh-observe) 0.2.13、[dsh-click](https://github.com/PerryLink/dsh-click) 0.3.11、[dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) 0.1.7 等);② **门禁本身被审计出两类系统性问题**——全族排查发现 **18 个仓的「已发布线」类型尺子从未在 CI 里跑过**、**11 个 JS 仓的第二把尺子量与第一把同一个类型宇宙**(`paths: {}` 是空操作);两类都已修或已排期,而新尺子立刻抓到真缺陷(附件契约改名、四个陈旧传递 peer 让 built entry 直接无法 import、重复的 `typert-protocol` 代际只有 `skipLibCheck: false` 看得见);③ **发布链路也修了三处**:全族陈旧的 `NPM_TOKEN`(npm 对未授权发布返回 **404** 而非 401)、peer 区间改动后遗留的 lockfile、以及早于 `agent/created` 带上 `source`/`signal` 的 compat pin;④ **12 个面向客户端的插件按住不发**,等人工浏览器清单标记 VERIFIED。

### 2026-09-16 轮

① **0.1.6-alpha.1 兼容波**——今天上午 6 个仓 8 次提交:[dsh-ticktick](https://github.com/PerryLink/dsh-ticktick) 为新 checkout 同时携带两种 Typert strict-codec 面孔、[dsh-click](https://github.com/PerryLink/dsh-click) 与 [dsh-score](https://github.com/PerryLink/dsh-score) 补上脚本化子进程 provider、[dsh-background-agents](https://github.com/PerryLink/dsh-background-agents) 改听 `agent/created`(原 `agent/session-start` 已移除),并清掉 [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) 与 [dsh-background-agents](https://github.com/PerryLink/dsh-background-agents) 葡语文档里的 UTF-8 BOM;② **值得点开的版本——[dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) 0.6.15**:修复 [#27](https://github.com/PerryLink/dsh-mcp-panel/issues/27),两种渲染器改输出加载器真实的 patch 方言(`- id:` + `name:` + `disabled:`/`config:`,取代未实现的 `- set:`),并可浏览上游 Resources;③ [dsh-plugin-guide](https://github.com/PerryLink/dsh-plugin-guide) 未修复清单补入第三批社区验证条目(现为 32+7,fs-ext 桌面条目作为 #27 入列)。

待业中。近期考虑给自己安排一次体检。因此最近将减少熬夜，后续的更新迭代节奏会适当放缓。当然，问题和缺陷修复不会停，只是发布频率会降低一些，还请大家谅解。
