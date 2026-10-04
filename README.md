# Hi, I'm PerryLink 👋

<!--
  Badge block: three centered rows, one badge per source line. The leading whitespace between the
  inline <a>/<img> tags collapses when GitHub renders the <p>, and the single <br> after each row
  forces the row break, so the layout is three rows regardless of how the source is wrapped.

  Order is recognition first, source second. Row 1 is the reach a visitor reads first: the GitHub
  trio (stars, followers, repos), then the two third-party scores (OpenSSF Scorecard, Glama), then
  the npm pair (packages, 30-day downloads). Row 2 is where the work is published and listed: the
  official MCP Registry, the curated awesome list, DSH Directory, DSH Market, the Gitee mirror.
  Row 3 is the DSH community footprint and the self-issued badges: the dshfind pair, the Desktop
  Market catalog source, the certification, the plugin count. Same-source badges stay adjacent --
  the GitHub trio, the npm pair, the dshfind pair -- and OpenSSF Scorecard sits next to Glama
  because both are third-party scores rather than listings; nothing here is restyled, badges only
  moved, so every colour is the source's own.

  The rows are partitioned to near-equal width, and that is measured, not assumed. Re-measured
  2026-10-04 from each badge's own SVG width/height at the 20px render height: 17 badges totalling
  2414px, split 797 / 811 / 806 (range 14) by a search over the row breaks, every row inside
  GitHub's ~888px README content column. Per badge, in that order: stars 90, followers 106, repos
  72, openssf scorecard 136, glama 110, npm packages 113, npm downloads 170, MCP Registry 144,
  awesome 168, DSH Directory 218, DSH Market 180, Gitee 101, dshfind 174, dshfind downloads 256,
  Desktop Market 172, certified 132, plugins 72. Of the three label edits this round, two are
  width-neutral (plugins 42 -> 42, npm downloads 134.9k -> 158.6k) and only the dshfind aggregate
  moved, 246 -> 256; re-solving the split after that move returns the same three row breaks, so the
  partition stands rather than being re-invented. The repos badge is a
  dynamic/json badge and was serving its "invalid" state (86px) at an earlier measure; as
  "repos: 211" it renders 72px, which fits the same partition -- both states fit the column and
  neither row order changes. If you add or remove a badge the total changes and this partition is
  lost: re-solve it rather than appending to a row, and re-measure the widths -- do not reuse these
  numbers after a label change, since a single label edit shifts a row.

  The dshfind entries: the plain dshfind badge is dshfind's own per-repo badge and links a specific
  plugin, so it can only show that repo's figure. dshfind publishes no owner-level badge and its API
  has no downloads field at all (listing, detail and GraphQL alike -- the figure exists only inside
  the rendered SVG, rounded to tiers such as "5k+"). The aggregate badge is therefore hand-written
  from the sum of every PerryLink badge's own rendered tier. Tiers are lower bounds, so "21k+" is a
  floor, and only the plugins dshfind currently renders a download figure for are counted (6 of the
  49 it indexes -- 5k+5k+5k+2k+2k+2k, re-summed 2026-09-24; two plugins that carried a figure last
  round now render their star count instead, which is why the badge moved 22k+ -> 21k+ and
  "8 plugins" -> "6 plugins" without any download falling): that is what "across 6 plugins" states.
  Re-summed 2026-10-04: dshfind now renders a download figure for 7 of the plugins it indexes --
  the six that carried one last round (5k+5k+5k+2k+2k+2k) plus dsh-plugin-guide at 500+ -- so the
  badge moved 21k+ across 6 -> 21.5k+ across 7. Tiers are lower bounds and the 500+ one is no
  exception, so "21.5k+" is a floor too. Re-sum it when dshfind reports more.

  Vertical spacing: the three rows are ONE <p>, not three, joined by <br>. Three separate <p>
  blocks each pay GitHub's 16px paragraph margin, and a 20px image also shows the font's descent
  under the text baseline, so the gap was measured ink-to-ink at 21px on the live profile (16px
  margin + ~5px descent). One <p> drops the margin and leaves the descent alone: re-measured on
  that page after the change, 5px. The profile renders this README at 14px/21px while the file view
  uses 16px/24px, so anything tied to the line box lands differently on each surface: align="top"
  on the images measured 1px on the profile against 4px in the file view and was left off.
  Re-measure both surfaces before touching this, and do not add align to tighten it further.

  Conventions are matched to the family, not invented here. Survey of the family READMEs found the
  shields.io badges on the default `flat` style, so no badge here sets a style either. The Gitee
  badge keeps the family's red c71d23; the npm badge keeps npm's cb3837. Labels use real spaces.
  The third-party badges are SVGs served by their own sites and cannot be restyled.
  Live badges (GitHub stars / repos / followers, OpenSSF Scorecard, Glama) update themselves.
  Four stay hand-written because no live source exists for them: the plugin count, the 30-day npm
  download aggregate, the dshfind aggregate, and the third-party listing badges. Update those by
  hand when they move. The repo/star/download figures this block used to mirror now live in
  "Where the plugins live"; the badge row is the live copy and the text there is the measured one.
