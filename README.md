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
  2026-09-23 from each badge's own SVG width/height at the 20px render height: 17 badges totalling
  2408px, split 801 / 811 / 796 (range 15) by a search over the row breaks, every row inside
  GitHub's ~888px README content column. Per badge, in that order: stars 90, followers 106, repos
  86, openssf scorecard 126, glama 110, npm packages 113, npm downloads 170, MCP Registry 144,
  awesome 168, DSH Directory 218, DSH Market 180, Gitee 101, dshfind 174, dshfind downloads 246,
  Desktop Market 172, certified 132, plugins 72. The repos badge is a dynamic/json badge and was
  serving its "invalid" state (86px) at measure time; as "repos: 209" it renders 72px, which makes
  the same partition 787 / 811 / 796 -- both states fit the column and neither row order changes.
  If you add or remove a badge the total changes and this partition is lost: re-solve it rather
  than appending to a row, and re-measure the widths -- do not reuse these numbers after a label
  change, since a single label edit shifts a row.

  The dshfind entries: the plain dshfind badge is dshfind's own per-repo badge and links a specific
  plugin, so it can only show that repo's figure. dshfind publishes no owner-level badge and its API
  has no downloads field at all (listing, detail and GraphQL alike -- the figure exists only inside
  the rendered SVG, rounded to tiers such as "5k+"). The aggregate badge is therefore hand-written
  from the sum of every PerryLink badge's own rendered tier. Tiers are lower bounds, so "22k+" is a
  floor, and only the plugins dshfind has a figure for are counted (8 of the 49 it indexes): that is
  what "across 8 plugins" states. Re-sum it when dshfind reports more.

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
<img alt="npm downloads 30d" src="https://img.shields.io/badge/npm%20downloads%2030d-137.4k-6e7781">
<br>
<a href="https://registry.modelcontextprotocol.io/v0/servers?search=perrylink"><img alt="MCP Registry" src="https://img.shields.io/badge/MCP%20Registry-3%20servers-6f42c1"></a>
<a href="https://awesome-dsh-plugin.com"><img alt="awesome-dsh-plugin" src="https://awesome-dsh-plugin.com/badge.svg"></a>
<a href="https://dsh.directory/plugins?q=perrylink"><img alt="Listed on DSH Directory" src="https://dsh.directory/badges/listed.svg"></a>
<a href="https://dsh.market/?q=PerryLink"><img alt="DSH Market" src="https://raw.githubusercontent.com/2BingLing/dsh-market/master/assets/readme/badge-listed-en.svg"></a>
<a href="https://gitee.com/perrylink"><img alt="Gitee mirror" src="https://img.shields.io/badge/Gitee-mirror-c71d23?logo=gitee"></a>
<br>
<a href="https://dshfind.com/plugins/PerryLink/dsh-auto-review?ref=badge"><img alt="dshfind" src="https://dshfind.com/api/badge/PerryLink/dsh-auto-review?metric=downloads"></a>
<a href="https://dshfind.com/plugins?q=PerryLink"><img alt="dshfind downloads across the family" src="https://img.shields.io/badge/dshfind%20downloads-22k%2B%20across%208%20plugins-6e7781"></a>
<a href="https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json"><img alt="DSH Desktop Market source" src="https://img.shields.io/badge/DSH%20Desktop%20Market-source-0969da"></a>
<a href="https://github.com/PerryLink/dsh-plugin-certification"><img alt="Certified dsh-auto-review" src="https://raw.githubusercontent.com/PerryLink/dsh-plugin-certification/main/badges/PerryLink__dsh-auto-review.svg"></a>
<img alt="plugins" src="https://img.shields.io/badge/plugins-42-6e7781">
</p>

