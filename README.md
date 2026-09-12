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

## 📣 Latest — 2026-09-12 round

- **Whole family moved to the `dsh-v0.1.5-rc.2` host line — 39 repos migrated and 42 Releases shipped in one day** — every repo took the same two-commit change (pin `@deepseek-ai/dsh-*` to `0.1.5-rc.2`, then refresh the five-language compatibility baseline); the newborn dsh-team-rooms refreshed its baseline without a family pin, and the security provider pinned its provider subtree separately. The day closed with 134 commits across 42 repos, 44 tags and **42 GitHub Releases** — the only two tags left without a Release are same-day supersedes (dsh-draw 0.2.13, skill-pack-security 2.2.15), and only dsh-catalog (which ships no releases) and dsh-cert-mcp (last released Sep 10) sit outside the wave.
- **[dsh-team-rooms](https://github.com/PerryLink/dsh-team-rooms) 1.0.1** — day two of the extracted plugin: CI builds the bundles before the test steps, the keystone test resolves the `0.9.6` fixture sibling instead of pinning an absolute path, and the five-language baseline moved to rc.2 with the rest of the family.
- **[dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) 0.7.1 → 0.7.2, twice in one day** — [PR #24](https://github.com/PerryLink/dsh-permission-rules/pull/24) splits the pure allow-host helpers out of the host-only module, then the rc.2 pin.
- **[dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) 0.2.1** — `fix(R8): catch every stale peer-range shape, not the two that existed on Sep 5`: the checker no longer passes a peer range it merely failed to recognise.
- **Hygiene and small correctness fixes** — dsh-budget and dsh-background-agents restored em dashes mangled in their comments, dsh-plugin-kit dropped the byte-order marks its own release gate forbids, dsh-research-report restored the Chinese evidence markers in its hub submission, dsh-personal-directive now derives its reported version from `package.json`, and dsh-draw's test reads the version from `src/version.ts` instead of hardcoding it.
- **Snapshot** — 938★ across 47 repos · 40 live repos declaring the `dsh.bundle` contract · 44 npm packages (38 bare + 6 scoped) · 676 versions · 63.9k downloads in August plus 51.2k in September so far (115.1k over the last 30 days; npm's published series reaches Sep 10, with Sep 3, 7 and 8 missing registry-wide) · 104 public Gitee repos.

### 2026-09-11 round

- **[dsh-team-rooms](https://github.com/PerryLink/dsh-team-rooms) 1.0.0** — team rooms extracted out of dsh-background-agents into a standalone plugin (whose background-agent half is superseded by DSH's native continuable subagents): cross-session rooms with a message bus, a shared task board, approval-gated handoffs and a timeline that survive restarts. CI also stopped passing the npm token through `NODE_AUTH_TOKEN`.
- **[dsh-plugin-upgrade-015](https://github.com/PerryLink/dsh-plugin-upgrade-015) 0.1.0** — the two upgrade corridors merged into one package; npm rejected the original name so it ships as `-015`, and a manual workflow deprecated the two retired npm names — a workflow that was itself retired once the deprecation had run.
- **Verified registry re-pointed** — [dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) moved its verified registry to dsh-plugin-upgrade-015 and enrolled dsh-team-rooms, refreshing the badges for both.

---

## 🚀 Flagship picks (start here)

| Plugin | What it gives you | Install |
|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | Second-model auto-review on the approval chain, fail-closed by default (157★) | `dsh plugin --profile web add dsh-auto-review` |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Claude Code-style declarative allow/deny/ask rules plus a process-level network policy (115★) | `dsh plugin --profile web add dsh-permission-rules` |
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
- **[Gitee](https://gitee.com/perrylink)** — 104 public repos, with 43 family repos mirrored automatically (branches + tags)
- **npm** — 44 packages published with CI provenance (38 bare + 6 scoped)
- **DSH Desktop Market** — add the catalog source `https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json` under Market → Sources to browse all 40 family packages in-app (curated summaries + icons, contract-validated, CI-smoked)

Listed on [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) (36 entries), [DSH Directory](https://dsh.directory/plugins?q=perrylink) (35 published), [Awesome DeepSeek Harness](https://github.com/0xsline/awesome-deepseek-harness), [awesome-deepseekharness](https://github.com/awesome-deepseekharness/awesome-deepseek-harness), [Zhiyuan-Fan's list](https://github.com/Zhiyuan-Fan/Awesome-DeepSeek-Harness-Plugins), the [AdamPlatin123 radar](https://github.com/AdamPlatin123/dsh-plugin-radar), [dsh-market](https://github.com/dsh-market/dsh-market) (via the awesome-dsh-plugin registry), [dsh-suite](https://github.com/whyihaveyou/dsh-suite), and [ZeroPointRepo's list](https://github.com/ZeroPointRepo/awesome-dsh-plugins). Auto-indexed on [deepseek1024.com](https://deepseek1024.com) (36 entries). Certification: [dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification).

## 中文介绍

我在 DeepSeek Harness 上把 Claude Code / Codex 生态里最实用的能力做成了开源插件:检查点回退、声明式权限、输出风格、跨会话记忆、MCP 面板、模型档位路由、微信/TickTick 桥接,以及可验证研究报告 / 基金研究 / 行业研究 / 数据质量「研究四件套」——共 **40 个插件**(Apache-2.0),全部带五语文档、CI、npm 发布与 Gitee 镜像。一键全家桶:[`dsh-kit`](https://github.com/PerryLink/dsh-kit)。同时我也是 DeepSeek Harness 上游核心框架 **Cordis**([cordiverse/cordis](https://github.com/cordiverse/cordis))的贡献者:Windows/macOS CI 已合并(#122),为 include-journal 修复(#121)提供了 45 个真实补丁文件的回归套件与验证,tarball 打包修复 PR(#126)与 NodeNext 类型声明 issue(#124)在途,并向 schemastery 提交了 ESM 消费面 issue(#77)与两枚 PR(#78/#79)。

2026-09-12 轮:① **全家族迁到 `dsh-v0.1.5-rc.2` 宿主线——39 个仓当日完成迁移,42 个 Release 当日发出**——每个仓都是同一套两提交改动(把 `@deepseek-ai/dsh-*` 钉到 `0.1.5-rc.2`,再刷新五语兼容基线);新生的 dsh-team-rooms 只刷基线、未钉家族,安全 provider 另钉 provider 子树。当天 42 个仓 134 次提交、44 个 tag、**42 个 GitHub Release**;44 个 tag 中仅两枚同日被后继版本取代者没有 Release(dsh-draw 0.2.13、skill-pack-security 2.2.15),波外仅 dsh-catalog(本就不发 Release)与 dsh-cert-mcp(上次发版 09-10);② **[dsh-team-rooms](https://github.com/PerryLink/dsh-team-rooms) 1.0.1**——抽取独立后的第二天:CI 先构建 bundle 再跑测试,keystone 用例改为解析 `0.9.6` fixture 的同级路径而非写死绝对路径,五语基线随家族一并迁到 rc.2;③ **[dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) 一天两发 0.7.1 → 0.7.2**——[PR #24](https://github.com/PerryLink/dsh-permission-rules/pull/24) 把纯 allow-host 辅助函数从 host-only 模块中拆出,随后钉 rc.2;④ **[dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) 0.2.1**——`fix(R8): catch every stale peer-range shape, not the two that existed on Sep 5`:不再对"只是没被识别"的 peer range 放行;⑤ **卫生与小修**——dsh-budget 与 dsh-background-agents 修回注释里被弄坏的破折号,dsh-plugin-kit 去掉自家发布门禁禁止的 BOM,dsh-research-report 修回 hub 投稿里的中文证据标记,dsh-personal-directive 改为从 `package.json` 推导上报版本,dsh-draw 的用例改为从 `src/version.ts` 读版本而非写死;⑥ **快照**——家族 938★ / 47 仓、40 个存活仓声明 `dsh.bundle`、npm **44 包**(38 裸名 + 6 scoped)· 676 版本 · 8 月 63.9k + 9 月 51.2k(近 30 天 115.1k;npm 已公布序列到 09-10,09-03/07/08 全站缺失)· Gitee 公开仓 104。

2026-09-11 轮:① **[dsh-team-rooms](https://github.com/PerryLink/dsh-team-rooms) 1.0.0**——从 dsh-background-agents 中抽出成为独立插件(后者的后台代理半已被 DSH 原生可续子代理取代):跨会话房间,带消息总线、共享任务板、审批门控的交接,以及可跨重启存活的时间线;同日 CI 不再经 `NODE_AUTH_TOKEN` 传 npm token;② **[dsh-plugin-upgrade-015](https://github.com/PerryLink/dsh-plugin-upgrade-015) 0.1.0**——两条升级走廊合并为一个包;npm 拒绝原包名,故以 `-015` 发布;并用一个手动 workflow 弃用两个退役包名——该 workflow 在弃用完成后自行退役;③ **verified 注册表改指**——[dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) 把 verified 注册表改指 dsh-plugin-upgrade-015 并纳入 dsh-team-rooms,同步刷新两者徽章。

待业中。近期考虑给自己安排一次体检。因此最近将减少熬夜，后续的更新迭代节奏会适当放缓。当然，问题和缺陷修复不会停，只是发布频率会降低一些，还请大家谅解。