-->
<p align="center">
<a href="https://github.com/PerryLink?tab=repositories"><img alt="GitHub stars" src="https://img.shields.io/github/stars/PerryLink?label=stars&affiliations=OWNER&color=24292f"></a>
<a href="https://github.com/PerryLink?tab=followers"><img alt="GitHub followers" src="https://img.shields.io/github/followers/PerryLink?label=followers&color=24292f"></a>
<a href="https://github.com/PerryLink?tab=repositories"><img alt="GitHub repos" src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.github.com%2Fusers%2FPerryLink&query=%24.public_repos&label=repos&color=24292f"></a>
<a href="https://github.com/PerryLink/dsh-plugin-doctor#readme"><img alt="OpenSSF Scorecard" src="https://img.shields.io/ossf-scorecard/github.com/PerryLink/dsh-auto-review?label=openssf%20scorecard"></a>
<a href="https://glama.ai/mcp/servers/PerryLink/jevcore"><img alt="Glama" src="https://glama.ai/mcp/servers/PerryLink/jevcore/badges/score.svg"></a>
<a href="https://www.npmjs.com/search?q=perrylink"><img alt="npm packages" src="https://img.shields.io/badge/npm-packages-cb3837?logo=npm"></a>
<img alt="npm downloads 30d" src="https://img.shields.io/badge/npm%20downloads%2030d-158.6k-6e7781">
<br>
<a href="https://registry.modelcontextprotocol.io/v0/servers?search=perrylink"><img alt="MCP Registry" src="https://img.shields.io/badge/MCP%20Registry-3%20servers-6f42c1"></a>
<a href="https://awesome-dsh-plugin.com"><img alt="awesome-dsh-plugin" src="https://awesome-dsh-plugin.com/badge.svg"></a>
<a href="https://dsh.directory/plugins?q=perrylink"><img alt="Listed on DSH Directory" src="https://dsh.directory/badges/listed.svg"></a>
<a href="https://dsh.market/?q=PerryLink"><img alt="DSH Market" src="https://raw.githubusercontent.com/2BingLing/dsh-market/master/assets/readme/badge-listed-en.svg"></a>
<a href="https://gitee.com/perrylink"><img alt="Gitee mirror" src="https://img.shields.io/badge/Gitee-mirror-c71d23?logo=gitee"></a>
<br>
<a href="https://dshfind.com/plugins/PerryLink/dsh-auto-review?ref=badge"><img alt="dshfind" src="https://dshfind.com/api/badge/PerryLink/dsh-auto-review?metric=downloads"></a>
<a href="https://dshfind.com/plugins?q=PerryLink"><img alt="dshfind downloads across the family" src="https://img.shields.io/badge/dshfind%20downloads-21.5k%2B%20across%207%20plugins-6e7781"></a>
<a href="https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json"><img alt="DSH Desktop Market source" src="https://img.shields.io/badge/DSH%20Desktop%20Market-source-0969da"></a>
<a href="https://github.com/PerryLink/dsh-plugin-certification"><img alt="Certified dsh-auto-review" src="https://raw.githubusercontent.com/PerryLink/dsh-plugin-certification/main/badges/PerryLink__dsh-auto-review.svg"></a>
<img alt="plugins" src="https://img.shields.io/badge/plugins-42-6e7781">
</p>

**Building the [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness) plugin ecosystem: 42 open-source plugins in a 48-repo family, 47 of them PerryLink-owned — security, workflows, research, messaging bridges, developer experience — plus the DSH Desktop Market catalog, a plugin-certification registry and the dsh-plugin-doctor CI checker. All 42 ship CI and a Gitee mirror, five-language docs held to the same section count, install command and configuration keys by a gate in each repo's own CI, and the `dsh.bundle` contract; 158,593 npm downloads over the trailing 30 days. I also contribute upstream to [Cordis](https://github.com/cordiverse/cordis) — the plugin-core framework DeepSeek Harness is built on — and to [deepseek-ai](https://github.com/deepseek-ai) projects, including a merged [FlashMLA](https://github.com/deepseek-ai/FlashMLA) fix.**

DeepSeek Harness turned "everything is a plugin" into an ecosystem. I build the plugins I wish existed — engineering-discipline guardrails, runtime panels, cross-session memory, and verifiable research engines — and publish them the way production software deserves.