**Building the [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness) plugin ecosystem: 42 open-source plugins in a 46-repo family (45 PerryLink-owned plus [pan17](https://github.com/pan17/dsh-wechat)'s dsh-wechat, Apache-2.0) — security, workflows, research, messaging bridges, developer experience — plus the DSH Desktop Market catalog, a plugin-certification registry and the dsh-plugin-doctor CI checker. All 42 ship CI and a Gitee mirror, five-language docs held to the same section count, install command and configuration keys by a gate in each repo's own CI, and the `dsh.bundle` contract; 137,423 npm downloads over the trailing 30 days. I also contribute upstream to [Cordis](https://github.com/cordiverse/cordis) — the plugin-core framework DeepSeek Harness is built on — and to [deepseek-ai](https://github.com/deepseek-ai) projects, including a merged [FlashMLA](https://github.com/deepseek-ai/FlashMLA) fix.**

DeepSeek Harness turned "everything is a plugin" into an ecosystem. I build the plugins I wish existed — engineering-discipline guardrails, runtime panels, cross-session memory, and verifiable research engines — and publish them the way production software deserves.

---

<!-- Round rotation: keep only the newest two rounds (current + one previous). Older rounds live in git history and can be restored on request. Rounds are narrative only — no Snapshot/counter lines: live counts belong to the badge row and "Where the plugins live", and per-edition copies go stale. GHSA/long-lived references belong in "Upstream & community contributions".

     DEVIATION, 2026-09-23: the English "Latest" now carries THREE rounds (09-23, 09-22, 09-21)
     rather than two. Reason: the 09-23 paper entry names laya-mcp and jevcore as the things it
     measures, and the 09-21 round is the one that introduces laya-mcp. Rotating it out here
     would leave a forward reference to a project the page no longer introduces anywhere. The
     extra round goes when the 09-23 entry no longer depends on it, not on a schedule. The
     Chinese block below already ran four rounds before this edit and is left as it was. -->

## 📣 Latest — 2026-09-23

- **The research this family rests on is now a published paper with a DOI — and it is, in large part, a measurement of two things on this profile: [laya-mcp](https://github.com/PerryLink/laya-mcp) and [jevcore](https://github.com/PerryLink/jevcore).** [*When a Judgment Layer's Self-Reported Fields Lie: Cost, Latency and the Failure Boundary of Three Judgment Layers on the Same Items*](https://doi.org/10.5281/zenodo.22901853) — three judgment layers measured on one item set: Laya (local, non-autoregressive), TypeSafe Jev (remote, typed decisions) and DeepSeek-V4.1-Flash. Four claims; **three hold and one the data refutes.** A [complete Chinese translation](https://doi.org/10.5281/zenodo.22902025) is archived separately, and the [artifact](https://doi.org/10.5281/zenodo.22901248) — code and every `results/` JSON — is a third record.

- **What it found, in one line each.** Cost is not the binding constraint: the real axes are latency and the usable state window, and "an order of magnitude cheaper" stops holding once state grows. **The judges' self-reported access-layer fields are not trustworthy**, and their failures cluster in one place — the concrete ones being a truncation flag that reports `passed` while silently dropping input, a probability field that inverts an item's conclusion, and two verdict words that are unreachable under real input. The shape behind them: the judge is near-perfect (0.9909, n=220) where the answer is explicitly stated and collapses (0.3091, n=220) where it must notice an **absence** — while its self-reported confidence stays high in both cases.

- **The negative result is reported as one.** A dissimilar judge does **not** supply incremental coverage in any of the three regimes: when the generator errs the judge is *less* accurate than its own marginal, and the failure correlation is positive in 3/3 draws. The paper also reports four instances of the error class it names — **a specification-level defect masquerading as a finding about the model** — each caught by a control and not by review, which is where its 23 mandatory protocol clauses come from.

- **Both language versions say they are one work, in their own pages.** Zenodo has no `is translation of` relation, so the fact is carried in each PDF's front matter and in the record descriptions instead. [10.5281/zenodo.22901853](https://doi.org/10.5281/zenodo.22901853) · [10.5281/zenodo.22902025](https://doi.org/10.5281/zenodo.22902025) — cite one, not both; where they differ, the English text governs.

### 2026-09-22 round

- **Five upstream pull requests merged — three of them in repositories this account had never contributed to before.** [reactive-resume](https://github.com/reactive-resume/reactive-resume) [#3527](https://github.com/reactive-resume/reactive-resume/pull/3527) (out-of-range months rendered an employment period as `undefined 2019 - Present`), [laya](https://github.com/NandhaKishorM/laya) [#94](https://github.com/NandhaKishorM/laya/pull/94) (a disclaimer footer sharing a paragraph made `clean_email_body` delete the whole body, with a regression suite wired into CI in the same change), [teamai-cli](https://github.com/Tencent/teamai-cli) [#695](https://github.com/Tencent/teamai-cli/pull/695) (Qoder CN keeps its user directory at `~/.qoder-cn`, so a CN install synced nothing; merged after four rounds of the repo's own automated review, each of which found a real defect in the previous attempt), and [walkinglabs' plugin list](https://github.com/walkinglabs/awesome-deepseek-harness-plugins) [#76](https://github.com/walkinglabs/awesome-deepseek-harness-plugins/pull/76) and [#65](https://github.com/walkinglabs/awesome-deepseek-harness-plugins/pull/65) (36 family plugins added to its curated README). Two further proposals were closed by me rather than left to compete, and are not counted as merged.
- **Upstream shipped 0.1.7-alpha.1** — it removes `resolutionMode` outright, so a source/`pnpm` launch no longer has two resolvers to disagree about. Worth recording because two of the three threads reporting *"Cannot read properties of undefined (reading 'prepare')"* were source launches, and the underlying defect was two module instances of `@deepseek-ai/dsh-tools` each holding its own private `TOOL_RUNTIME_SCHEDULER` symbol. Eighteen unanswered Discussions threads were answered, carrying that root cause with file-and-line references.
- **The family's five-language documentation was reconciled with itself, and the last gap in its CI coverage closed.** The family table is hand-maintained in five READMEs per repo and had drifted four ways across the 42 plugins: three rows described repos the family no longer publishes, the `dsh-plugin-upgrade` row was missing from every sibling table, nine rows had slipped above their own table header, and `dsh-fund-research`'s Chinese file introduced the family with a sentence no other repo used. All 210 files now carry the same 45-row table, byte-verified per file against its own line endings. [dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) changed roles too — English is now its source of truth — so **all 42 plugins carry five-language docs, every one gated in CI**; that gate was also found in [dsh-plugin-guide](https://github.com/PerryLink/dsh-plugin-guide) having sat for weeks with no workflow calling it, and is now wired.

### 2026-09-21 round

- **[laya-mcp](https://github.com/PerryLink/laya-mcp) is a new project line: Laya typed decisions as an installable sidecar and an MCP server, next to [dsh-laya](https://github.com/PerryLink/dsh-laya), the DSH plugin that puts the same `noul`/`choice`/`score` questions behind a Cordis service and two model-visible tools.** Three published repos carry the line — [dsh-laya](https://github.com/PerryLink/dsh-laya) (0.1.4), [laya-mcp](https://github.com/PerryLink/laya-mcp) (0.1.5) and [laya-mcp-npm](https://github.com/PerryLink/laya-mcp-npm), the Node launcher that finds the Python side and passes the MCP stream through untouched; the three `layacore` name reservations were archived rather than left to look like live projects.
- **[dsh-laya](https://github.com/PerryLink/dsh-laya) installs nothing and downloads nothing** — Laya is PyTorch and cannot live inside a Node plugin, so it is a client of a `laya-mcp serve` process you start yourself, and when that process is not running it says so instead of failing obscurely at the first tool call. One service (`ctx.laya`) plus `laya_ask` and `laya_plan`. The sidecar exists to buy the warm model: the cold build costs seconds to tens of seconds and the default lazy router rebuilds a checkpoint on every language switch.

## 🚀 Flagship picks (start here)

*The six most-starred family plugins (★ measured 2026-09-22); every other family repo is listed in full further down, and the research four-piece set is under [Research](#-research-4).*

| Plugin | What it gives you | Install |
|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | Second-model auto-review on the approval chain, fail-closed by default (193★) | `dsh plugin --profile web add dsh-auto-review` |
| [dsh-research-report](https://github.com/PerryLink/dsh-research-report) | Verifiable research reports: content-addressed evidence ledger, manifest seal hash, byte-level citation checks, drift detection, disproof ledger (152★) | `dsh plugin --profile web add dsh-research-report` |
| [dsh-industry-research](https://github.com/PerryLink/dsh-industry-research) | Industry/company research: chain-map SVG with bottleneck detection, timeline, company cards, adversarial review (150★) | `dsh plugin --profile web add dsh-industry-research` |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Claude Code-style declarative allow/deny/ask rules plus a process-level network policy (114★) | `dsh plugin --profile web add dsh-permission-rules` |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | Approval-gated cross-session memory (`ctx.memory` + SQLite) (108★) | `dsh plugin --profile web add dsh-memento` |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | MCP management console: `/mcp` + Settings tab + trial calls (65★) | `dsh plugin --profile web add dsh-mcp-panel` |

One-command starter pack: **[dsh-kit](https://github.com/PerryLink/dsh-kit)** — installs the core family in one command.

## 📦 The full family — 41 plugins + 5 support repos

*Counting note: the family's own READMEs say "42 plugins" because they count every repo that declares `dsh.bundle.patch`. Measured against all 46 repos this page names: **39 of the 41 plugin rows declare the contract, and 3 of the 5 support repos do** — [dsh-plugin-kit](https://github.com/PerryLink/dsh-plugin-kit) (a review-rule meta package), [dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) (a certification MCP server) and [dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) (the CI health checker); [dsh-catalog](https://github.com/PerryLink/dsh-catalog) and [dsh-kit](https://github.com/PerryLink/dsh-kit) ship none. 39 + 3 = the family's 42. The two plugin rows outside that arithmetic are the sibling project line [jevcore](https://github.com/PerryLink/jevcore) (no `dsh.bundle`; only its `jevcore-dsh` workspace member is a plugin) and the third-party [pan17/dsh-wechat](https://github.com/pan17/dsh-wechat). Both counts therefore describe the same 45 PerryLink-owned repos.*

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

<!-- Instrument, kept out of the rendered text: ★ from `gh api repos/<repo> --jq .stargazers_count`,
     counts from `GET /search/commits?q=repo:<repo>+author:PerryLink`, and a repo counts only when its
     default branch carries at least one commit of ours. `/contributors` is a lagging computed list --
     it returned an empty array for one repo below -- and a merged pull request is not by itself proof:
     one repo merged 32 of them with no commit on its default branch attributed to this account.
     Measured 2026-09-22. Merged work only; open proposals are deliberately not listed here. -->

*Every repo below is external to `PerryLink/*`; every number is measured, merged work only, and open proposals are deliberately not listed.*

**★ 1,000+ — named individually, as the rule requires.** Thirteen external repos above a thousand stars carry merged work:

| Repository | ★ | Merged |
|---|---|---|
| [reactive-resume](https://github.com/reactive-resume/reactive-resume) | 43,315 | 2 PRs |
| [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) | 16,613 | 42 PRs (44 commits) |
| [laya](https://github.com/NandhaKishorM/laya) | 14,755 | 1 PR |
| [FlashMLA](https://github.com/deepseek-ai/FlashMLA) | 12,953 | 1 PR |
| [Cordis](https://github.com/cordiverse/cordis) | 8,746 | 2 PRs |
| [dsh-web](https://github.com/zhu1090093659/dsh-web) | 7,934 | 4 PRs (6 commits) |
| [ouroboros](https://github.com/Q00/ouroboros) | 6,069 | 2 PRs (2 commits) |
| [teamai-cli](https://github.com/Tencent/teamai-cli) | 4,900 | 1 PR |
| [agent-client-protocol](https://github.com/agentclientprotocol/agent-client-protocol) | 4,301 | 2 PRs |
| [deepseek-harness-desktop](https://github.com/dsh-tauri/deepseek-harness-desktop) | 2,496 | 2 PRs (2 commits) |
| [dsh-plugin-radar](https://github.com/AdamPlatin123/dsh-plugin-radar) | 1,464 | 48 PRs (46 commits) |
| [awesome-deepseek-harness](https://github.com/0xsline/awesome-deepseek-harness) | 1,091 | 49 PRs (53 commits) |
| [awesome-vibecoded-saas](https://github.com/Anil-matcha/awesome-vibecoded-saas) | 1,020 | 1 PR |

*Cordis is the upstream plugin-core framework that powers DeepSeek Harness; FlashMLA #224 is the only merged pull request in the whole `deepseek-ai` org.*

**The rest of the contributor set:** [dsh-handbook](https://github.com/Electricitysheep/dsh-handbook) (801★, 2 commits — the official DSH handbook) · [goraven](https://github.com/8treenet/goraven) (737★, 1) · [Zhiyuan-Fan's list](https://github.com/Zhiyuan-Fan/Awesome-DeepSeek-Harness-Plugins) (567★, 5) · [dsh-genui](https://github.com/omdsh-dev/dsh-genui) (473★, 1) · [bruc3van/awesome-dsh-plugin](https://github.com/bruc3van/awesome-dsh-plugin) (358★, 11) · [Dominic789654's list](https://github.com/Dominic789654/awesome-deepseek-harness) (345★, 6) · [imsai-sh's catalog](https://github.com/imsai-sh/awesome-deepseek-harness-plugins) (248★, 41) · [beancookie/awesome-dsh-plugin](https://github.com/beancookie/awesome-dsh-plugin) (150★, 14) · [Oh-My-DSH](https://github.com/like-study1/Oh-My-DSH) (86★, 3) · [walkinglabs' list](https://github.com/walkinglabs/awesome-deepseek-harness-plugins) (29★, 4) · [dsh-advisor](https://github.com/omdsh-dev/dsh-advisor) (22★, 1) · [awesome-deepseekharness](https://github.com/awesome-deepseekharness/awesome-deepseek-harness) (15★, 1) · [jiji262's list](https://github.com/jiji262/awesome-deepseek-harness) (14★, 1) · [vvlife's list](https://github.com/vvlife/awesome-deepseek-harness-plugins) (9★, 3) · [pan17/dsh-wechat](https://github.com/pan17/dsh-wechat) (8★, 2) · [diegosouzapw's catalog](https://github.com/diegosouzapw/awesome-omni-dsh-plugins) (17★, 10). **32 external repositories carry merged work of ours, and 287 merges outside `PerryLink/*` were counted in the 62 external repositories probed for this round — so 287 is a floor, not an estimate.** ([SihanTeng's list](https://github.com/SihanTeng/awesome-deepseek-harness-plugins) carries entries but no attributed commit, so it is deliberately not counted.)

**Security** — published advisory [GHSA-j922-p6h6-p255](https://github.com/PerryLink/dsh-permission-rules/security/advisories/GHSA-j922-p6h6-p255) for dsh-permission-rules (medium, patched in 0.6.16).

**Official harness repo** — it does not accept external pull requests, so that line runs through issues, Discussions (the Show Your Plugins! post [#6104](https://github.com/deepseek-ai/deepseek-harness/discussions/6104)) and the plugin ecosystem instead — while the wider deepseek-ai org is open to fixes (FlashMLA #224 merged).

## 🌍 Where the plugins live

- **GitHub** (this profile), **[Gitee](https://gitee.com/perrylink)** and **npm** — source, CI and releases here; 104 owned repos mirrored to Gitee by a daily job (default branch + all tags); the `perrylink` account holds **55 npm names and 827 versions**, 48 of them active and 44 carrying a provenance attestation
- **npm downloads** — **137,423 over the trailing 30 days** (npm window 08-22..09-20, the last day its daily series covers); **[dshfind](https://dshfind.com/plugins?q=PerryLink)** independently tracks **22k+** across the 8 family plugins it has a download figure for — dshfind reports rounded tiers, so that is a floor rather than a total
- **DSH Desktop Market** — add the catalog source `https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json` under Market → Sources to browse the family in-app; **MCP Registry** — three servers, all published from their release workflows over GitHub OIDC: `dsh-cert-mcp`, `jevcore-mcp` and `laya-mcp`
- **GitHub Actions** — [dsh-github](https://github.com/PerryLink/dsh-github) and [dsh-test-drive](https://github.com/PerryLink/dsh-test-drive) also ship composite actions, so they install as `uses: PerryLink/dsh-test-drive@vX`

Published to a dozen-plus third-party DSH directories and curated lists — [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin), [DSH Directory](https://dsh.directory/plugins?q=perrylink), [Awesome DeepSeek Harness](https://github.com/0xsline/awesome-deepseek-harness), [walkinglabs' list](https://github.com/walkinglabs/awesome-deepseek-harness-plugins), [Zhiyuan-Fan's list](https://github.com/Zhiyuan-Fan/Awesome-DeepSeek-Harness-Plugins), the [AdamPlatin123 radar](https://github.com/AdamPlatin123/dsh-plugin-radar), [dsh-suite](https://github.com/whyihaveyou/dsh-suite), [dshfind.com](https://dshfind.com/zh/plugins/PerryLink/dsh-memento), [deepseek1024.com](https://deepseek1024.com) and [Glama](https://glama.ai/mcp/servers/PerryLink/dsh-cert-mcp) among them — and scored on [OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/PerryLink/dsh-auto-review); the GitHub [`dsh-plugin` topic](https://github.com/topics/dsh-plugin) is what most of them ingest from.

## 中文介绍

我在 DeepSeek Harness 上把自己希望存在的插件做了出来:检查点回退、声明式权限、输出风格、跨会话记忆、MCP 面板、模型档位路由、微信/TickTick 桥接,以及可验证研究报告 / 基金研究 / 行业研究 / 数据质量「研究四件套」——共 **42 个插件**(Apache-2.0):全部带 CI 与 Gitee 镜像,42 个插件仓**全部**带五语文档(五份文件的一致性由每个仓自己的 CI 闸门守着:段落数、安装命令、配置键),且全部声明 `dsh.bundle` 契约。`perrylink` 这个 npm 账号下共有 **55 个名称、827 个版本**:其中 **48 个在用**(本账号 42 个非 scoped + 5 个 `@perrylink/` scoped + pan17 的 `dsh-wechat`),**7 个已弃用**(折进 `dsh-plugin-upgrade` 2.0.0 的三条走廊腿、作者撤回的 `dsh-personal-directive`、改名前的 scoped `@perrylink/dsh-cert-mcp`,以及上面三个已归档的 `layacore` 名字);**55 个里有 44 个**当前 latest 版本带 provenance 证明(11 个没有:`@perrylink/dsh-plugin-doctor`、jevcore 四包、`dsh-laya`、`laya-mcp`、`dsh-wechat`)。下载量近 30 天 **137,423**(窗口 08-22..09-20):8 月 69,059 + 9 月截至 20 日 97,843;按名称拆开是 42 个非 scoped 60.0k/84.7k/120.0k、5 个 scoped 4.0k/8.3k/10.5k、7 个弃用名 2.7k/3.7k/6.3k、pan17 的 dsh-wechat 5.1k/2.8k/4.8k。一键全家桶:[`dsh-kit`](https://github.com/PerryLink/dsh-kit)。同时我是 DeepSeek Harness 上游核心框架 **Cordis**([cordiverse/cordis](https://github.com/cordiverse/cordis))的贡献者,也是 [deepseek-ai](https://github.com/deepseek-ai) 官方仓贡献者:[FlashMLA](https://github.com/deepseek-ai/FlashMLA) 的修复已合并(#224),这是该组织下唯一一条已合并的外部 PR;此外还有 13 个「千星以上」外部仓的已合并贡献(逐仓星数与合并数见上方 Upstream 一节的表格)。

2026-09-23 轮:**这一家子所依赖的那项研究,现在是一篇有 DOI 的论文 —— 而且它测的很大一部分,正是这份主页上的两个项目:[laya-mcp](https://github.com/PerryLink/laya-mcp) 与 [jevcore](https://github.com/PerryLink/jevcore)。**《[当判定层的自报字段说谎时:三类判断层的成本、延迟与失效边界实测](https://doi.org/10.5281/zenodo.22902025)》在一套相同条目上实测了三类判定层:Laya(本地、非自回归)、TypeSafe Jev(远程、定型决策)与 DeepSeek-V4.1-Flash。四条主张,**三条成立,一条被自己的数据否定**。

① **成本不是约束。** 真正分离三者的是**延迟**与**可用状态窗口**;「便宜一个数量级」在状态变大后就不成立了。
② **判定器的接入层自报字段不可信,且失效集中在同一个位置**:截断标志一边报「通过」一边静默丢弃输入、概率字段把条目结论反号、两个判定词在真实输入下根本不可达。这些现象收敛成一条形态 —— **答案被明确陈述时近乎完美(0.9909,n=220),必须注意到「缺席」时塌缩(0.3091,n=220),而两种情形下自报置信度都不低。**
③ **负结果照负结果报。** 异种判定器在三个区制上都**没有**提供增量覆盖:生成器出错时,判定器**比它自己的边际准确率还低**,失败相关在 3/3 次抽样中为正。论文还如实报告了它自己命名的那类错误的**四个实例** ——**规格级缺陷伪装成关于模型的发现** —— 每一个都是被对照抓出来的,不是被审阅抓出来的;那 23 条强制协议条款就来自这里。
④ **两个语言版本各自说明它们是同一项工作。** Zenodo 没有 `is translation of` 这个关系(CORAR 词表里就没有),所以这件事写在**两份 PDF 的扉页**和记录描述里:[英文原文](https://doi.org/10.5281/zenodo.22901853) · [中文译本](https://doi.org/10.5281/zenodo.22902025);制品(代码与全部 `results/` 产物)是第三条记录 [10.5281/zenodo.22901248](https://doi.org/10.5281/zenodo.22901248)。**引其一即可,不要当两篇引;两者有出入以英文为准。**

2026-09-21 轮:① **[laya-mcp](https://github.com/PerryLink/laya-mcp) 是一条新战线:把 Laya 的定型决策做成可安装的 sidecar 与 MCP server,旁边是 [dsh-laya](https://github.com/PerryLink/dsh-laya) —— 把同样的 `noul`/`choice`/`score` 问题放进一个 Cordis service 和两个模型可见的 tool。** 真正发布的只有三个仓:[dsh-laya](https://github.com/PerryLink/dsh-laya)(0.1.4)、[laya-mcp](https://github.com/PerryLink/laya-mcp)(0.1.5),以及负责找到 Python 侧、把 MCP 流原样透传的 Node 启动器 [laya-mcp-npm](https://github.com/PerryLink/laya-mcp-npm);三个 `layacore` 名字仓已归档,只作名称保留,不再像在跑的项目。
② **为什么必须拆开,而不是顺手装。** Laya 是 PyTorch,不可能塞进 Node 插件里,所以 [dsh-laya](https://github.com/PerryLink/dsh-laya) **什么都不装、什么都不下** —— 它是你自己启动的 `laya-mcp serve` 进程的客户端;那个进程没在跑时它会直说,而不是在第一次 tool 调用时莫名其妙地失败。它给出一个 service(`ctx.laya`)外加 `laya_ask` / `laya_plan` 两个 tool。sidecar 存在的意义是买到热模型:冷启动要几秒到几十秒,而默认的懒路由每换一次语言就重建一次 checkpoint。
③ **同一天还有 5 条上游 PR 合并**:[dsh-genui](https://github.com/omdsh-dev/dsh-genui) #194(把 lib 清理挪进 Node,Windows 打包才成立)、[dsh-advisor](https://github.com/omdsh-dev/dsh-advisor) #89(prepare-release 夹具改成 Windows 安全)、[ouroboros](https://github.com/Q00/ouroboros) #2427(随 skill 发布的 Getting Started 链接 404)、[dsh-web](https://github.com/zhu1090093659/dsh-web) #1657、[beancookie/awesome-dsh-plugin](https://github.com/beancookie/awesome-dsh-plugin) #184;同时给 [laya](https://github.com/NandhaKishorM/laya) 本体发了第一条提案(免责声明页脚与会话正文同段时 `clean_email_body` 会整段删掉正文),该提案已于 09-21 合并;另有两提案由我主动关闭,不再留在队列里,也不计入已合并。

#### 2026-09-20 轮

① **[jevcore](https://github.com/PerryLink/jevcore) 是新项目:把 TypeSafe Jev 接进 DeepSeek Harness 与任何其他 MCP host,拆成三个包——`jevcore`(决策内核,不 import 任何 DSH/Cordis 东西)、`jevcore-dsh`(DSH 插件:一个 service、三个 tool、两道 opt-in 门)、`jevcore-mcp`(同样三个 tool 走 MCP,带 stdio 二进制)。三个包今天全部上了 npm:12:53 发 0.1.0,13:06 发 0.1.1,内核已于 13:08 到 0.1.2。** 仓库今天下午新建,头三小时(10:14–13:08)就有 **38 次提交**;MIT,并由 `jevcore-dsh` 通过 `dsh.bundle` 契约。
② **它为什么存在,以及围绕什么保证来写。** 审计那些把 Jev 接进 DSH 的插件后,发现一个被项目自己 README 直说的规律:标着 *guard*、*gate*、*warden* 的那个模块,恰好也是把 prompt、tool 参数和文件内容发往第三方的模块,而 README 一般不说——其中有几个还是默认开启的。jevcore 把这些失效模式设计掉:默认 provider 是离线 mock,走活线要**同时**满足 `provider: live` 与已解析的凭据;每个功能都在启动日志里自报是否外发(`off`,或 `SENDS <feature> { fields }`);被关掉的门**不注册任何**事件监听器,由测试而非策略来保证;没有任何 tool 暴露门的配置,所以模型无法放宽自己的约束;判不出来时走显式配置,默认落到 `ask` 而不是 `allow`。
③ **前一天晚上(09-19)的其他事**:[dsh-plugin-upgrade](https://github.com/PerryLink/dsh-plugin-upgrade) **2.0.0** 把三条已退役的走廊腿折成一个包 + 走廊索引路由(0.1.6-alpha.2 批量 PR 与「已发布线」CI 尺子同时落地)、[dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) **0.2.2** 进入官方 MCP Registry,当晚共 **27 个家族仓 32 个 Release**;其余为例行卫生与依赖升级。

待业中。近期考虑给自己安排一次体检。因此最近将减少熬夜，后续的更新迭代节奏会适当放缓。当然，问题和缺陷修复不会停，只是发布频率会降低一些，还请大家谅解。
