# Hi, I'm PerryLink 👋

[![Gitee mirror](https://img.shields.io/badge/Gitee-mirror-c71d23?logo=gitee)](https://gitee.com/perrylink)
[![DSH Desktop Market](https://img.shields.io/badge/DSH_Desktop_Market-source-0969da)](https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json)
[![npm packages](https://img.shields.io/badge/npm-packages-cb3837?logo=npm)](https://www.npmjs.com/search?q=perrylink)
![plugins](https://img.shields.io/badge/plugins-40-0969da)
![repos](https://img.shields.io/badge/repos-158-green)
![stars](https://img.shields.io/badge/stars-1237-yellow)
![npm downloads](https://img.shields.io/badge/npm_downloads-130k_30d-cb3837)
[![Certified dsh-auto-review](https://raw.githubusercontent.com/PerryLink/dsh-plugin-certification/main/badges/PerryLink__dsh-auto-review.svg)](https://github.com/PerryLink/dsh-plugin-certification)
[![awesome-dsh-plugin](https://awesome-dsh-plugin.com/badge.svg)](https://awesome-dsh-plugin.com)
[![Listed on DSH Directory](https://dsh.directory/badges/listed.svg)](https://dsh.directory/plugins?q=perrylink)

**Building the [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness) plugin ecosystem: 40 open-source plugins in a 45-repo family (Apache-2.0) — security, workflows, research, messaging bridges, developer experience — plus the DSH Desktop Market catalog, a plugin-certification registry and the dsh-plugin-doctor CI checker. Every plugin ships CI, npm provenance and a Gitee mirror, 40 of the 45 repos carry five-language docs, and 43 of the PerryLink-owned ones declare the `dsh.bundle` contract — 69.1k npm downloads in August plus 82.4k in September through the 18th (131.0k over the trailing 30 days). I also contribute upstream to [Cordis](https://github.com/cordiverse/cordis) — the plugin-core framework DeepSeek Harness is built on — and to [deepseek-ai](https://github.com/deepseek-ai) projects, including a merged [FlashMLA](https://github.com/deepseek-ai/FlashMLA) fix.**

DeepSeek Harness turned "everything is a plugin" into an ecosystem. I build the plugins I wish existed — engineering-discipline guardrails, runtime panels, cross-session memory, and verifiable research engines — and publish them the way production software deserves.

---

<!-- Round rotation: keep only the newest two rounds (current + one previous). Older rounds live in git history and can be restored on request. Rounds are narrative only — no Snapshot/counter lines: live counts belong to the badge row and "Where the plugins live", and per-edition copies go stale. GHSA/long-lived references belong in "Upstream & community contributions". -->

## 📣 Latest — 2026-09-19 round

- **G-4b, the gate hardening, is now the default:** the published-line ruler runs in CI in **15 more repos**, **41** capped the compat-profile job at 25 minutes, and **22** added a `package.json`/lockfile fail-fast. The now-honest rulers immediately repaired **40** type errors in [dsh-claude-move](https://github.com/PerryLink/dsh-claude-move) and **54** in [dsh-catalog](https://github.com/PerryLink/dsh-catalog).
- **Releases worth opening:** [dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) **0.2.1** (off the `@perrylink/` scope, now listed in the official MCP Registry), [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) **0.12.6**, [dsh-plugin-guide](https://github.com/PerryLink/dsh-plugin-guide) **0.3.16** and [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) **0.7.4** — the rest of the 22-package wave was routine hygiene and dependency bumps.

### 2026-09-18 round

- **The 0.1.6-alpha.2 wave — 23 plugins released in one serial pass**, every peer range gaining the `>=0.1.6-0 <0.2.0` clause and every manifest declaring `dsh.manifestVersion: 1` + `engines.dsh`.
- **The gates themselves were the story:** a family-wide audit found **18 repos whose published-line typecheck had never run in CI**, and **11 JavaScript repos whose "second ruler" measured the same type universe as the first**.
- **The release path needed repairs too** — stale `NPM_TOKEN` secrets (npm answers **404**, not 401, for an unauthorized publish), lockfiles left by the peer-range edits, a stale compat pin — and twelve client-facing plugins were held for the browser checklist.

---

## 🚀 Flagship picks (start here)

*The six most-starred family plugins (★ measured 2026-09-19); every other family repo is listed in full further down.*

| Plugin | What it gives you | Install |
|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | Second-model auto-review on the approval chain, fail-closed by default (184★) | `dsh plugin --profile web add dsh-auto-review` |
| [dsh-research-report](https://github.com/PerryLink/dsh-research-report) | Verifiable research reports: content-addressed evidence ledger, manifest seal hash, byte-level citation checks, drift detection, disproof ledger (134★) | `dsh plugin --profile web add dsh-research-report` |
| [dsh-industry-research](https://github.com/PerryLink/dsh-industry-research) | Industry/company research: chain-map SVG with bottleneck detection, timeline, company cards, adversarial review (133★) | `dsh plugin --profile web add dsh-industry-research` |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Claude Code-style declarative allow/deny/ask rules plus a process-level network policy (112★) | `dsh plugin --profile web add dsh-permission-rules` |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | Approval-gated cross-session memory (`ctx.memory` + SQLite) (106★) | `dsh plugin --profile web add dsh-memento` |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | MCP management console: `/mcp` + Settings tab + trial calls (61★) | `dsh plugin --profile web add dsh-mcp-panel` |

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
| [dsh-plugin-upgrade](https://github.com/PerryLink/dsh-plugin-upgrade) | Plugin-author upgrade skill: one package, one corridor index that detects the caller's peer band and routes to the matching closed card (`0.1.3-alpha.1 → 0.1.5-rc.1`, `0.1.5-rc.2 → 0.1.6-alpha.2`), plus a zero-dependency seam scanner (bundle skill + npx CLI) | [npm](https://www.npmjs.com/package/dsh-plugin-upgrade) |

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

- **GitHub** (this profile) — source, CI, releases; **1,237★ across all 158 public repos, 1,167★ of it in the 45 family repos** (40 `dsh.bundle` plugins + 5 support repos), 43 of the PerryLink-owned repos declaring the `dsh.bundle` contract
- **[Gitee](https://gitee.com/perrylink)** — 105 public repos: all 45 family repos are mirrored (default branch + all tags, not every branch) alongside mirrors of other projects; the upgrade corridor is mirrored there as `dsh-plugin-upgrade`
- **npm** — 42 packages published through CI (37 unscoped + 5 scoped; 41 carry a provenance attestation on their current latest version), plus 3 deprecated old names still on the registry (the retired corridor leg `dsh-plugin-upgrade-rc1`, the withdrawn `dsh-personal-directive`, and the retired scoped `@perrylink/dsh-cert-mcp`, renamed to the unscoped `dsh-cert-mcp`) — 45 names, 735 versions (769 with pan17's dsh-wechat) — 69.1k downloads in August plus 82.4k in September through the 18th (131.0k over the trailing 30 days, npm window 08-20..09-18 — the series zeroes out 09-03, 09-07, 09-08, 09-15 and 09-17; the 45 PerryLink names alone are 63.9k / 79.8k / 125.7k)
- **DSH Desktop Market** — add the catalog source `https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json` under Market → Sources to browse the family in-app (43 catalog entries with curated summaries + icons, contract-validated, CI-smoked)
- **MCP Registry** — [`io.github.PerryLink/dsh-cert`](https://registry.modelcontextprotocol.io/v0/servers?search=perrylink) v0.2.2 (npm `dsh-cert-mcp`) is on the official registry, published from its release workflow over GitHub OIDC — note it is indexed under the server name, not the package name
- **GitHub Actions** — [dsh-github](https://github.com/PerryLink/dsh-github) and [dsh-test-drive](https://github.com/PerryLink/dsh-test-drive) also ship composite actions, so they install as `uses: PerryLink/dsh-test-drive@vX`

Listed on [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) (39 entries, 38 live), [DSH Directory](https://dsh.directory/plugins?q=perrylink) (35 plugin pages published; its own `q=perrylink` view surfaces 24), [walkinglabs' plugin list](https://github.com/walkinglabs/awesome-deepseek-harness-plugins) (Developer Tooling: [dsh-plugin-guide](https://github.com/PerryLink/dsh-plugin-guide), [dsh-test-drive](https://github.com/PerryLink/dsh-test-drive) and the upgrade corridor), [Awesome DeepSeek Harness](https://github.com/0xsline/awesome-deepseek-harness), [awesome-deepseekharness](https://github.com/awesome-deepseekharness/awesome-deepseek-harness), [Zhiyuan-Fan's list](https://github.com/Zhiyuan-Fan/Awesome-DeepSeek-Harness-Plugins), the [AdamPlatin123 radar](https://github.com/AdamPlatin123/dsh-plugin-radar), [dsh-market](https://github.com/dsh-market/dsh-market) (via the awesome-dsh-plugin registry), [dsh-suite](https://github.com/whyihaveyou/dsh-suite), and [ZeroPointRepo's list](https://github.com/ZeroPointRepo/awesome-dsh-plugins). Auto-indexed on [deepseek1024.com](https://deepseek1024.com) (45 plugin pages), also indexed on [dshfind.com](https://dshfind.com/zh/plugins/PerryLink/dsh-memento) — a third-party DSH plugin supermarket with per-plugin score badges — and on [Glama](https://glama.ai/mcp/servers/PerryLink/dsh-cert-mcp), and further catalogued by [DSH Get](https://dshget.com), [chnjames/dsh-plugin-market](https://github.com/chnjames/dsh-plugin-market) and [NoWint/Oh-My-DSH](https://github.com/NoWint/Oh-My-DSH) — the GitHub [`dsh-plugin` topic](https://github.com/topics/dsh-plugin) (46 family repos tagged) is what most of them ingest from. Scored on [OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/PerryLink/dsh-auto-review). Certification: [dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification) (spec + registry, 1 family repo certified so far).

## 中文介绍

我在 DeepSeek Harness 上把 Claude Code / Codex 生态里最实用的能力做成了开源插件:检查点回退、声明式权限、输出风格、跨会话记忆、MCP 面板、模型档位路由、微信/TickTick 桥接,以及可验证研究报告 / 基金研究 / 行业研究 / 数据质量「研究四件套」——共 **40 个插件**(Apache-2.0):全部带 CI、npm 发布与 Gitee 镜像,45 个家族仓中有 40 个带五语文档,43 个 PerryLink 自有仓声明 `dsh.bundle` 契约。npm 已发布 **42 个包**(37 个非 scoped + 5 个 scoped,另有 3 个弃用旧名仍挂在 registry 上),45 个 PerryLink 名称累计 735 个版本(含 pan17 的 dsh-wechat 为 769 个),下载量 8 月 69.1k + 9 月截至 18 日 82.4k(近 30 天 131.0k;npm 日序列在 09-03、09-07、09-08、09-15、09-17 归零)。一键全家桶:[`dsh-kit`](https://github.com/PerryLink/dsh-kit)。同时我是 DeepSeek Harness 上游核心框架 **Cordis**([cordiverse/cordis](https://github.com/cordiverse/cordis))的贡献者,也是 [deepseek-ai](https://github.com/deepseek-ai) 官方仓贡献者:[FlashMLA](https://github.com/deepseek-ai/FlashMLA) 的修复已合并(#224);逐条 PR/issue 见下方 Upstream 一节。

2026-09-19 轮:① **G-4b 门禁加固成为默认**:15 个仓把「已发布线」尺子接进 CI,41 个仓把 compat profile 封顶 25 分钟,22 个仓加上「`package.json` 与 lockfile 不一致即失败」——新尺子随即修掉 [dsh-claude-move](https://github.com/PerryLink/dsh-claude-move) 的 40 个、[dsh-catalog](https://github.com/PerryLink/dsh-catalog) 的 54 个类型错误。② **值得点开的版本**:[dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) **0.2.1**(去掉 `@perrylink/` scope、进入官方 MCP Registry)、[dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) **0.12.6**、[dsh-plugin-guide](https://github.com/PerryLink/dsh-plugin-guide) **0.3.16**、[dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) **0.7.4**,同批其余包为例行卫生与依赖升级。

### 2026-09-18 轮

① **0.1.6-alpha.2 升级波——23 个插件一次串行发完**:全族 peer 区间补上第三段 `>=0.1.6-0 <0.2.0`,清单统一声明 `dsh.manifestVersion: 1` + `engines.dsh`。② **门禁本身才是故事**:全族排查出 **18 个仓的「已发布线」类型尺子从未在 CI 里跑过**、**11 个 JS 仓的第二把尺子量与第一把同一个类型宇宙**。③ **发布链路也需修补**:全族陈旧的 `NPM_TOKEN`(npm 对未授权发布返回 **404** 而非 401)、peer 区间改动后遗留的 lockfile、过期的 compat pin;另有 12 个面向客户端的插件按住等浏览器清单。

待业中。近期考虑给自己安排一次体检。因此最近将减少熬夜，后续的更新迭代节奏会适当放缓。当然，问题和缺陷修复不会停，只是发布频率会降低一些，还请大家谅解。