Outside the family: **43 external repositories carry a merged pull request of mine together with a commit attributed to this account, and 20 of them are above a thousand stars** — Tencent's `teamai-cli`, DeepSeek's FlashMLA, cordiverse's Cordis, the ACP repositories Zed and JetBrains jointly govern, ruvnet's `ruflo`, and the DSH catalogs — part of the **348 merged pull requests** this account has outside `PerryLink/*`. The measurements behind the family's own judgment layer are published as a paper with a DOI: [*When a Judgment Layer's Self-Reported Fields Lie*](https://doi.org/10.5281/zenodo.22901853), a three-layer measurement (Laya, TypeSafe Jev, DeepSeek-V4.1-Flash) run on [laya-mcp](https://github.com/PerryLink/laya-mcp) and [jevcore](https://github.com/PerryLink/jevcore), with a [Chinese translation](https://doi.org/10.5281/zenodo.22902025) and the [artifact](https://doi.org/10.5281/zenodo.22901248) archived separately.

---

<!-- Round rotation: keep only the newest two rounds (current + one previous). Older rounds live in git history and can be restored on request. Rounds are narrative only — no Snapshot/counter lines: live counts belong to the badge row and "Where the plugins live", and per-edition copies go stale. GHSA/long-lived references belong in "Upstream & community contributions".

     ROUND COUNT, 2026-10-04: both blocks carry two rounds -- 10-04 (current) and
     09-25 (previous). The 09-24 round rotated out to git history by the rule above.
     The 10-04 round is a re-measurement report, so it reads as finding -> correction
     rather than as a list of commits: the window held 29 releases (all on 09-25) and
     16 commits, of which 10 are the doctor's daily badge refresh, so the round's news
     is what re-measuring changed, not what shipped. Every figure in it is dated. The
     09-25 round is kept verbatim, because a round is a dated snapshot and its counters
     are that round's, not the page's. Earlier rounds (09-24, 09-23, 09-22, 09-21,
     09-20) live in git history; the 09-21 round was where laya-mcp and dsh-laya were
     introduced by name, and dsh-laya still has its family-table row (the sidecar
     design lives there) while laya-mcp carries a clause in the page intro. -->

## 📣 Latest — 2026-10-04

- **The page said 36 external repositories carried my work; the same probe, run under the same rule, now returns 43 — and laya has no open pull requests at all.** Every external repository this account ever opened a pull request against (106 of them) was probed again with `/contributors`: **43 carry a commit attributed to this account, 20 of them above a thousand stars**, and the merged count outside `PerryLink/*` is **348**, up from 321. Five of the thousand-star rows are new since the last measurement — `ruvnet/ruflo` (73,833★), `walkinglabs/learn-harness-engineering` (18,892★), `dsh-market/dsh-market` (5,490★), `punkpeye/fastmcp` (3,272★) and `Anil-matcha/awesome-vibecoded-saas` (1,036★) — while `yibie/awesome-jev` moved the other way, from "merged but uncredited" to a contributor row (2,120★). The correction matters more than the growth: the page had been listing **14 pull requests as still open at laya**, and reading the repository's own pull-request connection shows **47 opened, 45 merged, 2 closed unmerged, 0 open** — those fourteen merged on 09-27 and 09-29, in two batches of eight, and the section below now says so.

- **The npm figures were re-derived name by name instead of carried forward, and the page had been overstating them.** The old line read **56 names, 917 versions, 49 active, 42 with provenance**; probing the registry directly — the search index alone is not enough, since it returns 47 names and silently omits the deprecated ones — gives **52 names, 909 versions, 46 whose `latest` is not deprecated, and 44 carrying a provenance attestation on that version**. Over the trailing 30 days the account served **158,593 downloads in the npm window 09-04..10-03**, against 134,856 in 08-23..09-21. The six scoped `@perrylink/*` names and the six deliberate deprecations both re-derived unchanged.

- **The one thing in the family that moved every single day of the window was the verification artifact.** [dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) committed ten times between 09-25 and 10-04, each one `chore: refresh verified badges` rewriting `data/verified.json` (+122/-122) against the live GitHub API — a dated, machine-generated record of which repos still pass the zero-dependency R+K static gate on their current default-branch HEAD. Everything else in the window is 29 releases published on 09-25 itself, the repackaging pass that followed the `0.1.7-rc.2` move the previous round reported, and no repository outside the doctor has been pushed since.

### 2026-09-25 round

## 🚀 Flagship picks (start here)

*The six most-starred family plugins (★ measured 2026-10-04); every other family repo is listed in full further down, and the research four-piece set is under [Research](#-research-4).*

| Plugin | What it gives you | Install |
|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | Second-model auto-review on the approval chain, fail-closed by default (228★) | `dsh plugin --profile web add dsh-auto-review` |
| [dsh-research-report](https://github.com/PerryLink/dsh-research-report) | Verifiable research reports: content-addressed evidence ledger, manifest seal hash, byte-level citation checks, drift detection, disproof ledger (214★) | `dsh plugin --profile web add dsh-research-report` |
| [dsh-industry-research](https://github.com/PerryLink/dsh-industry-research) | Industry/company research: chain-map SVG with bottleneck detection, timeline, company cards, adversarial review (207★) | `dsh plugin --profile web add dsh-industry-research` |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | Approval-gated cross-session memory (`ctx.memory` + SQLite) (138★) | `dsh plugin --profile web add dsh-memento` |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Claude Code-style declarative allow/deny/ask rules plus a process-level network policy (117★) | `dsh plugin --profile web add dsh-permission-rules` |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | MCP management console: `/mcp` + Settings tab + trial calls (74★) | `dsh plugin --profile web add dsh-mcp-panel` |

One-command starter pack: **[dsh-kit](https://github.com/PerryLink/dsh-kit)** — installs the core family in one command.

## 📦 The full family — 42 plugins + 5 support repos

*Counting note: "42 plugins" counts every repo that declares `dsh.bundle.patch`, re-derived one repo at a time on 2026-10-04 by reading each repo's own `package.json` at its default branch. Measured against the 47 PerryLink-owned repositories this page names: **42 declare the contract and 5 do not** — the support trio [dsh-catalog](https://github.com/PerryLink/dsh-catalog), [dsh-kit](https://github.com/PerryLink/dsh-kit) and [dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification) (the certification registry, whose MCP server publishes from [dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) instead), plus [jevcore](https://github.com/PerryLink/jevcore) (no `dsh.bundle`; only its `jevcore-dsh` workspace member is a plugin) and [laya-mcp](https://github.com/PerryLink/laya-mcp) (an MCP sidecar, not a plugin). The third-party [pan17/dsh-wechat](https://github.com/pan17/dsh-wechat) carries a plugin row but is not one of them: 47 + 1 = the 48 repos this page names. A naive scan of the account finds two more than the heading claims — the retired [dsh-plugin-upgrade](https://github.com/PerryLink/dsh-plugin-upgrade) corridor legs `dsh-plugin-upgrade-015` and `dsh-plugin-upgrade-016`, both archived, both still carrying the manifest, and neither an active plugin: 42 active + 2 retired = the 44 such a scan returns. The heading and the badge keep the active figure.*

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

*Support repos:* [dsh-plugin-kit](https://github.com/PerryLink/dsh-plugin-kit) (review-rule meta package) · [dsh-catalog](https://github.com/PerryLink/dsh-catalog) (DSH Desktop Market catalog source) · [dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) (certification MCP server) · [dsh-kit](https://github.com/PerryLink/dsh-kit) (one-command installer) · [dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) (plugin health checker). Five of these repos and plugins publish under a `@perrylink/` npm name rather than their repo name — the support repos `@perrylink/dsh-plugin-kit` and `@perrylink/dsh-plugin-doctor`, and the plugins `@perrylink/dsh-github`, `@perrylink/dsh-ticktick` and `@perrylink/dsh-skill-pack-security-provider` — and a sixth name, `@perrylink/dsh-cert-mcp`, is the deprecated scoped predecessor of `dsh-cert-mcp`; the `perrylink` account therefore holds **52 npm names** while the family has 42 plugin repos (measured 2026-10-04).

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

<!-- Instrument, kept out of the rendered text: ★ from `gh api repos/<repo> --jq .stargazers_count`,
     and a repo counts only when its default branch carries at least one commit of ours.
     Re-derived 2026-10-05 over every external repository this account ever opened a pull request
     against (106 of them). The probe is now the one the rule itself names --
     `defaultBranchRef.target.history` with `author:{id:<node id>}` -- because the two cheaper
     probes both fail in the direction that matters, and both were tried first. `/contributors` is a
     computed list capped at 100 entries, and it returns no entry for `yibie/awesome-jev` while that
     branch carries one of our commits: the 09-25 round read that false negative into the text as an
     uncredited merge and printed a row its own rule excluded, so the 43 attributed repositories here
     are 36 + the six repositories newly credited + that one correction -- a probe fix, not a merge
     surge. `/commits?author=<login>` returned an empty array for `pan17/dsh-wechat`, whose default
     branch holds three commits authored by this account, so a login probe silently under-counts and
     is not used again. A merged pull request is still not by itself proof:
     `SihanTeng/awesome-deepseek-harness-plugins` has taken 32 of ours and credits no commit, so it
     stays in prose and not in the table, and `MoonshotAI/checkpoint-engine` (1,006★, a merged PR, no
     commit of ours) is absent for the same reason. Merged work only; open proposals are deliberately
     not listed here. The merged count comes from the account's own pull requests, not from a probe,
     so it is exact. Attribution re-verified through the owners' own profiles and governance pages,
     which is why the column is here at all: a repository path alone does not tell a reader whether
     Tencent or a weekend maintainer owns the project. -->

*Every repo below is external to `PerryLink/*`; every number is measured, merged work only, and open proposals are deliberately not listed. The third column names the project's owner — the account alone does not say whether that is a company, a standards body or one person.*

**★ 1,000+ — named individually, as the rule requires, each carrying the party that owns the project.** Twenty external repos above a thousand stars carry merged work (★ measured 2026-10-05), three more than the round before — and none of the three is a row that merely drifted over the line: `ruvnet/ruflo` and `walkinglabs/learn-harness-engineering` entered with merges landed in the ten days since, and `punkpeye/fastmcp` has carried its merge since 2026-09-24 and was missing from the earlier seventeen. Six of those rows belong to a company or a well-known project organization — Reactive Resume, DeepSeek, cordiverse, Tencent, and the ACP project that Zed and JetBrains jointly govern, which accounts for two of the twenty; the other fourteen are catalog repos, small community orgs and one-person projects, and the column says so rather than letting the account name imply a company:

| Repository | ★ | 项目归属方 |
|---|---|---|
| [ruflo](https://github.com/ruvnet/ruflo) | 73,842 | ruvnet (rUv / Reuven Cohen) — individual maintainer; a 73.8k★ agent harness on a personal account, not a company repo, and the largest row in this table |
| [reactive-resume](https://github.com/reactive-resume/reactive-resume) | 43,755 | `reactive-resume` org — independent open-source project (rxresu.me) |
| [laya](https://github.com/NandhaKishorM/laya) | 30,650 | NandhaKishorM — individual maintainer; the repo was created 2026-09-18 |
| [learn-harness-engineering](https://github.com/walkinglabs/learn-harness-engineering) | 18,986 | `walkinglabs` community org — the harness-engineering tutorial site |
| [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) | 17,758 | `awesome-dsh-plugin` org — community catalog, no company behind it |
| [FlashMLA](https://github.com/deepseek-ai/FlashMLA) | 13,034 | **DeepSeek** — the official `deepseek-ai` org |
| [Cordis](https://github.com/cordiverse/cordis) | 8,999 | **cordiverse** org; its maintainer Shigma is now at **DeepSeek**, and Cordis is the kernel DeepSeek Harness vendors as `@deepseek-ai/cordis` |
| [dsh-web](https://github.com/zhu1090093659/dsh-web) | 8,364 | zhu1090093659 — individual maintainer |
| [ouroboros](https://github.com/Q00/ouroboros) | 6,179 | Q00 — individual maintainer (`@zep-us`) |
| [dsh-market](https://github.com/dsh-market/dsh-market) | 5,508 | `dsh-market` org — the community plugin market behind dshmarket.com, not a DeepSeek repo |
| [teamai-cli](https://github.com/Tencent/teamai-cli) | 5,121 | **腾讯 Tencent** — the official `Tencent` org, opensource.tencent.com |
| [agent-client-protocol](https://github.com/agentclientprotocol/agent-client-protocol) | 4,371 | `agentclientprotocol` org — governed jointly by **Zed Industries** and **JetBrains** |
| [fastmcp](https://github.com/punkpeye/fastmcp) | 3,272 | punkpeye (Frank Fiegel) — individual maintainer at Glama; the TypeScript MCP framework |
| [deepseek-harness-desktop](https://github.com/dsh-tauri/deepseek-harness-desktop) | 3,012 | `dsh-tauri` community org — self-described non-official and non-commercial, not a DeepSeek repo |
| [claude-agent-acp](https://github.com/agentclientprotocol/claude-agent-acp) | 2,610 | `agentclientprotocol` org — the same jointly-governed org as the row above, a separate repository |
| [awesome-jev](https://github.com/yibie/awesome-jev) | 2,124 | yibie — individual maintainer, community catalog for Jev; the row the 09-25 round both printed and denied, kept now on the commit the history probe finds |
| [dsh-plugin-radar](https://github.com/AdamPlatin123/dsh-plugin-radar) | 1,464 | AdamPlatin123 — individual maintainer, catalog is a generated artifact |
| [Agents-Anywhere](https://github.com/anywhere-labs/Agents-Anywhere) | 1,413 | `anywhere-labs` community org — 3 public repos, created 2026-05, dshdesktop.cn; not a company |
| [awesome-deepseek-harness](https://github.com/0xsline/awesome-deepseek-harness) | 1,137 | 0xsline — individual maintainer, community catalog |
| [awesome-vibecoded-saas](https://github.com/Anil-matcha/awesome-vibecoded-saas) | 1,037 | Anil Chandra Naidu Matcha — individual maintainer, community catalog |

*Cordis is the upstream plugin-core framework that powers DeepSeek Harness — vendored into that repo and renamed `@deepseek-ai/cordis`; FlashMLA #224 is the only merged pull request in the whole `deepseek-ai` org.*

**The rest of the contributor set** is the community catalog layer rather than upstream projects: **23 further repositories**, DSH plugin directories and small community projects ([dsh-handbook](https://github.com/Electricitysheep/dsh-handbook) and [imsai-sh's list](https://github.com/imsai-sh/awesome-deepseek-harness-plugins), which alone took 41 merges, among them) — the catalogs ingest the family and carry no company owner, so they are named here only in aggregate. **43 external repositories carry at least one merged pull request of ours together with a commit attributed to this account, and 316 merges were counted inside them** — re-derived 2026-10-05 from this account's own merged pull requests, so 316 is exact rather than a floor over a probed subset. One further repository took **32 more** of our merged pull requests **without** crediting a commit to this account on its default branch — [SihanTeng's list](https://github.com/SihanTeng/awesome-deepseek-harness-plugins), which is the case the rule at the top of this section was written about — so it does not size the contributor set. 316 + 32 = the **348 merged pull requests** this account has outside `PerryLink/*`, concentrated in **44 repositories**; a further **97 are open across 58 repositories** and are deliberately not counted here, 35 of them inside the 44 that have already merged something.

**The ten days since the last round moved the merged count by 27** (2026-09-25 → 2026-10-05, the window this round re-measured), and 21 of those 27 are `laya` alone. The other six landed one apiece in six repositories that were not part of this set at all before — [ruflo](https://github.com/ruvnet/ruflo), [learn-harness-engineering](https://github.com/walkinglabs/learn-harness-engineering), [koishi-plugin-booru](https://github.com/koishijs/koishi-plugin-booru), [dsh-plugin-manager](https://github.com/2768651338/dsh-plugin-manager), [dsh-plugin-market](https://github.com/losebird/dsh-plugin-market) and [dsh-annotation](https://github.com/omdsh-dev/dsh-annotation) — which is what puts the largest row in the table, `ruflo` at 73,842★, in a set it was not part of ten days ago. Ten fresh proposals went out in the same window and have not merged yet.

**laya** — [NandhaKishorM/laya](https://github.com/NandhaKishorM/laya) — **45 merged pull requests of the 49 this account has opened there**, and **second among merged-PR authors** there: behind `aashish254` (126) and ahead of `Bruce-Yii` (27), with the maintainer NandhaKishorM holding one merged PR of his own because he commits to `main` directly rather than through pull requests — none of the three leaders is a collaborator, so all three are outside contributors. All 45 merged inside a nine-day run (2026-09-21 → 2026-09-29), and the maintainer merges in batches rather than one at a time, which is why fifteen of the 45 share two timestamps: seven at `19:29:05` on 09-27 with [#556](https://github.com/NandhaKishorM/laya/pull/556) a second before them, and eight at `17:40:36` on 09-29. Nine areas rather than one:

- **Multilingual routing and evaluation** — a caller-supplied language hint ([#211](https://github.com/NandhaKishorM/laya/pull/211)), a reproducible per-language harness ([#210](https://github.com/NandhaKishorM/laya/pull/210)), a re-run of the 51-language sweep in both temperature regimes ([#222](https://github.com/NandhaKishorM/laya/pull/222)), the multilingual columns refreshed from that re-run ([#389](https://github.com/NandhaKishorM/laya/pull/389)), letters counted for the scripts no range claims ([#169](https://github.com/NandhaKishorM/laya/pull/169)), and a `Router` that no longer picks a checkpoint from a language code naming no language ([#368](https://github.com/NandhaKishorM/laya/pull/368)).
- **HTTP serving and containers** — inference moved off the event loop ([#230](https://github.com/NandhaKishorM/laya/pull/230)), the Compose `laya-serve` service ([#234](https://github.com/NandhaKishorM/laya/pull/234)), the inference failure the client is not allowed to see now reaching the operator's log ([#375](https://github.com/NandhaKishorM/laya/pull/375)), a request with no state no longer answered about the literal text `null` ([#427](https://github.com/NandhaKishorM/laya/pull/427)), and a lone surrogate in the body returning 400 instead of 500 ([#454](https://github.com/NandhaKishorM/laya/pull/454)).
- **Email disclaimers and names** — the request kept when a disclaimer footer shares its paragraph ([#94](https://github.com/NandhaKishorM/laya/pull/94)), "confidential" no longer read as a disclaimer ([#227](https://github.com/NandhaKishorM/laya/pull/227)), a `From:` line opening ordinary prose no longer deleting the request ([#371](https://github.com/NandhaKishorM/laya/pull/371)), and a name class that excluded lowercase in every script ([#503](https://github.com/NandhaKishorM/laya/pull/503)).
- **Correctness across the call surface** — three assertions that could not fail ([#231](https://github.com/NandhaKishorM/laya/pull/231)), the load-time and budget errors no suite reached ([#237](https://github.com/NandhaKishorM/laya/pull/237)), an ECE that binned differently from its siblings ([#232](https://github.com/NandhaKishorM/laya/pull/232)), non-ASCII characters kept in non-string instructions ([#228](https://github.com/NandhaKishorM/laya/pull/228)), a README link pointing at a heading that does not exist ([#236](https://github.com/NandhaKishorM/laya/pull/236)), a choice label with no description that came back as a non-string ([#380](https://github.com/NandhaKishorM/laya/pull/380)), a nested choice label reported as a named caller error instead of a bare `TypeError` ([#425](https://github.com/NandhaKishorM/laya/pull/425)), a score legend that echoed the caller's own type instead of level text ([#420](https://github.com/NandhaKishorM/laya/pull/420)), `hooks_installed` removing a hook it did not install ([#424](https://github.com/NandhaKishorM/laya/pull/424)), a null `choice` label that made the answer undecodable ([#508](https://github.com/NandhaKishorM/laya/pull/508)), a short temperature list that now fails at load rather than at the first decode ([#502](https://github.com/NandhaKishorM/laya/pull/502)), [#249](https://github.com/NandhaKishorM/laya/pull/249), where a `noul` criteria dict that cannot be read raises instead of silently falling back to defaults — the line the project's 0.3.11 release note calls "stricter noul criteria" — and [#299](https://github.com/NandhaKishorM/laya/pull/299), two parity cells in the benchmark table that did not match the JSON they cite.
- **The test and CI surface** — the Windows lane ([#212](https://github.com/NandhaKishorM/laya/pull/212)) and [#376](https://github.com/NandhaKishorM/laya/pull/376), six pytest suites that every lane invoked in a way that exited 0 without running a single test, including the only coverage of the HTTP surface.
- **Prediction hooks and batched routing** — process-wide default hooks never reaching `predict_batch` ([#379](https://github.com/NandhaKishorM/laya/pull/379)), `predict_batch` dropping each request's `lang`, so per-language temperatures never applied ([#381](https://github.com/NandhaKishorM/laya/pull/381)), and `lang_temperatures` crashing on the inputs it exists to reject ([#428](https://github.com/NandhaKishorM/laya/pull/428)).
- **The TypeScript front end** — the `From:` header rules the Python side already had, ported rather than re-derived ([#422](https://github.com/NandhaKishorM/laya/pull/422)); the Azerbaijani schwa counted as a non-English letter ([#423](https://github.com/NandhaKishorM/laya/pull/423)); and a score legend that echoed the caller's own types, unlike the Python backends ([#556](https://github.com/NandhaKishorM/laya/pull/556)).
- **CLI, packaging and serving edges** — `--preset` sending the request under a key no question set names ([#426](https://github.com/NandhaKishorM/laya/pull/426)); the onnx extra missing its `onnxscript` dependency ([#504](https://github.com/NandhaKishorM/laya/pull/504)); the packaging test scanning `.venv` for broken links ([#500](https://github.com/NandhaKishorM/laya/pull/500)); and two over-budget messages that each named a knob which makes the problem worse rather than the one that fixes it ([#455](https://github.com/NandhaKishorM/laya/pull/455), [#501](https://github.com/NandhaKishorM/laya/pull/501)).
- **Documentation** — [#378](https://github.com/NandhaKishorM/laya/pull/378), which stopped the README presenting a confidence threshold as permission to act on its own, and the pages the project's docs-structure issue asked contributors to write: the fine-tuning guide ([#505](https://github.com/NandhaKishorM/laya/pull/505)), the Questions and answers guide ([#418](https://github.com/NandhaKishorM/laya/pull/418)), and the reference entry for `answer_confidence`, which no page documented ([#419](https://github.com/NandhaKishorM/laya/pull/419)).

*The nine area headings above are this account's own grouping of its 45 merges, not the project's taxonomy; the merge counts are the repository's own.*

**Two are open there and deliberately not counted above** — [#924](https://github.com/NandhaKishorM/laya/pull/924), a load that crashes because transformers tries to import TensorFlow, and [#925](https://github.com/NandhaKishorM/laya/pull/925), a stale `low_confidence` left behind on a re-gate; both went up 2026-10-04, after the fourteen this page had listed as pending were all resolved — thirteen merged between 09-25 and 09-29, and [#416](https://github.com/NandhaKishorM/laya/pull/416) closed instead, with the guide it carried landing as [#418](https://github.com/NandhaKishorM/laya/pull/418). That leaves two closures unmerged in total, and the reason is on the record for each: [#370](https://github.com/NandhaKishorM/laya/pull/370), closed by this account as a duplicate of [#362](https://github.com/NandhaKishorM/laya/pull/362), which opened the same fix four minutes earlier, and [#416](https://github.com/NandhaKishorM/laya/pull/416), the Routing guide, closed by the maintainer in favour of another contributor's [#461](https://github.com/NandhaKishorM/laya/pull/461) so the project would not carry two routing pages.

**Security** — published advisory [GHSA-j922-p6h6-p255](https://github.com/PerryLink/dsh-permission-rules/security/advisories/GHSA-j922-p6h6-p255) for dsh-permission-rules (medium, patched in 0.6.16).

**Official harness repo** — it does not accept external pull requests, so that line runs through issues, Discussions (the Show Your Plugins! post [#6104](https://github.com/deepseek-ai/deepseek-harness/discussions/6104)) and the plugin ecosystem instead — while the wider `deepseek-ai` org is open to fixes, and the account now proposes them at the systems layer rather than only in its catalogs: of the **20 pull requests it has opened across that org, FlashMLA [#224](https://github.com/deepseek-ai/FlashMLA/pull/224) remains the only one merged**, and **16 are open**, 14 of them code fixes carrying a reproduction across ten repositories — [DeepEP](https://github.com/deepseek-ai/DeepEP) three, [FlashMLA](https://github.com/deepseek-ai/FlashMLA) and [deepseek-recipe](https://github.com/deepseek-ai/deepseek-recipe) two each, and one apiece in [DeepGEMM](https://github.com/deepseek-ai/DeepGEMM), [3FS](https://github.com/deepseek-ai/3FS), [TileKernels](https://github.com/deepseek-ai/TileKernels), [DeepSeek-MoE](https://github.com/deepseek-ai/DeepSeek-MoE), [DeepSeek-Prover-V1.5](https://github.com/deepseek-ai/DeepSeek-Prover-V1.5), [DeepJIT](https://github.com/deepseek-ai/DeepJIT) and [DeepSelect](https://github.com/deepseek-ai/DeepSelect) — the other two are catalog additions.

## 🌍 Where the plugins live

- **GitHub** (this profile), **[Gitee](https://gitee.com/perrylink)** and **npm** — source, CI and releases here; 46 family repos mirrored to Gitee by a daily job (default branch + all tags), plus this profile repo; the `perrylink` account holds **52 npm names and 909 versions**, 46 of them with a non-deprecated `latest` and 44 carrying a provenance attestation on that version (measured 2026-10-04 against each name's own packument — the registry **search** endpoint is not authoritative here, since it returns only 47 names and omits the deprecated ones)
- **npm downloads** — **158,593 over the trailing 30 days** (npm window 09-04..10-03, summed per name from the downloads point endpoint; **[dshfind](https://dshfind.com/plugins?q=PerryLink)** independently tracks **21.5k+** across the 7 family plugins it currently has a download figure for — dshfind reports rounded tiers, so that is a floor rather than a total
- **DSH Desktop Market** — add the catalog source `https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json` under Market → Sources to browse the family in-app; **MCP Registry** — three servers, all published from their release workflows over GitHub OIDC: `dsh-cert-mcp`, `jevcore-mcp` and `laya-mcp`
- **GitHub Actions** — [dsh-github](https://github.com/PerryLink/dsh-github) and [dsh-test-drive](https://github.com/PerryLink/dsh-test-drive) also ship composite actions, so they install as `uses: PerryLink/dsh-test-drive@vX`

Published to a dozen-plus third-party DSH directories and curated lists — [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin), [DSH Directory](https://dsh.directory/plugins?q=perrylink), [Awesome DeepSeek Harness](https://github.com/0xsline/awesome-deepseek-harness), [walkinglabs' list](https://github.com/walkinglabs/awesome-deepseek-harness-plugins), [Zhiyuan-Fan's list](https://github.com/Zhiyuan-Fan/Awesome-DeepSeek-Harness-Plugins), the [AdamPlatin123 radar](https://github.com/AdamPlatin123/dsh-plugin-radar), [dsh-suite](https://github.com/whyihaveyou/dsh-suite), [dshfind.com](https://dshfind.com/zh/plugins/PerryLink/dsh-memento), [deepseek1024.com](https://deepseek1024.com) and [Glama](https://glama.ai/mcp/servers/PerryLink/dsh-cert-mcp) among them — and scored on [OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/PerryLink/dsh-auto-review); the GitHub [`dsh-plugin` topic](https://github.com/topics/dsh-plugin) is what most of them ingest from.

## 中文介绍

**在 DeepSeek Harness 上构建插件生态:42 个开源插件,来自一个 48 仓的家族(其中 47 个由 PerryLink 自己维护)—— 安全、工作流、研究、消息桥接、开发者体验,外加 DSH Desktop Market 目录、插件认证注册表与 dsh-plugin-doctor 这个 CI 检查器。42 个插件全部带 CI 与 Gitee 镜像,五语文档由每个仓自己的 CI 闸门守着一致(段落数、安装命令、配置键),并声明 `dsh.bundle` 契约;近 30 天 npm 下载 **158,593**(窗口 09-04..10-03)。`perrylink` 这个 npm 账号下共有 **52 个名称、909 个版本**:其中 **46 个** latest 版本未弃用(**40 个**非 scoped + **6 个** `@perrylink/` scoped)、**6 个已弃用**(`dsh-plugin-upgrade` 折进 2.0.0 后退役的一条走廊腿、作者撤回的 `dsh-personal-directive`、改名前的 scoped `@perrylink/dsh-cert-mcp`,以及三个已归档的 `layacore` 名字)、**44 个**当前 latest 版本带 provenance 证明(均按 2026-10-04 实测,逐个读各自 packument —— 注意 npm 的 search 接口在这里不作数,它只返回 47 个名称并漏掉已弃用的那几个)。我也向上游 [Cordis](https://github.com/cordiverse/cordis)(DeepSeek Harness 所基于的插件内核框架)与 [deepseek-ai](https://github.com/deepseek-ai) 项目贡献:该组织下 20 条 PR 里,已合并的仍是 [FlashMLA](https://github.com/deepseek-ai/FlashMLA) 修复(#224,唯一一条),另有 **16 条开放**,其中 14 条是带复现的系统层修复(DeepEP 3 条、FlashMLA 与 deepseek-recipe 各 2 条,以及 DeepGEMM、3FS、TileKernels、DeepSeek-MoE、DeepSeek-Prover-V1.5、DeepJIT、DeepSelect 各 1 条);家族之外**共 43 个外部仓**带着本账号已合并的 PR 与一条归属提交,**其中 20 个在千星以上**,已合并 PR 合计 **348 条**(均按 2026-10-05 实测)。**

**这一家子所依赖的那项研究,现在是一篇有 DOI 的论文 —— 而且它测的很大一部分,正是这份主页上的两个项目:[laya-mcp](https://github.com/PerryLink/laya-mcp) 与 [jevcore](https://github.com/PerryLink/jevcore)。**《[当判定层的自报字段说谎时:三类判断层的成本、延迟与失效边界实测](https://doi.org/10.5281/zenodo.22902025)》在一套相同条目上实测三类判定层(Laya、TypeSafe Jev、DeepSeek-V4.1-Flash),四条主张**三条成立、一条被自己的数据否定**;判定器的接入层自报字段不可信(截断标志报「通过」却静默丢输入、概率字段把结论反号、两个判定词在真实输入下不可达),失效集中在一处 —— 答案被明确陈述时近乎完美(0.9909,n=220),必须注意到「缺席」时塌缩(0.3091,n=220);异种判定器在三个区制上都**没有**增量覆盖。**引其一即可,不要当两篇引**([英文原文](https://doi.org/10.5281/zenodo.22901853) · [中文译本](https://doi.org/10.5281/zenodo.22902025) · [制品](https://doi.org/10.5281/zenodo.22901248));两者有出入以英文为准。

**2026-10-04 轮:这一轮是重新测量,不是发布 —— 三处旧数字被自己的探针推翻。**其一,主页写「36 个外部仓带我的提交」,同一套规则重跑(106 个外部仓逐个查 `/contributors`)返回 **43 个**,千星以上从 17 涨到 **20 个**,家族之外的已合并 PR 从 321 涨到 **348**;更要紧的是纠错:主页把 **14 条 laya 的 PR 列为「仍开放」**,而读仓库自己的 pull request 连接是「开过 47 条、合并 45 条、自行关闭 2 条、**当前开放 0 条**」—— 那 14 条在 09-27 与 09-29 两批各 8 条合掉了。其二,npm 数字逐名重测后是 **52 个名称、909 个版本、46 个 latest 未弃用、44 个带 provenance**,而不是旧版写的 56 / 917 / 49 / 42。其三,窗口里唯一每天都有动作的是 [dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor):09-25 到 10-04 共 10 次提交,每次都是 `chore: refresh verified badges` 重写 `data/verified.json`(+122/-122)。

**2026-09-25 轮:全家搬到 `0.1.7-rc.2` 宿主线(41 个仓一次过、482 个 `@deepseek-ai/dsh-*` pin 移出 `0.1.7-rc.1`、36 个包在新 patch 上发布),并顺带发现一个被整整落后一条宿主线的仓。**

**laya**([NandhaKishorM/laya](https://github.com/NandhaKishorM/laya))是这个账号投入最深的外部项目:提了 **49 条 PR,其中 45 条已合并**,合并数在该仓**排第二** —— 前面是 `aashish254` 的 126 条,后面是 `Bruce-Yii` 的 27 条;维护者 NandhaKishorM 自己只有 1 条已合并 PR,因为他直接向 `main` 提交而不走 PR。这三位领头的都不是该仓的 collaborator,所以都算外部贡献者。45 条全部合在 2026-09-21 至 09-29 这九天里,而维护者是**成批合并**而不是逐条合,所以有 15 条共享两个时间戳:09-27 的 `19:29:05` 一次合了 7 条([#556](https://github.com/NandhaKishorM/laya/pull/556) 早一秒),09-29 的 `17:40:36` 一次合了 8 条。方向不是一个,而是九个:[#211](https://github.com/NandhaKishorM/laya/pull/211)、[#210](https://github.com/NandhaKishorM/laya/pull/210)、[#222](https://github.com/NandhaKishorM/laya/pull/222)、[#389](https://github.com/NandhaKishorM/laya/pull/389)、[#169](https://github.com/NandhaKishorM/laya/pull/169)、[#368](https://github.com/NandhaKishorM/laya/pull/368)(多语言路由与评测);[#230](https://github.com/NandhaKishorM/laya/pull/230)、[#234](https://github.com/NandhaKishorM/laya/pull/234)、[#375](https://github.com/NandhaKishorM/laya/pull/375)、[#427](https://github.com/NandhaKishorM/laya/pull/427)、[#454](https://github.com/NandhaKishorM/laya/pull/454)(HTTP 服务与容器);[#94](https://github.com/NandhaKishorM/laya/pull/94)、[#227](https://github.com/NandhaKishorM/laya/pull/227)、[#371](https://github.com/NandhaKishorM/laya/pull/371)、[#503](https://github.com/NandhaKishorM/laya/pull/503)(邮件免责声明与姓名类);[#231](https://github.com/NandhaKishorM/laya/pull/231)、[#237](https://github.com/NandhaKishorM/laya/pull/237)、[#232](https://github.com/NandhaKishorM/laya/pull/232)、[#228](https://github.com/NandhaKishorM/laya/pull/228)、[#236](https://github.com/NandhaKishorM/laya/pull/236)、[#380](https://github.com/NandhaKishorM/laya/pull/380)、[#425](https://github.com/NandhaKishorM/laya/pull/425)、[#420](https://github.com/NandhaKishorM/laya/pull/420)、[#424](https://github.com/NandhaKishorM/laya/pull/424)、[#508](https://github.com/NandhaKishorM/laya/pull/508)、[#502](https://github.com/NandhaKishorM/laya/pull/502)、[#249](https://github.com/NandhaKishorM/laya/pull/249)、[#299](https://github.com/NandhaKishorM/laya/pull/299)(调用面正确性);[#212](https://github.com/NandhaKishorM/laya/pull/212)、[#376](https://github.com/NandhaKishorM/laya/pull/376)(测试与 CI 面);[#379](https://github.com/NandhaKishorM/laya/pull/379)、[#381](https://github.com/NandhaKishorM/laya/pull/381)、[#428](https://github.com/NandhaKishorM/laya/pull/428)(prediction hooks 与批量路由);[#422](https://github.com/NandhaKishorM/laya/pull/422)、[#423](https://github.com/NandhaKishorM/laya/pull/423)、[#556](https://github.com/NandhaKishorM/laya/pull/556)(TypeScript 前端);[#426](https://github.com/NandhaKishorM/laya/pull/426)、[#504](https://github.com/NandhaKishorM/laya/pull/504)、[#500](https://github.com/NandhaKishorM/laya/pull/500)、[#455](https://github.com/NandhaKishorM/laya/pull/455)、[#501](https://github.com/NandhaKishorM/laya/pull/501)(CLI、打包与服务边界);[#378](https://github.com/NandhaKishorM/laya/pull/378)、[#505](https://github.com/NandhaKishorM/laya/pull/505)、[#418](https://github.com/NandhaKishorM/laya/pull/418)、[#419](https://github.com/NandhaKishorM/laya/pull/419)(文档)—— 包括项目的**第一条 Windows CI 车道**([#212](https://github.com/NandhaKishorM/laya/pull/212)),Linux 的 16 个 suite 里 15 个现在在 `windows-latest` 上跑。另有 **[#924](https://github.com/NandhaKishorM/laya/pull/924)、[#925](https://github.com/NandhaKishorM/laya/pull/925) 两条仍开放**(2026-10-04 提的,一条是 transformers 试图导入 TensorFlow 导致加载崩溃,一条是重新过闸时残留的 `low_confidence`),按上面的口径不计入;此前主页列为「仍开放」的那 14 条已全部了结:13 条在 09-25 至 09-29 之间合并,[#416](https://github.com/NandhaKishorM/laya/pull/416) 那条 Routing 指南则由维护者关闭、改用另一位贡献者的 [#461](https://github.com/NandhaKishorM/laya/pull/461),它承载的内容以 [#418](https://github.com/NandhaKishorM/laya/pull/418) 落地。因此未合并即关闭的一共 2 条,原因各自有记录:[#370](https://github.com/NandhaKishorM/laya/pull/370) 由我自己作为重复关闭(比它早四分钟的 [#362](https://github.com/NandhaKishorM/laya/pull/362) 是同一个修复),以及上面那条 [#416](https://github.com/NandhaKishorM/laya/pull/416)。

**还有一条在别处:一个根本起不来的进程现在能起来了。** [claude-agent-acp #1146](https://github.com/agentclientprotocol/claude-agent-acp/pull/1146) 让 `src/index.ts` 里那处没有保护的顶层 await 不再因一次瞬时错误就中断模块求值、在发出任何一条 ACP 消息之前退出。

待业中。十一准备出去玩一圈，所以更新迭代节奏可能短期内仍然提升的有限。当然，问题和缺陷修复不会停，只是发布频率会降低一些，还请大家谅解。
