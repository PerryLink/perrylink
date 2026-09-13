# Hi, I'm PerryLink 👋

[![Gitee mirror](https://img.shields.io/badge/Gitee-mirror-c71d23?logo=gitee)](https://gitee.com/perrylink)
[![DSH Desktop Market](https://img.shields.io/badge/DSH_Desktop_Market-source-0969da)](https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json)
[![npm packages](https://img.shields.io/badge/npm-packages-cb3837?logo=npm)](https://www.npmjs.com/search?q=perrylink)
![plugins](https://img.shields.io/badge/plugins-40-0969da)
![repos](https://img.shields.io/badge/repos-146-green)
![stars](https://img.shields.io/badge/stars-969-yellow)
![npm downloads](https://img.shields.io/badge/npm_downloads-125k%2B_AugSep-cb3837)
[![Certified dsh-auto-review](https://raw.githubusercontent.com/PerryLink/dsh-plugin-certification/main/badges/PerryLink__dsh-auto-review.svg)](https://github.com/PerryLink/dsh-plugin-certification)
[![awesome-dsh-plugin](https://awesome-dsh-plugin.com/badge.svg)](https://awesome-dsh-plugin.com)
[![Listed on DSH Directory](https://dsh.directory/badges/listed.svg)](https://dsh.directory/plugins?q=perrylink)

**Building the DeepSeek Harness plugin ecosystem: 40 open-source plugins (`dsh.bundle` plugins) — 45 repos in the family (Apache-2.0) across security, workflows, research, messaging bridges, and developer experience — plus the DSH Desktop Market catalog, a plugin-certification registry, and the dsh-plugin-doctor CI checker. 39 of the 45 repos ship five-language READMEs, and every plugin ships CI, npm provenance, and a Gitee mirror — 69.1k npm downloads in August plus 55.9k in September through the 11th (124.9k over the last 30 days). I also contribute upstream to [Cordis](https://github.com/cordiverse/cordis), the plugin-core framework DeepSeek Harness itself is built on.**

DeepSeek Harness turned "everything is a plugin" into an ecosystem. I build the plugins I wish existed — engineering-discipline guardrails, runtime panels, cross-session memory, and verifiable research engines — and publish them the way production software deserves.

---

<!-- Round rotation: keep only the newest two rounds (current + one previous). Older rounds live in git history and can be restored on request. GHSA/long-lived references belong in "Upstream & community contributions", not here. -->

## 📣 Latest — 2026-09-13 round

- **The day went wide instead of deep — the ecosystem-submission wave.** 29 new forks seeded across the harness ecosystem, then 149 pull requests and 47 issues opened against 33 upstream projects and directories in a single day, **52 of them already merged** ([imsai-sh](https://github.com/imsai-sh/awesome-deepseek-harness-plugins) took 17, [beancookie](https://github.com/beancookie/awesome-dsh-plugin) 4, [Dominic789654](https://github.com/Dominic789654/awesome-deepseek-harness) 3, plus [Oh-My-DSH](https://github.com/like-study1/Oh-My-DSH), [dsh-plugin-radar](https://github.com/AdamPlatin123/dsh-plugin-radar), [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) and more) — 147 of the 149 outside my own repos. The family itself was quiet: 16 commits across 11 repos and 2 releases.
- **Two releases to open** — [dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) 0.1.6 and [dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) 0.2.3, both adding `dsh.bundle` so the certification registry and the health checker clear the marketplace gates themselves. Alongside them: [dsh-catalog](https://github.com/PerryLink/dsh-catalog) added four entries (team-rooms, plugin-kit, plugin-doctor, plugin-upgrade-015), [dsh-team-rooms](https://github.com/PerryLink/dsh-team-rooms) repaired its CI workflow, and four repos dropped withdrawn-repo references from their manifests.
- **Snapshot** — 969★ across the 45 family repos (40 `dsh.bundle` plugins + 5 support repos) · 40 live repos declaring the `dsh.bundle` contract · 42 published npm packages (36 bare + 6 scoped; two further names are the deprecated legacy corridor packages) · 689 versions · 69.1k downloads in August plus 55.9k in September through the 11th (124.9k over the last 30 days, npm window 08-13..09-11) · 105 public Gitee repos, 42 of them family mirrors.

### 2026-09-12 round

- **The whole family moved twice in one day.** In the afternoon every plugin repo adopted the `dsh-v0.1.5-rc.2` host line — the same two-commit change everywhere (pin `@deepseek-ai/dsh-*`, refresh the five-language compatibility baseline) — 39 repos migrated and 42 Releases shipped in one pass. In the evening the same fleet ran a second synchronized pass: 42 repos refreshed their five-language READMEs and the shared family roster at once. The day closed at **198 commits across 46 repos and 45 GitHub Releases**.
- **A few releases worth opening** — [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) 0.7.1 → 0.7.2 splits the pure allow-host helpers out of the host-only module ([PR #24](https://github.com/PerryLink/dsh-permission-rules/pull/24)); [dsh-team-rooms](https://github.com/PerryLink/dsh-team-rooms) 1.0.1 is day two of the extracted plugin; [dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) 0.2.2 stopped passing a stale peer range it merely failed to recognise; [dsh-mask](https://github.com/PerryLink/dsh-mask) 0.2.10 and [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) 0.12.4 tightened their docs and tests. Alongside them the usual hygiene batch: restored em dashes and Chinese evidence markers, the byte-order marks the release gate forbids, and two plugins now reading their version from the package manifest instead of a hardcoded string.
- **Snapshot** — 950★ across the 45 family repos (40 `dsh.bundle` plugins + 5 support repos) · 40 live repos declaring the `dsh.bundle` contract · 44 published npm packages (38 bare + 6 scoped; two are the deprecated legacy names retired by the upgrade-corridor merge) · 679 versions · 63.9k downloads in August plus 51.2k in September so far (115.1k over the last 30 days; npm's published series reaches Sep 10, with Sep 3, 7 and 8 missing registry-wide) · 104 public Gitee repos.

---

## 🚀 Flagship picks (start here)

| Plugin | What it gives you | Install |
|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | Second-model auto-review on the approval chain, fail-closed by default (165★) | `dsh plugin --profile web add dsh-auto-review` |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Claude Code-style declarative allow/deny/ask rules plus a process-level network policy (114★) | `dsh plugin --profile web add dsh-permission-rules` |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | Approval-gated cross-session memory (`ctx.memory` + SQLite) (89★) | `dsh plugin --profile web add dsh-memento` |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | MCP management console: `/mcp` + Settings tab + trial calls (55★) | `dsh plugin --profile web add dsh-mcp-panel` |
| [dsh-checkpoint-rewind](https://github.com/PerryLink/dsh-checkpoint-rewind) | Claude Code `/rewind` equivalent: git-first snapshots, session forks, one-shot restore (18★) | `dsh plugin --profile web add dsh-checkpoint-rewind` |
| [dsh-autotier](https://github.com/PerryLink/dsh-autotier) | Automatic strong/cheap model-tier routing with deterministic risk guards and a `/tier` command (new) | `dsh plugin --profile web add dsh-autotier` |

One-command starter pack: **[dsh-kit](https://github.com/PerryLink/dsh-kit)** — installs the core family in one command.

## 🔬 Research suite

| Plugin | What it gives you | npm |
|---|---|---|
| [dsh-research-report](https://github.com/PerryLink/dsh-research-report) | Verifiable research reports: content-addressed evidence ledger, manifest seal hash, byte-level citation checks, drift detection, disproof ledger | [npm](https://www.npmjs.com/package/dsh-research-report) |
| [dsh-fund-research](https://github.com/PerryLink/dsh-fund-research) | Chinese mutual-fund research with sealed, traceable snapshots — every number traces to a hashed source | [npm](https://www.npmjs.com/package/dsh-fund-research) |
| [dsh-industry-research](https://github.com/PerryLink/dsh-industry-research) | Industry/company research: chain-map SVG with bottleneck detection, timeline, company cards, adversarial review | [npm](https://www.npmjs.com/package/dsh-industry-research) |
| [dsh-data-quality](https://github.com/PerryLink/dsh-data-quality) | Deterministic data profiling/cleaning/verification: DAMA scorecard, content-hash dedupe, metric expectations | [npm](https://www.npmjs.com/package/dsh-data-quality) |

## 📦 The full family — 40 plugins by pillar

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
- **Official harness repo** — it does not accept external pull requests (verified: `GET /repos/deepseek-ai/deepseek-harness/pulls` returns 404 and CONTRIBUTING.md says so), so that line runs through issues, Discussions (the Show Your Plugins! post [#6104](https://github.com/deepseek-ai/deepseek-harness/discussions/6104)) and the plugin ecosystem instead.
- **Directory & hub submissions** — 35 plugins published on [DSH Directory](https://dsh.directory) (29 submission issues authored via [alexchenzl/dsh-plugin-directory](https://github.com/alexchenzl/dsh-plugin-directory)) · 149 open [Submission] issues tracked on the [omdsh hub](https://github.com/omdsh-dev/dsh-hub-workshop) · curated entries merged into [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin), [0xsline/awesome-deepseek-harness](https://github.com/0xsline/awesome-deepseek-harness), the [AdamPlatin123 radar](https://github.com/AdamPlatin123/dsh-plugin-radar), and [Zhiyuan-Fan's list](https://github.com/Zhiyuan-Fan/Awesome-DeepSeek-Harness-Plugins).

## 🌍 Where the plugins live

- **GitHub** (this profile) — source, CI, releases
- **[Gitee](https://gitee.com/perrylink)** — 105 public repos, with 42 family repos mirrored automatically (branches + tags)
- **npm** — 42 packages published with CI provenance (36 bare + 6 scoped; two further names on the registry are the deprecated legacy corridor packages) — 124.9k downloads over npm's 2026-08-13..2026-09-11 window
- **DSH Desktop Market** — add the catalog source `https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json` under Market → Sources to browse all 40 family packages in-app (curated summaries + icons, contract-validated, CI-smoked)

Listed on [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) (36 entries), [DSH Directory](https://dsh.directory/plugins?q=perrylink) (35 published), [Awesome DeepSeek Harness](https://github.com/0xsline/awesome-deepseek-harness), [awesome-deepseekharness](https://github.com/awesome-deepseekharness/awesome-deepseek-harness), [Zhiyuan-Fan's list](https://github.com/Zhiyuan-Fan/Awesome-DeepSeek-Harness-Plugins), the [AdamPlatin123 radar](https://github.com/AdamPlatin123/dsh-plugin-radar), [dsh-market](https://github.com/dsh-market/dsh-market) (via the awesome-dsh-plugin registry), [dsh-suite](https://github.com/whyihaveyou/dsh-suite), and [ZeroPointRepo's list](https://github.com/ZeroPointRepo/awesome-dsh-plugins). Auto-indexed on [deepseek1024.com](https://deepseek1024.com) (36 entries). Certification: [dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification).

## 中文介绍

我在 DeepSeek Harness 上把 Claude Code / Codex 生态里最实用的能力做成了开源插件:检查点回退、声明式权限、输出风格、跨会话记忆、MCP 面板、模型档位路由、微信/TickTick 桥接,以及可验证研究报告 / 基金研究 / 行业研究 / 数据质量「研究四件套」——共 **40 个插件**(Apache-2.0),全部带五语文档、CI、npm 发布与 Gitee 镜像。npm 下载量:8 月 69.1k + 9 月截至 11 日 55.9k(近 30 天 124.9k,统计窗口 08-13..09-11)。一键全家桶:[`dsh-kit`](https://github.com/PerryLink/dsh-kit)。同时我也是 DeepSeek Harness 上游核心框架 **Cordis**([cordiverse/cordis](https://github.com/cordiverse/cordis))的贡献者:Windows/macOS CI 已合并(#122),为 include-journal 修复(#121)提供了 45 个真实补丁文件的回归套件与验证,tarball 打包修复 PR(#126)与 NodeNext 类型声明 issue(#124)在途,并向 schemastery 提交了 ESM 消费面 issue(#77)与两枚 PR(#78/#79)。

2026-09-13 轮:① **这一天不在深而在广——生态投稿波**。当天为 DSH 生态新开 29 个 fork 仓,随后面向 **33 个上游项目与目录**一次性提交 **149 枚 PR 与 47 条 issue,其中 52 枚已合并**([imsai-sh](https://github.com/imsai-sh/awesome-deepseek-harness-plugins) 收 17 枚,[beancookie](https://github.com/beancookie/awesome-dsh-plugin) 收 4 枚,[Dominic789654](https://github.com/Dominic789654/awesome-deepseek-harness) 收 3 枚,另有 [Oh-My-DSH](https://github.com/like-study1/Oh-My-DSH)、[dsh-plugin-radar](https://github.com/AdamPlatin123/dsh-plugin-radar)、[awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) 等)——149 枚里 147 枚落在家门之外;家族本体这天反而安静:11 个仓 16 次提交、2 个 Release;② **两个值得点开的版本**——[dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) 0.1.6 与 [dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) 0.2.3,双双补上 `dsh.bundle` 让自己也过市场门禁;同批还有 [dsh-catalog](https://github.com/PerryLink/dsh-catalog) 新增 4 条包条目(team-rooms、plugin-kit、plugin-doctor、plugin-upgrade-015)、[dsh-team-rooms](https://github.com/PerryLink/dsh-team-rooms) 修复 CI workflow,以及 4 个仓清掉已撤回仓的清单引用;③ **快照**——家族 969★(45 仓:40 个 `dsh.bundle` 插件 + 5 个支撑仓)· 40 个存活仓声明 `dsh.bundle` · npm **42 包**(36 裸名 + 6 scoped;另有 2 个已弃用的走廊旧名在册)· 689 版本 · 8 月 69.1k + 9 月截至 11 日 55.9k(近 30 天 124.9k,窗口 08-13..09-11)· Gitee 公开仓 105,其中 42 个为家族镜像。

### 2026-09-12 轮

① **全家族一天两波推进**——下午 39 个仓统一迁到 `dsh-v0.1.5-rc.2` 宿主线(全家族同一套两提交改动:钉 `@deepseek-ai/dsh-*`、刷新五语兼容基线),42 个 Release 当波发出;傍晚同一批仓再同步刷一遍,42 个仓一次性刷新五语文档与家族名册。全天 46 个仓 198 次提交、**45 个 GitHub Release**;② **几个值得点开的版本**——[dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) 0.7.1 → 0.7.2 把纯 allow-host 辅助函数从 host-only 模块拆出([PR #24](https://github.com/PerryLink/dsh-permission-rules/pull/24)),[dsh-team-rooms](https://github.com/PerryLink/dsh-team-rooms) 1.0.1 是抽独立后的第二天,[dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) 0.2.2 不再对"只是没被识别"的 peer range 放行,[dsh-mask](https://github.com/PerryLink/dsh-mask) 0.2.10 与 [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) 0.12.4 收紧文档与用例;同批还有例行卫生修复(修回被弄坏的破折号与中文证据标记、清掉发布门禁禁止的 BOM、两个插件改为从 package.json 读版本);③ **快照**——家族 950★(45 仓:40 个 `dsh.bundle` 插件 + 5 个支撑仓)· 40 个存活仓声明 `dsh.bundle` · npm **44 包**(38 裸名 + 6 scoped,其中两个是升级走廊合并后弃用的旧名)· 679 版本 · 8 月 63.9k + 9 月 51.2k(近 30 天 115.1k;npm 已公布序列到 09-10,09-03/07/08 全站缺失)· Gitee 公开仓 104。

待业中。近期考虑给自己安排一次体检。因此最近将减少熬夜，后续的更新迭代节奏会适当放缓。当然，问题和缺陷修复不会停，只是发布频率会降低一些，还请大家谅解。
