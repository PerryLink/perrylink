# Hi, I'm PerryLink 👋

<!--
  Badge block: three centered groups, ordered links -> metrics -> listings.
  Every shields.io badge uses style=flat-square so the row reads as one set; the third-party
  badges in the last group are SVGs from their own sites and cannot be restyled.
  Live badges (GitHub stars / repos / followers, OpenSSF Scorecard, Glama) update themselves.
  Three stay hand-written because no live source exists for them: the plugin count, the 30-day
  npm download aggregate, and the third-party listing badges. Update those by hand when they move.
  The last row is also hand-written, and deliberately so: cla-assistant serves one generic
  signed/not_signed SVG and exposes no per-user query, so a CLA badge cannot be dynamic. Its two
  values were verified from the CLAassistant comment on each PR ("All committers have signed the
  CLA"). Re-check those comments before trusting the row after a new PR.
-->
<p align="center">
<a href="https://www.npmjs.com/search?q=perrylink"><img alt="npm packages" src="https://img.shields.io/badge/npm-packages-cb3837?logo=npm&style=flat-square"></a>
<a href="https://gitee.com/perrylink"><img alt="Gitee mirror" src="https://img.shields.io/badge/Gitee-mirror-0969da?logo=gitee&style=flat-square"></a>
<a href="https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json"><img alt="DSH Desktop Market" src="https://img.shields.io/badge/DSH_Desktop_Market-source-0969da?style=flat-square"></a>
</p>

<p align="center">
<a href="https://github.com/PerryLink?tab=repositories"><img alt="GitHub stars" src="https://img.shields.io/github/stars/PerryLink?label=stars&affiliations=OWNER&style=flat-square"></a>
<a href="https://github.com/PerryLink?tab=repositories"><img alt="GitHub repos" src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.github.com%2Fusers%2FPerryLink&query=%24.public_repos&label=repos&color=2da44e&style=flat-square"></a>
<a href="https://github.com/PerryLink?tab=followers"><img alt="GitHub followers" src="https://img.shields.io/github/followers/PerryLink?label=followers&style=flat-square"></a>
<img alt="plugins" src="https://img.shields.io/badge/plugins-41-6e7781?style=flat-square">
<img alt="npm downloads" src="https://img.shields.io/badge/npm_downloads-137k_30d-6e7781?style=flat-square">
</p>

<p align="center">
<a href="https://github.com/PerryLink/dsh-plugin-certification"><img alt="Certified dsh-auto-review" src="https://raw.githubusercontent.com/PerryLink/dsh-plugin-certification/main/badges/PerryLink__dsh-auto-review.svg"></a>
<a href="https://github.com/PerryLink/dsh-plugin-doctor#readme"><img alt="OpenSSF Scorecard" src="https://img.shields.io/ossf-scorecard/github.com/PerryLink/dsh-auto-review?label=openssf%20scorecard&style=flat-square"></a>
<a href="https://glama.ai/mcp/servers/PerryLink/jevcore"><img alt="Glama" src="https://glama.ai/mcp/servers/PerryLink/jevcore/badges/score.svg"></a>
</p>

<p align="center">
<a href="https://awesome-dsh-plugin.com"><img alt="awesome-dsh-plugin" src="https://awesome-dsh-plugin.com/badge.svg"></a>
<a href="https://dsh.directory/plugins?q=perrylink"><img alt="Listed on DSH Directory" src="https://dsh.directory/badges/listed.svg"></a>
<a href="https://dsh.market/?q=PerryLink"><img alt="DSH Market" src="https://raw.githubusercontent.com/2BingLing/dsh-market/master/assets/readme/badge-listed-en.svg"></a>
<a href="https://registry.modelcontextprotocol.io/v0/servers?search=perrylink"><img alt="MCP Registry" src="https://img.shields.io/badge/MCP_Registry-2_servers-6f42c1?style=flat-square"></a>
</p>

<p align="center">
<a href="https://github.com/alibaba/open-code-review/pull/1518"><img alt="open-code-review PR #1518, CLA signed" src="https://img.shields.io/badge/CLA_signed-open--code--review_%231518-2da44e?style=flat-square"></a>
<a href="https://github.com/bytedance/deer-flow/pull/5660"><img alt="deer-flow PR #5660, CLA signed" src="https://img.shields.io/badge/CLA_signed-deer--flow_%235660-2da44e?style=flat-square"></a>
</p>

**Building the [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness) plugin ecosystem: 41 open-source plugins in a 46-repo family (45 PerryLink-owned plus [pan17](https://github.com/pan17/dsh-wechat)'s dsh-wechat, Apache-2.0) — security, workflows, research, messaging bridges, developer experience — plus the DSH Desktop Market catalog, a plugin-certification registry and the dsh-plugin-doctor CI checker. Across the 45 PerryLink-owned repos, 44 ship CI and a Gitee mirror — the exception is [dsh-laya](https://github.com/PerryLink/dsh-laya), published tonight — 41 carry five-language docs, 44 declare the `dsh.bundle` contract, and 40 of the 49 active npm names carry a provenance attestation — 69.1k npm downloads in August plus 97.6k in September through the 20th (137.2k over the trailing 30 days). I also contribute upstream to [Cordis](https://github.com/cordiverse/cordis) — the plugin-core framework DeepSeek Harness is built on — and to [deepseek-ai](https://github.com/deepseek-ai) projects, including a merged [FlashMLA](https://github.com/deepseek-ai/FlashMLA) fix.**

DeepSeek Harness turned "everything is a plugin" into an ecosystem. I build the plugins I wish existed — engineering-discipline guardrails, runtime panels, cross-session memory, and verifiable research engines — and publish them the way production software deserves.

---

<!-- Round rotation: keep only the newest two rounds (current + one previous). Older rounds live in git history and can be restored on request. Rounds are narrative only — no Snapshot/counter lines: live counts belong to the badge row and "Where the plugins live", and per-edition copies go stale. GHSA/long-lived references belong in "Upstream & community contributions". -->

## 📣 Latest — 2026-09-21 round

- **[laya-mcp](https://github.com/PerryLink/laya-mcp) is a new project line: Laya typed decisions as an installable sidecar and an MCP server, next to [dsh-laya](https://github.com/PerryLink/dsh-laya), the DSH plugin that puts the same `noul`/`choice`/`score` questions behind a Cordis service and two model-visible tools.** Five repos — [layacore](https://github.com/PerryLink/layacore), [layacore-mcp](https://github.com/PerryLink/layacore-mcp), [layacore-install](https://github.com/PerryLink/layacore-install), [laya-mcp](https://github.com/PerryLink/laya-mcp) and [dsh-laya](https://github.com/PerryLink/dsh-laya) — went up between 20:03 and 20:16 local, and five npm names followed the same evening: `dsh-laya` 0.1.0 at 20:09, `layacore-install` and `layacore` at 20:09–20:10, `layacore-mcp` at 20:10, and `laya-mcp` reaching 0.1.1 by 21:01. **58 commits landed today** across 48 family repos plus this profile repo, all five new repos are Apache-2.0, and `dsh-laya` declares the `dsh.bundle` contract.
- **Why the split is the design, not an accident.** Laya is PyTorch and cannot live inside a Node plugin, so [dsh-laya](https://github.com/PerryLink/dsh-laya) **installs nothing and downloads nothing** — it is a client of a `laya-mcp serve` process you start yourself, and when that process is not running it says so instead of failing obscurely at the first tool call. It contributes one service (`ctx.laya`, with `ask`, `health`, `capabilities`, `sidecarUrl` and `loopback` — whether state stays on this machine, as a fact rather than a policy) plus `laya_ask` and `laya_plan` tools. The sidecar exists to buy the warm model: the cold build costs seconds to tens of seconds and the default lazy router rebuilds a checkpoint on every language switch.
- **Elsewhere the same day:** five PRs merged upstream — [dsh-genui](https://github.com/omdsh-dev/dsh-genui) #194 (run the lib cleanup in Node so Windows packing works), [dsh-advisor](https://github.com/omdsh-dev/dsh-advisor) #89 (Windows-safe prepare-release fixture), [ouroboros](https://github.com/Q00/ouroboros) #2427 (Getting Started links that 404'd from shipped skills), [dsh-web](https://github.com/zhu1090093659/dsh-web) #1657 and [beancookie/awesome-dsh-plugin](https://github.com/beancookie/awesome-dsh-plugin) #184 — and the first proposal went out to [laya](https://github.com/NandhaKishorM/laya) itself (★7,911): a report that a disclaimer footer sharing a paragraph makes `clean_email_body` delete the whole body, with the fix in the same PR.

### 2026-09-20 round

- **[jevcore](https://github.com/PerryLink/jevcore) is a new project: TypeSafe Jev for DeepSeek Harness and any other MCP host, as three packages — `jevcore` (the decision core, importing nothing from DSH or Cordis), `jevcore-dsh` (the DSH plugin: one service, three tools, two opt-in gates) and `jevcore-mcp` (the same three tools over MCP with a stdio binary). All of them reached npm today: 0.1.0 at 12:53, 0.1.1 at 13:06, and the core at 0.1.2 by 13:08.** The repo was created this afternoon and carries **38 commits in its first three hours** (10:14 to 13:08); it is Apache-2.0 and passes the `dsh.bundle` contract through `jevcore-dsh`.
- **Why it exists, and the guarantees it is built around.** Auditing the plugins that wire Jev into DSH found a consistent pattern the project's own README states plainly: the module labelled *guard*, *gate* or *warden* was also the one shipping prompts, tool arguments and file contents to a third party, and the README generally did not say so — several were on by default. jevcore designs those failure modes out: the default provider is an offline mock and the live path needs both `provider: live` **and** a resolved credential; every feature names its own transmission in one startup log line (`off`, or `SENDS <feature> { fields }`); a disabled gate registers **no** event listener at all, verified by test rather than by policy; no tool exposes gate configuration, so the model cannot widen its own constraints; and an undecided judgment resolves through explicit config, defaulting to `ask` instead of `allow`.
- **The evening before (09-19):** [dsh-plugin-upgrade](https://github.com/PerryLink/dsh-plugin-upgrade) **2.0.0** folded three retired corridor legs into one package with corridor-index routing (0.1.6-alpha.2 batch PRs and the published-line CI ruler also landed), [dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) **0.2.2** got onto the official MCP Registry, and **32 Releases across 27 family repos** went out — the rest of that wave was routine hygiene and dependency bumps.

---

## 🚀 Flagship picks (start here)

*The six most-starred family plugins (★ measured 2026-09-21); every other family repo is listed in full further down.*

| Plugin | What it gives you | Install |
|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | Second-model auto-review on the approval chain, fail-closed by default (189★) | `dsh plugin --profile web add dsh-auto-review` |
| [dsh-research-report](https://github.com/PerryLink/dsh-research-report) | Verifiable research reports: content-addressed evidence ledger, manifest seal hash, byte-level citation checks, drift detection, disproof ledger (146★) | `dsh plugin --profile web add dsh-research-report` |
| [dsh-industry-research](https://github.com/PerryLink/dsh-industry-research) | Industry/company research: chain-map SVG with bottleneck detection, timeline, company cards, adversarial review (146★) | `dsh plugin --profile web add dsh-industry-research` |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Claude Code-style declarative allow/deny/ask rules plus a process-level network policy (114★) | `dsh plugin --profile web add dsh-permission-rules` |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | Approval-gated cross-session memory (`ctx.memory` + SQLite) (108★) | `dsh plugin --profile web add dsh-memento` |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | MCP management console: `/mcp` + Settings tab + trial calls (62★) | `dsh plugin --profile web add dsh-mcp-panel` |

One-command starter pack: **[dsh-kit](https://github.com/PerryLink/dsh-kit)** — installs the core family in one command.

## 🔬 Research suite

| Plugin | What it gives you | npm |
|---|---|---|
| [dsh-research-report](https://github.com/PerryLink/dsh-research-report) | Verifiable research reports: content-addressed evidence ledger, manifest seal hash, byte-level citation checks, drift detection, disproof ledger | [npm](https://www.npmjs.com/package/dsh-research-report) |
| [dsh-fund-research](https://github.com/PerryLink/dsh-fund-research) | Chinese mutual-fund research with sealed, traceable snapshots — every number traces to a hashed source | [npm](https://www.npmjs.com/package/dsh-fund-research) |
| [dsh-industry-research](https://github.com/PerryLink/dsh-industry-research) | Industry/company research: chain-map SVG with bottleneck detection, timeline, company cards, adversarial review | [npm](https://www.npmjs.com/package/dsh-industry-research) |
| [dsh-data-quality](https://github.com/PerryLink/dsh-data-quality) | Deterministic data profiling/cleaning/verification: DAMA scorecard, content-hash dedupe, metric expectations | [npm](https://www.npmjs.com/package/dsh-data-quality) |

## 📦 The full family — 41 plugins + 5 support repos

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

### 🛠️ Developer experience (6)

| Plugin | One-liner | npm |
|---|---|---|
| [dsh-lsp-actions](https://github.com/PerryLink/dsh-lsp-actions) | LSP diagnostics/formatting/completion/actions | [npm](https://www.npmjs.com/package/dsh-lsp-actions) |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | MCP management console | [npm](https://www.npmjs.com/package/dsh-mcp-panel) |
| [dsh-plugin-guide](https://github.com/PerryLink/dsh-plugin-guide) | Plugin-dev knowledge base + CLI toolchain + release-engineering guide | [npm](https://www.npmjs.com/package/dsh-plugin-guide) |
| [dsh-plugin-upgrade](https://github.com/PerryLink/dsh-plugin-upgrade) | Plugin-author upgrade skill: one package, one corridor index that detects the caller's peer band and routes to the matching closed card (`0.1.3-alpha.1 → 0.1.5-rc.1`, `0.1.5-rc.2 → 0.1.6-alpha.2`), plus a zero-dependency seam scanner (bundle skill + npx CLI) | [npm](https://www.npmjs.com/package/dsh-plugin-upgrade) |
| [jevcore](https://github.com/PerryLink/jevcore) | TypeSafe Jev as typed decisions instead of prose (`noul`/`choice`/`score` with calibrated probabilities): offline by default, every transmission named before it happens, disabled gates register nothing (the DSH adapter `jevcore-dsh`, plus `jevcore` core and `jevcore-mcp` for non-DSH MCP hosts) | [npm](https://www.npmjs.com/package/jevcore-dsh) |
| [dsh-laya](https://github.com/PerryLink/dsh-laya) | Laya typed decisions (`noul`/`choice`/`score`) as a first-class Cordis service (`ctx.laya`) plus `laya_ask`/`laya_plan` tools; a client of a `laya-mcp serve` sidecar, so it installs and downloads nothing, and reports whether state stays on this machine as a fact rather than a policy | [npm](https://www.npmjs.com/package/dsh-laya) |

*Support repos:* [dsh-plugin-kit](https://github.com/PerryLink/dsh-plugin-kit) (review-rule meta package) · [dsh-catalog](https://github.com/PerryLink/dsh-catalog) (DSH Desktop Market catalog source) · [dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) (certification MCP server) · [dsh-kit](https://github.com/PerryLink/dsh-kit) (one-command installer) · [dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) (plugin health checker). Five repos publish under a `@perrylink/` npm name rather than their repo name — the support repos `@perrylink/dsh-plugin-kit` and `@perrylink/dsh-plugin-doctor`, and the plugins `@perrylink/dsh-github`, `@perrylink/dsh-ticktick` and `@perrylink/dsh-skill-pack-security-provider` — so the `perrylink` npm account holds 53 names while the family has 41 plugin repos.

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

*Every repo below is external to `PerryLink/*` and every number is measured: `★` from `gh api repos/<repo> --jq .stargazers_count`, commit counts from `GET /repos/<repo>/contributors` — so a contributor stays a contributor through squash merges and direct pushes. Measured 2026-09-21. Merged work and open proposals are listed separately and never mixed.*

**★ 1,000+ — named individually, as the rule requires.** Ten external repos above a thousand stars carry merged work:

- **[reactive-resume](https://github.com/reactive-resume/reactive-resume) (43,257★)** — merged [#3515](https://github.com/reactive-resume/reactive-resume/pull/3515): a Kubernetes self-hosting guide, plus a follow-up fix rejecting out-of-range months that rendered as `"undefined"` ([#3527](https://github.com/reactive-resume/reactive-resume/pull/3527), open).
- **[awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) (16,496★)** — 43 commits, 42 merged PRs, the ecosystem's largest curated index. The PerryLink family is listed there, and the listings are maintained rather than dumped: [#5459](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin/pull/5459) `dsh-cert-mcp`, [#5460](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin/pull/5460) `dsh-plugin-doctor`, [#5480](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin/pull/5480) `dsh-plugin-kit` and [#5527](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin/pull/5527) `dsh-plugin-upgrade` all merged on 2026-09-20.
- **[FlashMLA](https://github.com/deepseek-ai/FlashMLA) (12,953★)** — merged [PR #224](https://github.com/deepseek-ai/FlashMLA/pull/224) (2026-09-15), switching the 128-bit `st.async` PTX transport from `long2` to `longlong2` — on Windows (LLP64) the pair silently carried two 32-bit halves into an instruction expecting two 64-bit values. Two further MSVC-portability fixes are open ([#225](https://github.com/deepseek-ai/FlashMLA/pull/225), [#226](https://github.com/deepseek-ai/FlashMLA/pull/226)). This is the only merged pull request in the whole `deepseek-ai` org.
- **[Cordis](https://github.com/cordiverse/cordis) (8,721★)** — the upstream plugin-core framework that powers DeepSeek Harness. Contributor: merged [PR #122](https://github.com/cordiverse/cordis/pull/122) (Windows + macOS CI, contributor badge) · 45-patch real-world regression suite + verification contributed to the upstream-authored, merged include-journal fix [PR #121](https://github.com/cordiverse/cordis/pull/121) · reported [issue #112](https://github.com/cordiverse/cordis/issues/112) with an initial fix ([PR #116](https://github.com/cordiverse/cordis/pull/116), superseded by #121) · open [issue #124](https://github.com/cordiverse/cordis/issues/124) (NodeNext type declarations, evidence + local fix) · open [PR #126](https://github.com/cordiverse/cordis/pull/126) (ship `src` in core/loader/timer tarballs, CI green) · 18-item errata for the [Cordis paper](https://arxiv.org/abs/2608.25512).
- **[dsh-web](https://github.com/zhu1090093659/dsh-web) (7,896★)** — 6 commits, 4 merged PRs: the community web index now carries the family ([#1643](https://github.com/zhu1090093659/dsh-web/pull/1643), [#1647](https://github.com/zhu1090093659/dsh-web/pull/1647)), including a fix syncing a `dsh-genui` npm name with upstream ([#1657](https://github.com/zhu1090093659/dsh-web/pull/1657), merged 2026-09-21).
- **[ouroboros](https://github.com/Q00/ouroboros) (6,053★)** — 2 commits: a Chinese translation of the DeepSeek Harness guide ([#2400](https://github.com/Q00/ouroboros/pull/2400)) and a fix for two shipped skills whose relative `docs/getting-started.md` link 404'd from the installed skill ([#2427](https://github.com/Q00/ouroboros/pull/2427), merged 2026-09-21).
- **[deepseek-harness-desktop](https://github.com/dsh-tauri/deepseek-harness-desktop) (2,433★)** — 2 commits: a right-click paste double-insert race ([#508](https://github.com/dsh-tauri/deepseek-harness-desktop/pull/508), fixes #506) and five missing i18n keys in the application panel ([#632](https://github.com/dsh-tauri/deepseek-harness-desktop/pull/632)).
- **[dsh-plugin-radar](https://github.com/AdamPlatin123/dsh-plugin-radar) (1,464★)** — 46 commits, 48 merged PRs: the longest-running registry relationship here, opened 2026-08-14 and still maintained, plus status-evidence review issues such as [#768](https://github.com/AdamPlatin123/dsh-plugin-radar/issues/768).
- **[awesome-deepseek-harness](https://github.com/0xsline/awesome-deepseek-harness) (1,088★)** — 53 commits, 49 merged PRs, the highest commit count of any external repo: entries for the whole family, including the withdrawal of `dsh-personal-directive` at the author's request ([#615](https://github.com/0xsline/awesome-deepseek-harness/pull/615)).
- **[awesome-vibecoded-saas](https://github.com/Anil-matcha/awesome-vibecoded-saas) (1,019★)** — merged [#154](https://github.com/Anil-matcha/awesome-vibecoded-saas/pull/154): 13 family plugins across categories.

**The rest of the contributor set** (★ measured 2026-09-21; contributor confirmed by the `/contributors` endpoint): [dsh-handbook](https://github.com/Electricitysheep/dsh-handbook) (800★, 2 commits — the official DSH handbook, [#67](https://github.com/Electricitysheep/dsh-handbook/pull/67), [#68](https://github.com/Electricitysheep/dsh-handbook/pull/68)) · [goraven](https://github.com/8treenet/goraven) (734★, 1) · [Zhiyuan-Fan's list](https://github.com/Zhiyuan-Fan/Awesome-DeepSeek-Harness-Plugins) (567★, 5) · [dsh-genui](https://github.com/omdsh-dev/dsh-genui) (471★, 1) · [bruc3van/awesome-dsh-plugin](https://github.com/bruc3van/awesome-dsh-plugin) (351★, 11) · [Dominic789654's list](https://github.com/Dominic789654/awesome-deepseek-harness) (344★, 6) · [imsai-sh's catalog](https://github.com/imsai-sh/awesome-deepseek-harness-plugins) (246★, 40 — 40 commits in eight days) · [beancookie/awesome-dsh-plugin](https://github.com/beancookie/awesome-dsh-plugin) (150★, 14) · [Oh-My-DSH](https://github.com/like-study1/Oh-My-DSH) (86★, 3) · [walkinglabs' list](https://github.com/walkinglabs/awesome-deepseek-harness-plugins) (26★, 2) · [dsh-advisor](https://github.com/omdsh-dev/dsh-advisor) (22★, 1) · [awesome-deepseekharness](https://github.com/awesome-deepseekharness/awesome-deepseek-harness) (15★, 1) · [jiji262's list](https://github.com/jiji262/awesome-deepseek-harness) (14★, 1) · [vvlife's list](https://github.com/vvlife/awesome-deepseek-harness-plugins) (9★, 2) · [pan17/dsh-wechat](https://github.com/pan17/dsh-wechat) (8★, 2). **25 external repos in total; 268 merged pull requests outside `PerryLink/*`.**

**Open, and explicitly not counted as merged.** [cordiverse/http](https://github.com/cordiverse/http) [issue #14](https://github.com/cordiverse/http/issues/14) (README documents a `Response` wrapper `ctx.http()` no longer returns, with repo-verified line references) · [schemastery](https://github.com/shigma/schemastery) [issue #77](https://github.com/shigma/schemastery/issues/77) plus PRs [#78](https://github.com/shigma/schemastery/pull/78) and [#79](https://github.com/shigma/schemastery/pull/79) · [laya](https://github.com/NandhaKishorM/laya) [issue #93](https://github.com/NandhaKishorM/laya/issues/93) and PR [#94](https://github.com/NandhaKishorM/laya/pull/94) (★7,911) · [dsh-desktop](https://github.com/anywhere-labs/dsh-desktop) [PR #1101](https://github.com/anywhere-labs/dsh-desktop/pull/1101) (★28,246) · [koishi](https://github.com/koishijs/koishi) PRs [#1553](https://github.com/koishijs/koishi/pull/1553), [#1554](https://github.com/koishijs/koishi/pull/1554) · [agent-client-protocol](https://github.com/agentclientprotocol/agent-client-protocol) PRs [#2191](https://github.com/agentclientprotocol/agent-client-protocol/pull/2191), [#2192](https://github.com/agentclientprotocol/agent-client-protocol/pull/2192) · [EverOS](https://github.com/EverMind-AI/EverOS) [PR #447](https://github.com/EverMind-AI/EverOS/pull/447) · [slime](https://github.com/THUDM/slime) [PR #2396](https://github.com/THUDM/slime/pull/2396) · [checkpoint-engine](https://github.com/MoonshotAI/checkpoint-engine) [PR #108](https://github.com/MoonshotAI/checkpoint-engine/pull/108) · [Agents-Anywhere](https://github.com/anywhere-labs/Agents-Anywhere) [PR #131](https://github.com/anywhere-labs/Agents-Anywhere/pull/131) · [open-code-review](https://github.com/alibaba/open-code-review) (★38,997) [PR #1518](https://github.com/alibaba/open-code-review/pull/1518) (never anchor an inline comment to an old-file line number; CLA signed) · [deer-flow](https://github.com/bytedance/deer-flow) (★82,803) [PR #5660](https://github.com/bytedance/deer-flow/pull/5660) (bound `list_dir` so a stalled `find` cannot hold the sandbox lock; CLA signed) · [agent-browser](https://github.com/vercel-labs/agent-browser) (★42,990) [PR #1969](https://github.com/vercel-labs/agent-browser/pull/1969) (`batch` items bypassed the global-flag stripping every other path applies, so a flag's value was read as the URL — reproduced before/after on Windows) · [codex-security](https://github.com/openai/codex-security) (★10,818) [PR #986](https://github.com/openai/codex-security/pull/986) (run warnings never reached the SARIF projection; sealed into the coverage contract, with the sealed-vs-DB trade-off and the #978/#586 overlap flagged for the maintainer) · [deepsec](https://github.com/vercel-labs/deepsec) (★8,003) [PR #177](https://github.com/vercel-labs/deepsec/pull/177) (a `py-litestar-route` matcher — the one major Python web framework without one; all four CI gates run locally) · [teamai-cli](https://github.com/Tencent/teamai-cli) (★4,875) [PR #695](https://github.com/Tencent/teamai-cli/pull/695) (Qoder CN keeps its user directory at `~/.qoder-cn`, so a CN install synced nothing and users symlinked the two) · [docker-agent](https://github.com/docker/docker-agent) (★3,339) [PR #4372](https://github.com/docker/docker-agent/pull/4372) (`maxDefusePasses` justified its bound with an argument that is measurably false; the real invariant is the placeholder's character set — signed commits after review) · [tau](https://github.com/huggingface/tau) (★2,826) [PR #734](https://github.com/huggingface/tau/pull/734) (`--show-full-output` plus Ctrl+O revealing the untruncated TUI output behind the preview cap, with a stash-vs-changed regression comparison) · and 13 more open PRs across the `deepseek-ai` org ([DeepEP](https://github.com/deepseek-ai/DeepEP), [DeepGEMM](https://github.com/deepseek-ai/DeepGEMM), [3FS](https://github.com/deepseek-ai/3FS), [DeepSeek-MoE](https://github.com/deepseek-ai/DeepSeek-MoE), [DeepSeek-Prover-V1.5](https://github.com/deepseek-ai/DeepSeek-Prover-V1.5), [TileKernels](https://github.com/deepseek-ai/TileKernels), [deepseek-recipe](https://github.com/deepseek-ai/deepseek-recipe), [DeepSelect](https://github.com/deepseek-ai/DeepSelect), [awesome-deepseek-integration](https://github.com/deepseek-ai/awesome-deepseek-integration)).

**Security** — published advisory [GHSA-j922-p6h6-p255](https://github.com/PerryLink/dsh-permission-rules/security/advisories/GHSA-j922-p6h6-p255) for dsh-permission-rules (medium, patched in 0.6.16).

**Official harness repo** — it does not accept external pull requests (verified: `GET /repos/deepseek-ai/deepseek-harness/pulls` returns 404 and CONTRIBUTING.md says so, and `/contributors` does not list this account), so that line runs through issues, Discussions (the Show Your Plugins! post [#6104](https://github.com/deepseek-ai/deepseek-harness/discussions/6104)) and the plugin ecosystem instead — while the wider deepseek-ai org is open to fixes (FlashMLA #224 merged).

**Directory & hub submissions** — 33 plugins published on [DSH Directory](https://dsh.directory) (every `/plugins/PerryLink/<name>` page probed; 29 submission issues authored via [alexchenzl/dsh-plugin-directory](https://github.com/alexchenzl/dsh-plugin-directory), all 29 since closed) · 153 open [Submission] issues tracked on the [omdsh hub](https://github.com/omdsh-dev/dsh-hub-workshop), 114 of them filed from here · and registry entries merged into the curated lists named above.

## 🌍 Where the plugins live

- **GitHub** (this profile) — source, CI, releases; **1,295★ across all 200 public repos, 1,224★ of it in the 46-repo family** (41 plugins + 5 support repos; the 45 PerryLink-owned ones are 1,216★, the other 8★ is [pan17/dsh-wechat](https://github.com/pan17/dsh-wechat)), 44 of the PerryLink-owned repos declaring the `dsh.bundle` contract and 41 of the 45 carrying five-language docs. The stars/repos/followers badges above are live, so this line is the one measured figure; the badges will drift ahead of it between refreshes
- **[Gitee](https://gitee.com/perrylink)** — 106 public repos: 44 of the 45 family repos are mirrored (default branch + all tags, not every branch) alongside mirrors of other projects — [dsh-laya](https://github.com/PerryLink/dsh-laya) is the exception, created after the daily sync had run; the upgrade corridor is mirrored there as `dsh-plugin-upgrade`
- **npm** — the `perrylink` account holds **53 names, 770 versions (804 with pan17's dsh-wechat)**: 49 active (44 unscoped + 5 scoped) and 4 deprecated old names still on the registry (the retired corridor legs `dsh-plugin-upgrade-rc1` and `dsh-plugin-upgrade-015`, the withdrawn `dsh-personal-directive`, and the retired scoped `@perrylink/dsh-cert-mcp`, renamed to the unscoped `dsh-cert-mcp`). 40 of the 49 active names carry a provenance attestation on their current latest version — the nine without one are `@perrylink/dsh-plugin-doctor`, the three jevcore packages (`jevcore` / `jevcore-dsh` / `jevcore-mcp`) and the five laya-family names published tonight; across all 53 names the attestation count is 44
- **npm downloads** — 69.1k in August plus 97.6k in September through the 20th, **137.2k over the trailing 30 days** (npm window 08-22..09-20, the last day the daily series covers — it zeroes out 09-03, 09-07, 09-08, 09-15, 09-17 and 09-21). The 48 established PerryLink names alone are 63.9k / 94.8k / 132.3k; the five laya-family names published tonight have no download series yet
- **DSH Desktop Market** — add the catalog source `https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json` under Market → Sources to browse the family in-app (41 catalog entries with curated summaries + icons, contract-validated, CI-smoked)
- **MCP Registry** — two servers are on the official registry, both published from their release workflows over GitHub OIDC: [`io.github.PerryLink/dsh-cert`](https://registry.modelcontextprotocol.io/v0/servers?search=perrylink) v0.2.2 (npm `dsh-cert-mcp`) and `io.github.PerryLink/jevcore` v0.4.1 (npm `jevcore-mcp`) — note both are indexed under the server name, not the package name
- **GitHub Actions** — [dsh-github](https://github.com/PerryLink/dsh-github) and [dsh-test-drive](https://github.com/PerryLink/dsh-test-drive) also ship composite actions, so they install as `uses: PerryLink/dsh-test-drive@vX`

Listed on [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) (42 entry files under `data/plugins/PerryLink__*`), [DSH Directory](https://dsh.directory/plugins?q=perrylink) (33 plugin pages published; its own `q=perrylink` view surfaces 24), [walkinglabs' plugin list](https://github.com/walkinglabs/awesome-deepseek-harness-plugins) (Developer Tooling: [dsh-plugin-guide](https://github.com/PerryLink/dsh-plugin-guide), [dsh-test-drive](https://github.com/PerryLink/dsh-test-drive) and the upgrade corridor), [Awesome DeepSeek Harness](https://github.com/0xsline/awesome-deepseek-harness), [awesome-deepseekharness](https://github.com/awesome-deepseekharness/awesome-deepseek-harness), [Zhiyuan-Fan's list](https://github.com/Zhiyuan-Fan/Awesome-DeepSeek-Harness-Plugins), the [AdamPlatin123 radar](https://github.com/AdamPlatin123/dsh-plugin-radar), [dsh-market](https://github.com/dsh-market/dsh-market) (via the awesome-dsh-plugin registry), [dsh-suite](https://github.com/whyihaveyou/dsh-suite), and [ZeroPointRepo's list](https://github.com/ZeroPointRepo/awesome-dsh-plugins). Auto-indexed on [deepseek1024.com](https://deepseek1024.com) (43 plugin pages — its sitemap also indexes three fixture subpaths as if they were plugins, and still carries the withdrawn `dsh-personal-directive` and the retired `dsh-plugin-upgrade-015`), also indexed on [dshfind.com](https://dshfind.com/zh/plugins/PerryLink/dsh-memento) — a third-party DSH plugin supermarket with per-plugin score badges — and on [Glama](https://glama.ai/mcp/servers/PerryLink/dsh-cert-mcp), and further catalogued by [DSH Get](https://dshget.com), [chnjames/dsh-plugin-market](https://github.com/chnjames/dsh-plugin-market) and [NoWint/Oh-My-DSH](https://github.com/NoWint/Oh-My-DSH) — the GitHub [`dsh-plugin` topic](https://github.com/topics/dsh-plugin) (55 PerryLink repos tagged, all 45 family repos among them) is what most of them ingest from. Scored on [OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/PerryLink/dsh-auto-review) — **40 of the 45 family repos carry a scorecard result** (3.5–5.6, measured 2026-09-21), and 39 of them now show the scorecard badge in their README; the five without a result are [dsh-laya](https://github.com/PerryLink/dsh-laya), [dsh-ticktick](https://github.com/PerryLink/dsh-ticktick), [dsh-catalog](https://github.com/PerryLink/dsh-catalog), [dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) and [dsh-kit](https://github.com/PerryLink/dsh-kit). Certification: [dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification) (spec + registry, 1 family repo certified so far).

## 中文介绍

我在 DeepSeek Harness 上把自己希望存在的插件做了出来:检查点回退、声明式权限、输出风格、跨会话记忆、MCP 面板、模型档位路由、微信/TickTick 桥接,以及可验证研究报告 / 基金研究 / 行业研究 / 数据质量「研究四件套」——共 **41 个插件**(Apache-2.0):全部带 CI 与 Gitee 镜像,45 个 PerryLink 自有家族仓中有 41 个带五语文档、44 个声明 `dsh.bundle` 契约。`perrylink` 这个 npm 账号下共有 **53 个名称、770 个版本**(含 pan17 的 dsh-wechat 为 54 个名称、804 个版本):49 个在用(44 个非 scoped + 5 个 scoped)+ 4 个弃用旧名;在用的 49 个里有 40 个当前 latest 版本带 provenance 证明(9 个没有:`@perrylink/dsh-plugin-doctor`、jevcore 三包,以及今晚刚发布的 laya 五包),53 个名称合计 44 个带证明。下载量 8 月 69.1k + 9 月截至 20 日 97.6k(近 30 天 137.2k,窗口 08-22..09-20;npm 日序列在 09-03、09-07、09-08、09-15、09-17、09-21 归零);48 个既有 PerryLink 名称单独算是 63.9k / 94.8k / 132.3k。一键全家桶:[`dsh-kit`](https://github.com/PerryLink/dsh-kit)。同时我是 DeepSeek Harness 上游核心框架 **Cordis**([cordiverse/cordis](https://github.com/cordiverse/cordis))的贡献者,也是 [deepseek-ai](https://github.com/deepseek-ai) 官方仓贡献者:[FlashMLA](https://github.com/deepseek-ai/FlashMLA) 的修复已合并(#224),这是该组织下唯一一条已合并的外部 PR;此外还有 10 个「千星以上」外部仓的已合并贡献(见上方 Upstream 一节,含逐仓星数与提交数)。

2026-09-21 轮:① **[laya-mcp](https://github.com/PerryLink/laya-mcp) 是一条新战线:把 Laya 的定型决策做成可安装的 sidecar 与 MCP server,旁边是 [dsh-laya](https://github.com/PerryLink/dsh-laya) —— 把同样的 `noul`/`choice`/`score` 问题放进一个 Cordis service 和两个模型可见的 tool。** 五个仓([layacore](https://github.com/PerryLink/layacore)、[layacore-mcp](https://github.com/PerryLink/layacore-mcp)、[layacore-install](https://github.com/PerryLink/layacore-install)、[laya-mcp](https://github.com/PerryLink/laya-mcp)、[dsh-laya](https://github.com/PerryLink/dsh-laya))在 20:03–20:16 之间上线,五个 npm 名称当晚跟进:`dsh-laya` 0.1.0 于 20:09,`layacore-install` 与 `layacore` 于 20:09–20:10,`layacore-mcp` 于 20:10,`laya-mcp` 到 21:01 已到 0.1.1。当天 **49 个家族仓共 58 次提交**,五个新仓都是 Apache-2.0,`dsh-laya` 通过 `dsh.bundle` 契约。
② **为什么必须拆开,而不是顺手装。** Laya 是 PyTorch,不可能塞进 Node 插件里,所以 [dsh-laya](https://github.com/PerryLink/dsh-laya) **什么都不装、什么都不下** —— 它是你自己启动的 `laya-mcp serve` 进程的客户端;那个进程没在跑时它会直说,而不是在第一次 tool 调用时莫名其妙地失败。它给出一个 service(`ctx.laya`,含 `ask`、`health`、`capabilities`、`sidecarUrl`、`loopback` —— 「状态是否留在这台机器上」是事实,不是策略)外加 `laya_ask` / `laya_plan` 两个 tool。sidecar 存在的意义是买到热模型:冷启动要几秒到几十秒,而默认的懒路由每换一次语言就重建一次 checkpoint。
③ **同一天还有 5 条上游 PR 合并**:[dsh-genui](https://github.com/omdsh-dev/dsh-genui) #194(把 lib 清理挪进 Node,Windows 打包才成立)、[dsh-advisor](https://github.com/omdsh-dev/dsh-advisor) #89(prepare-release 夹具改成 Windows 安全)、[ouroboros](https://github.com/Q00/ouroboros) #2427(随 skill 发布的 Getting Started 链接 404)、[dsh-web](https://github.com/zhu1090093659/dsh-web) #1657、[beancookie/awesome-dsh-plugin](https://github.com/beancookie/awesome-dsh-plugin) #184;同时给 [laya](https://github.com/NandhaKishorM/laya) 本体(★7,911)发了第一条提案:免责声明页脚与会话正文同段时 `clean_email_body` 会整段删掉正文,同 PR 附修复。

### 2026-09-20 轮

① **[jevcore](https://github.com/PerryLink/jevcore) 是新项目:把 TypeSafe Jev 接进 DeepSeek Harness 与任何其他 MCP host,拆成三个包——`jevcore`(决策内核,不 import 任何 DSH/Cordis 东西)、`jevcore-dsh`(DSH 插件:一个 service、三个 tool、两道 opt-in 门)、`jevcore-mcp`(同样三个 tool 走 MCP,带 stdio 二进制)。三个包今天全部上了 npm:12:53 发 0.1.0,13:06 发 0.1.1,内核已于 13:08 到 0.1.2。** 仓库今天下午新建,头三小时(10:14–13:08)就有 **38 次提交**;MIT,并由 `jevcore-dsh` 通过 `dsh.bundle` 契约。
② **它为什么存在,以及围绕什么保证来写。** 审计那些把 Jev 接进 DSH 的插件后,发现一个被项目自己 README 直说的规律:标着 *guard*、*gate*、*warden* 的那个模块,恰好也是把 prompt、tool 参数和文件内容发往第三方的模块,而 README 一般不说——其中有几个还是默认开启的。jevcore 把这些失效模式设计掉:默认 provider 是离线 mock,走活线要**同时**满足 `provider: live` 与已解析的凭据;每个功能都在启动日志里自报是否外发(`off`,或 `SENDS <feature> { fields }`);被关掉的门**不注册任何**事件监听器,由测试而非策略来保证;没有任何 tool 暴露门的配置,所以模型无法放宽自己的约束;判不出来时走显式配置,默认落到 `ask` 而不是 `allow`。
③ **前一天晚上(09-19)的其他事**:[dsh-plugin-upgrade](https://github.com/PerryLink/dsh-plugin-upgrade) **2.0.0** 把三条已退役的走廊腿折成一个包 + 走廊索引路由(0.1.6-alpha.2 批量 PR 与「已发布线」CI 尺子同时落地)、[dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) **0.2.2** 进入官方 MCP Registry,当晚共 **27 个家族仓 32 个 Release**;其余为例行卫生与依赖升级。

待业中。近期考虑给自己安排一次体检。因此最近将减少熬夜，后续的更新迭代节奏会适当放缓。当然，问题和缺陷修复不会停，只是发布频率会降低一些，还请大家谅解。
