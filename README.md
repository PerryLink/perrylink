# Hi, I'm PerryLink 👋

[![Gitee mirror](https://img.shields.io/badge/Gitee-mirror-c71d23?logo=gitee)](https://gitee.com/perrylink)
[![DSH Desktop Market](https://img.shields.io/badge/DSH_Desktop_Market-source-0969da)](https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json)
[![npm packages](https://img.shields.io/badge/npm-packages-cb3837?logo=npm)](https://www.npmjs.com/search?q=perrylink)
![plugins](https://img.shields.io/badge/plugins-40-0969da)
![repos](https://img.shields.io/badge/repos-117-green)
![stars](https://img.shields.io/badge/stars-930%2B-yellow)
![npm downloads](https://img.shields.io/badge/npm_downloads-115k%2B_AugSep-cb3837)
[![Certified dsh-auto-review](https://raw.githubusercontent.com/PerryLink/dsh-plugin-certification/main/badges/PerryLink__dsh-auto-review.svg)](https://github.com/PerryLink/dsh-plugin-certification)
[![awesome-dsh-plugin](https://awesome-dsh-plugin.com/badge.svg)](https://awesome-dsh-plugin.com)
[![Listed on DSH Directory](https://dsh.directory/badges/listed.svg)](https://dsh.directory/plugins?q=perrylink)

**Building the DeepSeek Harness plugin ecosystem: 40 open-source plugins (Apache-2.0) across security, workflows, research, messaging bridges, and developer experience — plus the DSH Desktop Market catalog, a plugin-certification registry, and the dsh-plugin-doctor CI checker. Every project ships five-language READMEs, CI, npm provenance, and Gitee mirrors — 63.9k npm downloads in August plus 51.2k in September so far (115.1k over the last 30 days). I also contribute upstream to [Cordis](https://github.com/cordiverse/cordis), the plugin-core framework DeepSeek Harness itself is built on.**

DeepSeek Harness turned "everything is a plugin" into an ecosystem. I build the plugins I wish existed — engineering-discipline guardrails, runtime panels, cross-session memory, and verifiable research engines — and publish them the way production software deserves.

---

## 📣 Latest — 2026-09-10 round

- **Whole family moved to the `0.1.5-rc.1` line** — 38 packages upgraded and republished in one wave (37 plugin repos + the security provider): dual-line peers (`0.1.2-rc.1` and the `0.1.5` alpha→rc line), the new V3 session format and client-UI seams, a 3,516-file encoding audit with published tarballs byte-identical to git blobs, 44 Gitee mirrors synced. The Market catalog is at 40 entries, because the family's 40th plugin landed the same day.
- **npm had been serving the Chinese README on every package page — root cause found, fixed family-wide** — npm takes the first match of its `{README,README.*}` glob, and `README.zh.md` sorted ahead of `README.md` (the registry's own `readmeFilename` still reports `README.zh.md` for 33 published packages). Every translation is now `README-<lang>.md` in 38 of the 40 plugin repos (the audit counted 1,931 references across all 40; file contents are unchanged byte for byte), with a CI guard that fails if a second npm-visible `README*.md` ever reappears in a package root. Docs-only, so each package page flips to English as its next version ships.
- **Security advisory [GHSA-j922-p6h6-p255](https://github.com/PerryLink/dsh-permission-rules/security/advisories/GHSA-j922-p6h6-p255) published** — an IPv4-mapped IPv6 literal could slip past `ips` network rules in dsh-permission-rules (medium, CVSS 5.5); fixed in 0.6.16 and hardened in 0.6.17/0.6.18, where the proxy connects to the address it actually adjudicated — never a second DNS resolution. The two follow-ups from that same report then shipped in **0.7.0**: `network.upstreamProxy` (chain through an upstream proxy, with three guards — never chain loopback, never chain what `ips` already adjudicated, never chain without a usable upstream; an unreachable upstream is a 502, never a silent direct fallback) and a Settings-page **Allow this host** action that writes the minimal allow rule at index 0 through the YAML document API, so comments survive. 0.6.20/0.6.21 also make a corrected rule take effect without restarting, and the docs now state plainly what the network policy covers: traffic from shell subprocesses the plugin derives — not the host's own outbound connections.
- **Two new tools for plugin authors** — [dsh-plugin-upgrade-rc1](https://github.com/PerryLink/dsh-plugin-upgrade-rc1) scans the `0.1.5-alpha.1 → 0.1.5-rc.1` step: 11 client-UI seams (C1–C5/H1–H4/P1), a migration card, a bundled skill, zero runtime dependencies, v0.1.0 with provenance. One seam deliberately stays an error — the bare `conversation` slot is deleted in rc.1 with no alias, so a third-party plugin keyed on it fails to mount silently; the card ships the rewrite recipe (`conversation` → `main.conversation`) instead of a green check. [dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) 0.2.0 adds the first third-party scan (20 plugins, machine-readable results, a stated corrections path), closes three silent-pass paths, and retires declarations that stopped being true.
- **Inbound, release and repository hygiene** — six community reports answered with shipped fixes (permission-rules [#18](https://github.com/PerryLink/dsh-permission-rules/issues/18)/[#19](https://github.com/PerryLink/dsh-permission-rules/issues/19)/[#21](https://github.com/PerryLink/dsh-permission-rules/issues/21)/[#22](https://github.com/PerryLink/dsh-permission-rules/issues/22) → 0.6.19, session-pin [#4](https://github.com/PerryLink/dsh-session-pin/issues/4) → 0.7.10, lsp-actions [#4](https://github.com/PerryLink/dsh-lsp-actions/issues/4) → 0.5.0); 14 dependency PRs merged or closed (open PRs 16 → 0); phantom branch-protection contexts repaired in three repos so outside PRs can merge again; publish workflows gained `--provenance` and now fail loudly instead of reporting a release that published nothing. A 29-fork / 329-branch audit retired 16 dead forks and one repo — public repos 124 → 108, forks 29 → 13, non-default branches 329 → 22, fork Actions 813 → 0 — after quarantining every branch head first, and kept six archived forks whose branches exist nowhere else.
- **Snapshot** — 937★ across 47 repos · 40 live repos declaring the `dsh.bundle` contract · 44 npm packages (38 bare + 6 scoped) · 674 versions · 63.9k downloads in August plus 51.2k in September so far (115.1k over the last 30 days; npm's published series reaches Sep 10, with Sep 3, 7 and 8 missing registry-wide) · 104 public Gitee repos.

### 2026-09-09 round

- **[dsh-autotier](https://github.com/PerryLink/dsh-autotier)** — a new cost-routing plugin taken from 0.1.0 to **0.2.0 in one day**: alpha-line peer support with request-time provider/model preflight, then the browser half (Settings card + composer tier pill over Typert Remote), explicit model-selection sync and multi-router detection — 206 tests, Compat matrix green on both harness lines.
- **[dsh-plugin-upgrade](https://github.com/PerryLink/dsh-plugin-upgrade-015) 0.1.2** — a plugin-author upgrade skill: a version-locked `0.1.3-alpha.1 → 0.1.5-alpha.1` migration card plus a zero-dependency seam scanner, shipped as a bundle skill and an npx CLI.
- **Release hygiene** — backfilled all 10 missing GitHub Releases (gap zero) and checked every published package's `latest` against its repo version; plus same-day fixes in session-sync 0.2.12, permission-rules 0.6.15 and skill-pack-security 2.2.13, with plugin-doctor pinned to 0.1.5 across 35 CI workflows.

---

## 🚀 Flagship picks (start here)

| Plugin | What it gives you | Install |
|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | Second-model auto-review on the approval chain, fail-closed by default (157★) | `dsh plugin --profile web add dsh-auto-review` |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Claude Code-style declarative allow/deny/ask rules plus a process-level network policy (114★) | `dsh plugin --profile web add dsh-permission-rules` |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | Approval-gated cross-session memory (`ctx.memory` + SQLite) (85★) | `dsh plugin --profile web add dsh-memento` |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | MCP management console: `/mcp` + Settings tab + trial calls (55★) | `dsh plugin --profile web add dsh-mcp-panel` |
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
- **[Gitee](https://gitee.com/perrylink)** — 104 public repos, with 44 family repos mirrored automatically (branches + tags)
- **npm** — 44 packages published with CI provenance (38 bare + 6 scoped)
- **DSH Desktop Market** — add the catalog source `https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json` under Market → Sources to browse all 40 family packages in-app (curated summaries + icons, contract-validated, CI-smoked)

Listed on [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) (36 entries), [DSH Directory](https://dsh.directory/plugins?q=perrylink) (35 published), [Awesome DeepSeek Harness](https://github.com/0xsline/awesome-deepseek-harness), [awesome-deepseekharness](https://github.com/awesome-deepseekharness/awesome-deepseek-harness), [Zhiyuan-Fan's list](https://github.com/Zhiyuan-Fan/Awesome-DeepSeek-Harness-Plugins), the [AdamPlatin123 radar](https://github.com/AdamPlatin123/dsh-plugin-radar), [dsh-market](https://github.com/dsh-market/dsh-market) (via the awesome-dsh-plugin registry), [dsh-suite](https://github.com/whyihaveyou/dsh-suite), and [ZeroPointRepo's list](https://github.com/ZeroPointRepo/awesome-dsh-plugins). Auto-indexed on [deepseek1024.com](https://deepseek1024.com) (36 entries). Certification: [dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification).

## 中文介绍

我在 DeepSeek Harness 上把 Claude Code / Codex 生态里最实用的能力做成了开源插件:检查点回退、声明式权限、输出风格、跨会话记忆、MCP 面板、模型档位路由、微信/TickTick 桥接,以及可验证研究报告 / 基金研究 / 行业研究 / 数据质量「研究四件套」——共 **40 个插件**(Apache-2.0),全部带五语文档、CI、npm 发布与 Gitee 镜像。一键全家桶:[`dsh-kit`](https://github.com/PerryLink/dsh-kit)。同时我也是 DeepSeek Harness 上游核心框架 **Cordis**([cordiverse/cordis](https://github.com/cordiverse/cordis))的贡献者:Windows/macOS CI 已合并(#122),为 include-journal 修复(#121)提供了 45 个真实补丁文件的回归套件与验证,tarball 打包修复 PR(#126)与 NodeNext 类型声明 issue(#124)在途,并向 schemastery 提交了 ESM 消费面 issue(#77)与两枚 PR(#78/#79)。

2026-09-10 轮:① **全家族迁到 `0.1.5-rc.1` 线**——38 个包一次性升级并重发(37 个插件仓 + 安全 provider):双线 peer(`0.1.2-rc.1` 与 `0.1.5` alpha→rc)、新的 V3 会话格式与客户端 UI 缝、3,516 个受控文本文件编码核验(发布 tarball 与 git blob 逐字节相等)、Gitee 44 个镜像同步;Market 目录 40 项——家族第 40 个声明 `dsh.bundle` 的插件同日落地;② **npm 包页此前一直在展示中文 README,根因已定位并全家族修复**——npm 取 `{README,README.*}` glob 的首个命中,而 `README.zh.md` 排在 `README.md` 之前(registry 自己的 `readmeFilename` 对 33 个已发布包仍报 `README.zh.md`);全部译文改名为 `README-<lang>.md`(40 个插件仓已完成 38 个;审计口径为 40 仓 1,931 处引用,文件内容逐字节不变),并新增 CI 守卫:包根一旦再出现第二个 npm 可见的 `README*.md` 即失败。纯文档改动,各包页面随下一次发版切到英文;③ **安全公告 [GHSA-j922-p6h6-p255](https://github.com/PerryLink/dsh-permission-rules/security/advisories/GHSA-j922-p6h6-p255) 发布**——dsh-permission-rules 的 `ips` 网络规则可被 IPv4 映射 IPv6 字面量绕过(medium / CVSS 5.5),0.6.16 修复,0.6.17/0.6.18 进一步加固(代理只连裁决到的地址,不做二次 DNS 解析);同一份来件的两项后续在 **0.7.0** 出厂:`network.upstreamProxy`(经上游代理链式转发,三条守卫——loopback 不链、`ips` 已裁决的不链、无可用上游不链;上游不可达即 502,绝不静默回退直连)与设置页 **「允许此主机」**(走 YAML Document API 在索引 0 写入最小 allow 规则,保留注释);0.6.20/0.6.21 让改对的规则无需重启即生效,并如实写明该网络策略的覆盖面——插件派生的 shell 子进程流量,**不含宿主自身的出站连接**;④ **两件面向插件作者的新工具**——[dsh-plugin-upgrade-rc1](https://github.com/PerryLink/dsh-plugin-upgrade-rc1) 扫描 `0.1.5-alpha.1 → 0.1.5-rc.1` 走廊的 11 个客户端 UI 缝(C1–C5/H1–H4/P1),带迁移卡与捆绑 skill,零运行时依赖,v0.1.0 带 provenance;其中一条缝按保守侧保持 error:裸 `conversation` slot 在 rc.1 被删且无别名,按旧 key 的第三方插件会静默不挂载,故卡片给的是改写配方(`conversation` → `main.conversation`)而不是绿勾;[dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) 0.2.0 交付首次第三方扫描(20 个插件、机器可读结果、明确的更正通道),封掉三条静默通过路径,并撤下已不成立的声明;⑤ **来件、发布与仓库卫生**——6 个社区来件答复并交付修复(permission-rules #18/#19/#21/#22 → 0.6.19,session-pin #4 → 0.7.10,lsp-actions #4 → 0.5.0),14 个依赖 PR 合并或关闭(开放 PR 16 → 0),修复 3 个仓的分支保护幻影检查项(此前外部 PR 无法合并),发布 workflow 补 `--provenance` 并改为「没真正发布就不再报成功」;29 fork / 329 分支审计退役 16 个死 fork 与 1 个仓——公开仓 124 → 108、fork 29 → 13、非默认分支 329 → 22、fork 内 Actions 813 → 0——退役前先隔离保存每条分支头,并保留 6 个归档 fork(其分支在别处已不存在);⑥ **快照**——家族 892★ / 47 仓、40 个声明 `dsh.bundle` 的插件、npm **42 包**(36 裸名 + 6 scoped)· 631 版、8 月 6.39 万 + 9 月至今 3.84 万下载(近 30 天 10.23 万;npm 已发布序列到 9-09,其中 9-03 / 9-07 / 9-08 全 registry 缺数据)、Gitee 公开仓 104。

2026-09-09 轮:① **dsh-autotier**——一天内从 0.1.0 走到 **0.2.0**:补齐 alpha 线 peer 并新增请求期 provider/model 预检,随后交付浏览器半(Settings 卡 + 输入框档位胶囊,走 Typert Remote)、显式选型同步与多路由器并存检测,206 个用例全绿;② **dsh-plugin-upgrade 0.1.2**——插件作者升级技能:版本锁定迁移卡 + 零依赖 seam 扫描器(bundle skill + npx CLI);③ **发布卫生**——补齐全部 10 个缺失的 GitHub Release(缺口归零),并完成 session-sync 0.2.12、permission-rules 0.6.15、skill-pack-security 2.2.13 当日修复,plugin-doctor 在 35 个 CI 工作流统一钉 0.1.5。

待业中。近期考虑给自己安排一次体检。因此最近将减少熬夜，后续的更新迭代节奏会适当放缓。当然，问题和缺陷修复不会停，只是发布频率会降低一些，还请大家谅解。
