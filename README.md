# Hi, I'm PerryLink 👋

[![Gitee mirror](https://img.shields.io/badge/Gitee-mirror-c71d23?logo=gitee)](https://gitee.com/perrylink)
[![DSH Desktop Market](https://img.shields.io/badge/DSH_Desktop_Market-source-0969da)](https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json)
[![npm packages](https://img.shields.io/badge/npm-packages-cb3837?logo=npm)](https://www.npmjs.com/search?q=perrylink)
![plugins](https://img.shields.io/badge/plugins-39-0969da)
![repos](https://img.shields.io/badge/repos-124-green)
![stars](https://img.shields.io/badge/stars-890%2B-yellow)
![npm downloads](https://img.shields.io/badge/npm_downloads-90k%2B_AugSep-cb3837)
[![Certified dsh-auto-review](https://raw.githubusercontent.com/PerryLink/dsh-plugin-certification/main/badges/PerryLink__dsh-auto-review.svg)](https://github.com/PerryLink/dsh-plugin-certification)
[![awesome-dsh-plugin](https://awesome-dsh-plugin.com/badge.svg)](https://awesome-dsh-plugin.com)
[![Listed on DSH Directory](https://dsh.directory/badges/listed.svg)](https://dsh.directory/plugins/perrylink)

**Building the DeepSeek Harness plugin ecosystem: 39 open-source plugins (Apache-2.0) across security, workflows, research, messaging bridges, and developer experience — plus the DSH Desktop Market catalog, a plugin-certification registry, and the dsh-plugin-doctor CI checker. Every project ships five-language READMEs, CI, npm provenance, and Gitee mirrors — 63.9k npm downloads in August plus 26.4k in the first 9 days of September (90.3k over the last 30 days). I also contribute upstream to [Cordis](https://github.com/cordiverse/cordis), the plugin-core framework DeepSeek Harness itself is built on.**

DeepSeek Harness turned "everything is a plugin" into an ecosystem. I build the plugins I wish existed — engineering-discipline guardrails, runtime panels, cross-session memory, and verifiable research engines — and publish them the way production software deserves.

---

## 📣 Latest — 2026-09-09 round

- **[dsh-autotier](https://github.com/PerryLink/dsh-autotier)** — a new cost-routing plugin taken from 0.1.0 to **0.2.0 in one day**: alpha-line peer support (`0.1.5-alpha.1`) with request-time provider/model preflight, then the browser half (Settings card + composer tier pill over Typert Remote), explicit model-selection sync, multi-router detection — 206 tests, Compat matrix green on both harness lines.
- **[dsh-plugin-upgrade](https://github.com/PerryLink/dsh-plugin-upgrade) 0.1.2** — a plugin-author upgrade skill: a version-locked `0.1.3-alpha.1 → 0.1.5-alpha.1` migration card plus a zero-dependency seam scanner (V3 session format, `Inbox`, `ctx.agent`, PTC rename …), shipped as a bundle skill and an npx CLI.
- **Release hygiene** — backfilled all 10 missing GitHub Releases (gap now zero) and checked every published package's `latest` against its repo version (39/40 verified, one bump in flight); the DSH Desktop Market catalog holds 39 entries with zero version lag.
- **Same-day fixes** — session-sync 0.2.12 (fork timestamps), permission-rules 0.6.15 (re-vendored auto-review 0.12.1), skill-pack-security 2.2.13 (v3-harness verify), and plugin-doctor pinned to 0.1.5 across 35 CI workflows.
- **Snapshot** — 892★ across 46 repos · 41 npm packages (35 bare + 6 scoped) · 573 versions · 90.3k downloads in Aug + Sep · 103 public Gitee mirrors.

### 2026-09-08 round

- **[dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor)** — a four-layer plugin health checker (package structure, Cordis contract, sandbox smoke, directory conformance), released on npm and wired into CI across 35 repos (now 0.1.6).
- **[dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) 0.11.0 → 0.12.1** — dual-line support for the `0.1.3-alpha.2` and `0.1.2-rc.1` harness lines with provenance publishing; its certification grade is **A**.
- **Cordis upstream** — open PR [#126](https://github.com/cordiverse/cordis/pull/126) (ship `src` in core/loader/timer tarballs, CI 8/8 green) and [schemastery issue #77](https://github.com/shigma/schemastery/issues/77); npm quality sweep (37 repos' badge fixes + a 532-tarball encoding audit, 35/35 re-published).

---

## 🚀 Flagship picks (start here)

| Plugin | What it gives you | Install |
|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | Second-model auto-review on the approval chain, fail-closed by default (150★) | `dsh plugin --profile web add dsh-auto-review` |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Claude Code-style declarative allow/deny/ask rules with session-log audit (113★) | `dsh plugin --profile web add dsh-permission-rules` |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | Approval-gated cross-session memory (`ctx.memory` + SQLite) (105★) | `dsh plugin --profile web add dsh-memento` |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | MCP management console: `/mcp` + Settings tab + trial calls (53★) | `dsh plugin --profile web add dsh-mcp-panel` |
| [dsh-checkpoint-rewind](https://github.com/PerryLink/dsh-checkpoint-rewind) | Claude Code `/rewind` equivalent: git-first snapshots, session forks, one-shot restore (16★) | `dsh plugin --profile web add dsh-checkpoint-rewind` |
| [dsh-autotier](https://github.com/PerryLink/dsh-autotier) | Automatic strong/cheap model-tier routing with deterministic risk guards and a `/tier` command (new) | `dsh plugin --profile web add dsh-autotier` |

One-command starter pack: **[dsh-kit](https://github.com/PerryLink/dsh-kit)** — installs the 37-plugin core family.

## 🔬 Research suite

| Plugin | What it gives you | npm |
|---|---|---|
| [dsh-research-report](https://github.com/PerryLink/dsh-research-report) | Verifiable research reports: content-addressed evidence ledger, manifest seal hash, byte-level citation checks, drift detection, disproof ledger | [npm](https://www.npmjs.com/package/dsh-research-report) |
| [dsh-fund-research](https://github.com/PerryLink/dsh-fund-research) | Chinese mutual-fund research with sealed, traceable snapshots — every number traces to a hashed source | [npm](https://www.npmjs.com/package/dsh-fund-research) |
| [dsh-industry-research](https://github.com/PerryLink/dsh-industry-research) | Industry/company research: chain-map SVG with bottleneck detection, timeline, company cards, adversarial review | [npm](https://www.npmjs.com/package/dsh-industry-research) |
| [dsh-data-quality](https://github.com/PerryLink/dsh-data-quality) | Deterministic data profiling/cleaning/verification: DAMA scorecard, content-hash dedupe, metric expectations | [npm](https://www.npmjs.com/package/dsh-data-quality) |

## 📦 The full family — 39 plugins by pillar

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

### 📊 Observability & cost (4)

| Plugin | One-liner | npm |
|---|---|---|
| [dsh-autotier](https://github.com/PerryLink/dsh-autotier) | Automatic strong/cheap model-tier routing with deterministic risk guards | [npm](https://www.npmjs.com/package/dsh-autotier) |
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

### 🛠️ Developer experience (4)

| Plugin | One-liner | npm |
|---|---|---|
| [dsh-lsp-actions](https://github.com/PerryLink/dsh-lsp-actions) | LSP diagnostics/formatting/completion/actions | [npm](https://www.npmjs.com/package/dsh-lsp-actions) |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | MCP management console | [npm](https://www.npmjs.com/package/dsh-mcp-panel) |
| [dsh-plugin-guide](https://github.com/PerryLink/dsh-plugin-guide) | Plugin-development knowledge base + CLI toolchain | [npm](https://www.npmjs.com/package/dsh-plugin-guide) |
| [dsh-plugin-upgrade](https://github.com/PerryLink/dsh-plugin-upgrade) | Plugin-author upgrade skill: version card + zero-dependency seam scanner (npx CLI) | [npm](https://www.npmjs.com/package/dsh-plugin-upgrade) |

*Support repos:* [dsh-plugin-kit](https://github.com/PerryLink/dsh-plugin-kit) (review-rule meta package) · [dsh-catalog](https://github.com/PerryLink/dsh-catalog) (DSH Desktop Market catalog source) · [dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) (certification MCP server) · [dsh-kit](https://github.com/PerryLink/dsh-kit) (one-command installer) · [dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) (plugin health checker)

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

## 🔧 Upstream & community contributions

- **[Cordis](https://github.com/cordiverse/cordis)** — the upstream plugin-core framework that powers DeepSeek Harness. Contributor: merged [PR #122](https://github.com/cordiverse/cordis/pull/122) (Windows + macOS CI, contributor badge) · 45-patch real-world regression suite + verification for the merged include-journal fix [PR #121](https://github.com/cordiverse/cordis/pull/121) · reported [issue #112](https://github.com/cordiverse/cordis/issues/112) with an initial fix ([PR #116](https://github.com/cordiverse/cordis/pull/116), superseded by #121) · open [issue #124](https://github.com/cordiverse/cordis/issues/124) (NodeNext type declarations, evidence + local fix) · open [PR #126](https://github.com/cordiverse/cordis/pull/126) (ship `src` in core/loader/timer tarballs, CI green) · 18-item errata for the [Cordis paper](https://arxiv.org/abs/2608.25512).
- **[schemastery](https://github.com/shigma/schemastery)** — the schema framework used across the DSH stack: filed [issue #77](https://github.com/shigma/schemastery/issues/77) (ESM/NodeNext consumption gap, full evidence + local fix branch).
- **[dsh-handbook](https://github.com/Electricitysheep/dsh-handbook)** — the official DSH handbook: two merged PRs ([#67](https://github.com/Electricitysheep/dsh-handbook/pull/67), [#68](https://github.com/Electricitysheep/dsh-handbook/pull/68)).
- **[dsh-wechat](https://github.com/pan17/dsh-wechat)** — cross-session PR [#4](https://github.com/pan17/dsh-wechat/pull/4) merged (v0.9.0).
- **Directory & hub submissions** — 35 plugins published on [DSH Directory](https://dsh.directory) (29 submission issues authored via [alexchenzl/dsh-plugin-directory](https://github.com/alexchenzl/dsh-plugin-directory)) · 149 open [Submission] issues tracked on the [omdsh hub](https://github.com/omdsh-dev/dsh-hub-workshop) · curated entries merged into [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin), [0xsline/awesome-deepseek-harness](https://github.com/0xsline/awesome-deepseek-harness), the [AdamPlatin123 radar](https://github.com/AdamPlatin123/dsh-plugin-radar), and [Zhiyuan-Fan's list](https://github.com/Zhiyuan-Fan/Awesome-DeepSeek-Harness-Plugins).

## 🌍 Where the plugins live

- **GitHub** (this profile) — source, CI, releases
- **[Gitee](https://gitee.com/perrylink)** — 103 public repos mirrored (branches + tags)
- **npm** — 41 packages published with CI provenance (35 bare + 6 scoped)
- **DSH Desktop Market** — add the catalog source `https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json` under Market → Sources to browse all 39 family packages in-app (curated summaries + icons, contract-validated, CI-smoked)

Listed on [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) (36 entries), [DSH Directory](https://dsh.directory/plugins/perrylink) (35 published), [Awesome DeepSeek Harness](https://github.com/0xsline/awesome-deepseek-harness), [awesome-deepseekharness](https://github.com/awesome-deepseekharness/awesome-deepseek-harness), [Zhiyuan-Fan's list](https://github.com/Zhiyuan-Fan/Awesome-DeepSeek-Harness-Plugins), the [AdamPlatin123 radar](https://github.com/AdamPlatin123/dsh-plugin-radar), [dsh-market](https://github.com/dsh-market/dsh-market) (via the awesome-dsh-plugin registry), [dsh-suite](https://github.com/whyihaveyou/dsh-suite), and [ZeroPointRepo's list](https://github.com/ZeroPointRepo/awesome-dsh-plugins). Auto-indexed on [deepseek1024.com](https://deepseek1024.com) (36 entries). Certification: [dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification).

## 中文介绍

我在 DeepSeek Harness 上把 Claude Code / Codex 生态里最实用的能力做成了开源插件:检查点回退、声明式权限、输出风格、跨会话记忆、MCP 面板、模型档位路由、微信/TickTick 桥接,以及可验证研究报告 / 基金研究 / 行业研究 / 数据质量「研究四件套」——共 **39 个插件**(Apache-2.0),全部带五语文档、CI、npm 发布与 Gitee 镜像。一键全家桶:[`dsh-kit`](https://github.com/PerryLink/dsh-kit)。同时我也是 DeepSeek Harness 上游核心框架 **Cordis**([cordiverse/cordis](https://github.com/cordiverse/cordis))的贡献者:Windows/macOS CI 已合并(#122),为 include-journal 修复(#121)提供了 45 个真实补丁文件的回归套件与验证,tarball 打包修复 PR(#126)与 NodeNext 类型声明 issue(#124)在途,并向 schemastery 提交了 ESM 消费面 issue(#77)。

2026-09-09 轮:① **dsh-autotier**——一天内从 0.1.0 走到 **0.2.0**:补齐 `0.1.5-alpha.1` 预发布 peer 线并新增请求期 provider/model 预检,随后交付浏览器半(Settings 卡 + 输入框档位胶囊,走 Typert Remote)、显式选型同步与多路由器并存检测,206 个用例全绿、Compat 双线矩阵全绿;② **dsh-plugin-upgrade 0.1.2**——插件作者升级技能:版本锁定迁移卡(`0.1.3-alpha.1 → 0.1.5-alpha.1`)+ 零依赖 seam 扫描器(V3 会话格式、`Inbox`、`ctx.agent`、PTC 改名等),以 bundle skill + npx CLI 交付;③ **发布卫生**——补齐全部 10 个缺失的 GitHub Release(缺口归零),逐包核对 `latest` 与仓库版本(39/40 一致,1 个 bump 在途),市场目录 39 项零滞后;④ **当日修复**——session-sync 0.2.12(fork 时间戳)、permission-rules 0.6.15(重 vendor auto-review 0.12.1)、skill-pack-security 2.2.13(v3 harness 校验)、plugin-doctor 在 35 个 CI 工作流统一钉 0.1.5;⑤ **快照**——家族 892★ / 46 仓、npm **41 包**(35 裸名 + 6 scoped)· 573 版、Aug+Sep 9.0 万下载、Gitee 公开镜像 103。

2026-09-08 轮:① **[dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) 发布**——四层插件体检器(包结构 / Cordis 契约 / 沙箱冒烟 / 目录一致性),已接入 35 仓 CI(现 0.1.6);② **dsh-auto-review 0.11.0 → 0.12.1**——双线支持 `0.1.3-alpha.2` 与 `0.1.2-rc.1`,带 provenance 发布,认证等级 **A**;③ **Cordis 上游**——tarball 打包修复 PR #126(CI 8/8 绿)在途,schemastery ESM issue #77 已投;④ npm 质量战役——37 仓徽章修复 + 全量 532 个 tarball 编码审计,35/35 重发对齐。

待业中。近期考虑给自己安排一次体检。因此最近将减少熬夜，后续的更新迭代节奏会适当放缓。当然，问题和缺陷修复不会停，只是发布频率会降低一些，还请大家谅解。
