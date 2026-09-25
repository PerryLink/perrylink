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
  from the sum of every PerryLink badge's own rendered tier. Tiers are lower bounds, so "21k+" is a
  floor, and only the plugins dshfind currently renders a download figure for are counted (6 of the
  49 it indexes -- 5k+5k+5k+2k+2k+2k, re-summed 2026-09-24; two plugins that carried a figure last
  round now render their star count instead, which is why the badge moved 22k+ -> 21k+ and
  "8 plugins" -> "6 plugins" without any download falling): that is what "across 6 plugins" states.
  Re-sum it when dshfind reports more.

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
<img alt="npm downloads 30d" src="https://img.shields.io/badge/npm%20downloads%2030d-134.9k-6e7781">
<br>
<a href="https://registry.modelcontextprotocol.io/v0/servers?search=perrylink"><img alt="MCP Registry" src="https://img.shields.io/badge/MCP%20Registry-3%20servers-6f42c1"></a>
<a href="https://awesome-dsh-plugin.com"><img alt="awesome-dsh-plugin" src="https://awesome-dsh-plugin.com/badge.svg"></a>
<a href="https://dsh.directory/plugins?q=perrylink"><img alt="Listed on DSH Directory" src="https://dsh.directory/badges/listed.svg"></a>
<a href="https://dsh.market/?q=PerryLink"><img alt="DSH Market" src="https://raw.githubusercontent.com/2BingLing/dsh-market/master/assets/readme/badge-listed-en.svg"></a>
<a href="https://gitee.com/perrylink"><img alt="Gitee mirror" src="https://img.shields.io/badge/Gitee-mirror-c71d23?logo=gitee"></a>
<br>
<a href="https://dshfind.com/plugins/PerryLink/dsh-auto-review?ref=badge"><img alt="dshfind" src="https://dshfind.com/api/badge/PerryLink/dsh-auto-review?metric=downloads"></a>
<a href="https://dshfind.com/plugins?q=PerryLink"><img alt="dshfind downloads across the family" src="https://img.shields.io/badge/dshfind%20downloads-21k%2B%20across%206%20plugins-6e7781"></a>
<a href="https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json"><img alt="DSH Desktop Market source" src="https://img.shields.io/badge/DSH%20Desktop%20Market-source-0969da"></a>
<a href="https://github.com/PerryLink/dsh-plugin-certification"><img alt="Certified dsh-auto-review" src="https://raw.githubusercontent.com/PerryLink/dsh-plugin-certification/main/badges/PerryLink__dsh-auto-review.svg"></a>
<img alt="plugins" src="https://img.shields.io/badge/plugins-42-6e7781">
</p>

**Building the [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness) plugin ecosystem: 42 open-source plugins in a 48-repo family, 47 of them PerryLink-owned — security, workflows, research, messaging bridges, developer experience — plus the DSH Desktop Market catalog, a plugin-certification registry and the dsh-plugin-doctor CI checker. All 42 ship CI and a Gitee mirror, five-language docs held to the same section count, install command and configuration keys by a gate in each repo's own CI, and the `dsh.bundle` contract; 134,856 npm downloads over the trailing 30 days. I also contribute upstream to [Cordis](https://github.com/cordiverse/cordis) — the plugin-core framework DeepSeek Harness is built on — and to [deepseek-ai](https://github.com/deepseek-ai) projects, including a merged [FlashMLA](https://github.com/deepseek-ai/FlashMLA) fix.**

DeepSeek Harness turned "everything is a plugin" into an ecosystem. I build the plugins I wish existed — engineering-discipline guardrails, runtime panels, cross-session memory, and verifiable research engines — and publish them the way production software deserves.

Outside the family: **36 external repositories carry a merged pull request of mine together with a commit attributed to this account, and 17 of them are above a thousand stars** — Tencent's `teamai-cli`, DeepSeek's FlashMLA, cordiverse's Cordis, the ACP repositories Zed and JetBrains jointly govern, and the DSH catalogs — part of the **321 merged pull requests** this account has outside `PerryLink/*`. The measurements behind the family's own judgment layer are published as a paper with a DOI: [*When a Judgment Layer's Self-Reported Fields Lie*](https://doi.org/10.5281/zenodo.22901853), a three-layer measurement (Laya, TypeSafe Jev, DeepSeek-V4.1-Flash) run on [laya-mcp](https://github.com/PerryLink/laya-mcp) and [jevcore](https://github.com/PerryLink/jevcore), with a [Chinese translation](https://doi.org/10.5281/zenodo.22902025) and the [artifact](https://doi.org/10.5281/zenodo.22901248) archived separately.

---

<!-- Round rotation: keep only the newest two rounds (current + one previous). Older rounds live in git history and can be restored on request. Rounds are narrative only — no Snapshot/counter lines: live counts belong to the badge row and "Where the plugins live", and per-edition copies go stale. GHSA/long-lived references belong in "Upstream & community contributions".

     ROUND COUNT, 2026-09-25: both blocks carry two rounds -- 09-25 (current) and
     09-24 (previous). The 09-23 round rotated out to git history by the rule above.
     The 09-25 round is a migration report, not a new narrative: it leads with the
     rc.2 move and the repo that had been left a whole host line behind, because that
     is the one fact in the round a reader cannot get from the badge row. The 09-24
     round keeps its npm measurement verbatim -- a round is a dated snapshot and its
     counters are that round's, not the page's. Earlier rounds (09-23, 09-22, 09-21,
     09-20) live in git history; the 09-21 round was where laya-mcp and dsh-laya were
     introduced by name, and dsh-laya still has its family-table row (the sidecar
     design lives there) while laya-mcp carries a clause in the page intro. -->

## 📣 Latest — 2026-09-25

- **The family moved onto the `0.1.7-rc.2` host line: 41 repositories migrated in one pass, 482 `@deepseek-ai/dsh-*` pins moved off `0.1.7-rc.1`, and 36 packages published at the new patch.** The host window `dsh-v0.1.7-rc.1..rc.2` is 346 commits with no breaking declaration, but unlike the previous window `packages/core/*` did change source this time — an optional `displayReason` on the approval decision, `Session.toolHistory()`, and a tool-registry `developer/message` — all additive, and the one genuinely removed export (`OnboardingSurface`) is referenced nowhere in the family. Admission was re-measured with the host's **own** semver under `includePrerelease`, the predicate its compatibility gate actually uses: **298 peer ranges and 38 `engines.dsh` clauses, zero repositories blocked** — so the declared ranges were deliberately left untouched, and the move is a re-verification rather than a version bump dressed up as one.

- **The sweep found a repository that had been silently left a whole host line behind — and being two lines back was hiding a real API change.** [dsh-test-drive](https://github.com/PerryLink/dsh-test-drive) was still pinned to `0.1.5-rc.2` while the rest of the family sat on `rc.1`: the previous pass rewrote by line number, its anchors did not match that file, and a refused rule was read as "not applicable" instead of a miss. Compiling it against the current line then surfaced what four intermediate lines had absorbed — `jobs.wait`/`read`/`kill` take `caller?: SessionId` where they took `Agent` (the ownership fence compares `owner.id` to the caller directly, not to `caller.id`), and `JobHooks.readOutput` is gone, replaced by the job's own ring writer. Fixed in `src/batch.ts` plus eight test call sites. The lesson is now written into the workflow that produced it: a migration driver classifies by content, never by line number, and a rule that is expected to match but does not is an error rather than a skip.

- **Verified the way that catches a plugin which loads but never starts.** Every repackaged plugin is installed into a throwaway `DSH_HOME` and **booted**, not merely composed — `--dump-config` builds the tree without mounting it, so an activation failure is invisible there. **40 of the 41 pass**, and the one that does not is a `private` data repository with no version at all, which cannot be packed in the first place. Two long-standing red gates were repaired on the way: a repository whose own self-contained check rejects absolute paths was fighting the `/tmp` in its own CI workflow, and an npm-lockfile migration that `npm install` could not resolve needed `npm update --package-lock-only` to move first. Nine repositories were deliberately left out and each is recorded with its reason — three whose host pins live on an unmerged branch, one stopped mid-cherry-pick, one third-party fork, and four with nothing to pin.

### 2026-09-24 round

- **The whole family moved onto the `0.1.7-rc.1` host line in one day: 39 releases across 36 of the 42 plugin repos, 373 commits across 44 of them.** The pins moved from `0.1.7-alpha.2` to `0.1.7-rc.1` and every plugin re-verified against that host; 23 of the 39 release notes name the new line explicitly. The declared peer ranges and `engines.dsh` were deliberately left unchanged — the existing four-clause union already admits the RC — so this is a re-verification, not a version bump dressed up as one. [dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) is the busiest of the day on its own: 32 commits and four releases (0.3.0 → 0.4.4), including a stretch that took it from `0.1.7` to `0.1.7-rc.1` compatibility while the rest of the family followed.

- **`perrylink` on npm, as measured on the 24th: 56 names, 917 versions, 49 active, 42 of them carrying a provenance attestation** — six of the names are scoped `@perrylink/*`, and seven are deprecated on purpose: the three [dsh-plugin-upgrade](https://github.com/PerryLink/dsh-plugin-upgrade) corridor legs folded into 2.0.0, the author-withdrawn `dsh-personal-directive`, the old scoped `@perrylink/dsh-cert-mcp`, and the three archived `layacore` names. Over the trailing 30 days (npm window 08-23..09-21) the account served **134,856 downloads**; that series returns plain zeros for 09-03, 09-07, 09-08, 09-15 and 09-17, so the figure is a floor rather than an exact count.

## 🚀 Flagship picks (start here)

*The six most-starred family plugins (★ measured 2026-09-25); every other family repo is listed in full further down, and the research four-piece set is under [Research](#-research-4).*

| Plugin | What it gives you | Install |
|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | Second-model auto-review on the approval chain, fail-closed by default (201★) | `dsh plugin --profile web add dsh-auto-review` |
| [dsh-industry-research](https://github.com/PerryLink/dsh-industry-research) | Industry/company research: chain-map SVG with bottleneck detection, timeline, company cards, adversarial review (166★) | `dsh plugin --profile web add dsh-industry-research` |
| [dsh-research-report](https://github.com/PerryLink/dsh-research-report) | Verifiable research reports: content-addressed evidence ledger, manifest seal hash, byte-level citation checks, drift detection, disproof ledger (165★) | `dsh plugin --profile web add dsh-research-report` |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | Approval-gated cross-session memory (`ctx.memory` + SQLite) (118★) | `dsh plugin --profile web add dsh-memento` |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Claude Code-style declarative allow/deny/ask rules plus a process-level network policy (114★) | `dsh plugin --profile web add dsh-permission-rules` |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | MCP management console: `/mcp` + Settings tab + trial calls (66★) | `dsh plugin --profile web add dsh-mcp-panel` |

One-command starter pack: **[dsh-kit](https://github.com/PerryLink/dsh-kit)** — installs the core family in one command.

## 📦 The full family — 42 plugins + 5 support repos

*Counting note: "42 plugins" is the figure the family's own READMEs and this page's heading both carry, because it counts every repo that declares `dsh.bundle.patch`. Measured against all 48 repos this page names: **39 of the 41 plugin rows declare the contract, and 3 of the 5 support repos do** — [dsh-plugin-kit](https://github.com/PerryLink/dsh-plugin-kit) (a review-rule meta package), [dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) (a certification MCP server) and [dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) (the CI health checker); [dsh-catalog](https://github.com/PerryLink/dsh-catalog) and [dsh-kit](https://github.com/PerryLink/dsh-kit) ship none. 39 + 3 = the family's 42, measured one repo at a time from each repo's own `package.json`. The two plugin rows outside that arithmetic are the sibling project line [jevcore](https://github.com/PerryLink/jevcore) (no `dsh.bundle`; only its `jevcore-dsh` workspace member is a plugin) and the third-party [pan17/dsh-wechat](https://github.com/pan17/dsh-wechat). Both counts therefore describe the same 47 PerryLink-owned repos: the 41 plugin rows plus the five support repos plus [laya-mcp](https://github.com/PerryLink/laya-mcp), which is named on this page but is not one of the 42.*

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

*Support repos:* [dsh-plugin-kit](https://github.com/PerryLink/dsh-plugin-kit) (review-rule meta package) · [dsh-catalog](https://github.com/PerryLink/dsh-catalog) (DSH Desktop Market catalog source) · [dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) (certification MCP server) · [dsh-kit](https://github.com/PerryLink/dsh-kit) (one-command installer) · [dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) (plugin health checker). Five repos publish under a `@perrylink/` npm name rather than their repo name — the support repos `@perrylink/dsh-plugin-kit` and `@perrylink/dsh-plugin-doctor`, and the plugins `@perrylink/dsh-github`, `@perrylink/dsh-ticktick` and `@perrylink/dsh-skill-pack-security-provider` — and a sixth name, `@perrylink/dsh-cert-mcp`, is the deprecated scoped predecessor of `dsh-cert-mcp`; the `perrylink` account therefore holds 56 names while the family has 42 plugin repos.

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
     `/contributors` is a lagging computed list -- it returned an empty array for one repo below --
     and a merged pull request is not by itself proof: one repo merged 32 of them with no commit on
     its default branch attributed to this account, and another at 1,399★ merged ours on 2026-09-23
     yet its default branch carries only the maintainer's own re-authored commits. Re-derived
     2026-09-24 in one pass: every external repository this account ever opened a pull request
     against (107 of them) was probed with `/contributors`, and the >=1,000★ set is whatever that
     pass returned a commit for -- which is why it is 17 rows here and was 14 the round before, and
     why `MoonshotAI/checkpoint-engine` (1,005★, a merged PR, no commit of ours) is absent.
     Merged work only; open proposals are deliberately not listed here. The merged count comes from
     the account's own pull requests, not from a probe, so it is exact. Attribution re-verified
     through the owners' own profiles and governance pages, which is why the column is here at all:
     a repository path alone does not tell a reader whether Tencent or a weekend maintainer owns
     the project. -->

*Every repo below is external to `PerryLink/*`; every number is measured, merged work only, and open proposals are deliberately not listed. The third column names the project's owner — the account alone does not say whether that is a company, a standards body or one person.*

**★ 1,000+ — named individually, as the rule requires, each carrying the party that owns the project.** Seventeen external repos above a thousand stars carry merged work (★ measured 2026-09-24). Five of those rows belong to a major company or a well-known organization — Tencent, DeepSeek, cordiverse, and the ACP project that Zed and JetBrains jointly govern, which accounts for two of the seventeen; the other twelve are catalog repos, small community orgs and one-person projects, and the column says so rather than letting the account name imply a company:

| Repository | ★ | 项目归属方 |
|---|---|---|
| [reactive-resume](https://github.com/reactive-resume/reactive-resume) | 43,391 | `reactive-resume` org — independent open-source project (rxresu.me) |
| [laya](https://github.com/NandhaKishorM/laya) | 23,111 | NandhaKishorM — individual maintainer; the repo was created 2026-09-18 |
| [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) | 16,812 | `awesome-dsh-plugin` org — community catalog, no company behind it |
| [FlashMLA](https://github.com/deepseek-ai/FlashMLA) | 12,953 | **DeepSeek** — the official `deepseek-ai` org |
| [Cordis](https://github.com/cordiverse/cordis) | 8,794 | **cordiverse** org; its maintainer Shigma is now at **DeepSeek**, and Cordis is the kernel DeepSeek Harness vendors as `@deepseek-ai/cordis` |
| [dsh-web](https://github.com/zhu1090093659/dsh-web) | 7,989 | zhu1090093659 — individual maintainer |
| [ouroboros](https://github.com/Q00/ouroboros) | 6,088 | Q00 — individual maintainer (`@zep-us`) |
| [teamai-cli](https://github.com/Tencent/teamai-cli) | 4,990 | **腾讯 Tencent** — the official `Tencent` org, opensource.tencent.com |
| [dsh-market](https://github.com/dsh-market/dsh-market) | 4,496 | `dsh-market` org — the community plugin market behind dshmarket.com, not a DeepSeek repo |
| [agent-client-protocol](https://github.com/agentclientprotocol/agent-client-protocol) | 4,319 | `agentclientprotocol` org — governed jointly by **Zed Industries** and **JetBrains** |
| [deepseek-harness-desktop](https://github.com/dsh-tauri/deepseek-harness-desktop) | 2,592 | `dsh-tauri` community org — self-described non-official and non-commercial, not a DeepSeek repo |
| [claude-agent-acp](https://github.com/agentclientprotocol/claude-agent-acp) | 2,572 | `agentclientprotocol` org — the same jointly-governed org as the row above, a separate repository |
| [awesome-jev](https://github.com/yibie/awesome-jev) | 1,593 | yibie — individual maintainer, community catalog for Jev |
| [dsh-plugin-radar](https://github.com/AdamPlatin123/dsh-plugin-radar) | 1,465 | AdamPlatin123 — individual maintainer, catalog is a generated artifact |
| [Agents-Anywhere](https://github.com/anywhere-labs/Agents-Anywhere) | 1,181 | `anywhere-labs` community org — 3 public repos, created 2026-05, dshdesktop.cn; not a company |
| [awesome-deepseek-harness](https://github.com/0xsline/awesome-deepseek-harness) | 1,102 | 0xsline — individual maintainer, community catalog |
| [awesome-vibecoded-saas](https://github.com/Anil-matcha/awesome-vibecoded-saas) | 1,022 | Anil Chandra Naidu Matcha — individual maintainer, community catalog |

*Cordis is the upstream plugin-core framework that powers DeepSeek Harness — vendored into that repo and renamed `@deepseek-ai/cordis`; FlashMLA #224 is the only merged pull request in the whole `deepseek-ai` org.*

**The rest of the contributor set** is the community catalog layer rather than upstream projects: **21 further repositories**, DSH plugin directories and small community projects ([dsh-handbook](https://github.com/Electricitysheep/dsh-handbook) among them) — the catalogs ingest the family and carry no company owner, so they are named here only in aggregate. **36 external repositories carry at least one merged pull request of ours together with a commit attributed to this account, and 288 merges were counted inside them** — re-derived 2026-09-25 from this account's own merged pull requests, so 288 is exact rather than a floor over a probed subset. Two further repositories took **33 more** of our merged pull requests **without** crediting a commit to this account on their default branches — [SihanTeng's list](https://github.com/SihanTeng/awesome-deepseek-harness-plugins), 32 of them, which is the case the rule at the top of this section was written about, and [yibie/awesome-jev](https://github.com/yibie/awesome-jev) with 1 — so neither sizes the contributor set. 288 + 33 = the **321 merged pull requests** this account has outside `PerryLink/*`, concentrated in **38 repositories**; a further 14 of our pull requests are open and are deliberately not counted here.

**laya** — [NandhaKishorM/laya](https://github.com/NandhaKishorM/laya) — **24 merged pull requests**, every one this account opened there, and the most of any outside contributor — second only to the maintainer, who commits to `main` directly rather than through pull requests. The next outside contributor has 11. Six areas rather than one:

- **Multilingual routing and evaluation** — a caller-supplied language hint ([#211](https://github.com/NandhaKishorM/laya/pull/211)), a reproducible per-language harness ([#210](https://github.com/NandhaKishorM/laya/pull/210)), a re-run of the 51-language sweep in both temperature regimes ([#222](https://github.com/NandhaKishorM/laya/pull/222)), and a `Router` that no longer picks a checkpoint from a language code naming no language ([#368](https://github.com/NandhaKishorM/laya/pull/368)).
- **HTTP serving and containers** — inference moved off the event loop ([#230](https://github.com/NandhaKishorM/laya/pull/230)), the Compose `laya-serve` service ([#234](https://github.com/NandhaKishorM/laya/pull/234)), and the inference failure the client is not allowed to see now reaching the operator's log ([#375](https://github.com/NandhaKishorM/laya/pull/375)).
- **Email disclaimers and language detection** — the request kept when a disclaimer footer shares its paragraph ([#94](https://github.com/NandhaKishorM/laya/pull/94)), letters counted for the scripts no range claims ([#169](https://github.com/NandhaKishorM/laya/pull/169)), "confidential" no longer read as a disclaimer ([#227](https://github.com/NandhaKishorM/laya/pull/227)), and a `From:` line opening ordinary prose no longer deleting the request ([#371](https://github.com/NandhaKishorM/laya/pull/371)).
- **Correctness and test repairs** — three assertions that could not fail ([#231](https://github.com/NandhaKishorM/laya/pull/231)), the load-time and budget errors no suite reached ([#237](https://github.com/NandhaKishorM/laya/pull/237)), the test suite run on Windows as well as Linux ([#212](https://github.com/NandhaKishorM/laya/pull/212)), an ECE that binned differently from its siblings ([#232](https://github.com/NandhaKishorM/laya/pull/232)), non-ASCII characters kept in non-string instructions ([#228](https://github.com/NandhaKishorM/laya/pull/228)), a README link pointing at a heading that does not exist ([#236](https://github.com/NandhaKishorM/laya/pull/236)), a choice label with no description that came back as a non-string ([#380](https://github.com/NandhaKishorM/laya/pull/380)), [#249](https://github.com/NandhaKishorM/laya/pull/249), where a `noul` criteria dict that cannot be read raises instead of silently falling back to defaults — the line the project's 0.3.11 release note calls "stricter noul criteria" — and [#299](https://github.com/NandhaKishorM/laya/pull/299), two parity cells in the benchmark table that did not match the JSON they cite.
- **The test and CI surface** — [#376](https://github.com/NandhaKishorM/laya/pull/376), six pytest suites that every lane invoked in a way that exited 0 without running a single test, including the only coverage of the HTTP surface.
- **Prediction hooks and batched routing** — process-wide default hooks never reaching `predict_batch` ([#379](https://github.com/NandhaKishorM/laya/pull/379)) and `predict_batch` dropping each request's `lang`, so per-language temperatures never applied ([#381](https://github.com/NandhaKishorM/laya/pull/381)).
- **Documentation** — [#378](https://github.com/NandhaKishorM/laya/pull/378), which stopped the README presenting a confidence threshold as permission to act on its own.

**Fourteen more are open there and deliberately not counted above** — [#389](https://github.com/NandhaKishorM/laya/pull/389), [#416](https://github.com/NandhaKishorM/laya/pull/416), [#418](https://github.com/NandhaKishorM/laya/pull/418), [#419](https://github.com/NandhaKishorM/laya/pull/419), [#420](https://github.com/NandhaKishorM/laya/pull/420), [#422](https://github.com/NandhaKishorM/laya/pull/422), [#423](https://github.com/NandhaKishorM/laya/pull/423), [#424](https://github.com/NandhaKishorM/laya/pull/424), [#425](https://github.com/NandhaKishorM/laya/pull/425), [#426](https://github.com/NandhaKishorM/laya/pull/426), [#427](https://github.com/NandhaKishorM/laya/pull/427), [#428](https://github.com/NandhaKishorM/laya/pull/428), [#454](https://github.com/NandhaKishorM/laya/pull/454) and [#455](https://github.com/NandhaKishorM/laya/pull/455) — each a reproduced defect with a test that fails without the fix, or one of the two guides the project's own docs-structure issue asks contributors to write.

**Security** — published advisory [GHSA-j922-p6h6-p255](https://github.com/PerryLink/dsh-permission-rules/security/advisories/GHSA-j922-p6h6-p255) for dsh-permission-rules (medium, patched in 0.6.16).

**Official harness repo** — it does not accept external pull requests, so that line runs through issues, Discussions (the Show Your Plugins! post [#6104](https://github.com/deepseek-ai/deepseek-harness/discussions/6104)) and the plugin ecosystem instead — while the wider deepseek-ai org is open to fixes (FlashMLA #224 merged).

## 🌍 Where the plugins live

- **GitHub** (this profile), **[Gitee](https://gitee.com/perrylink)** and **npm** — source, CI and releases here; 46 family repos mirrored to Gitee by a daily job (default branch + all tags), plus this profile repo; the `perrylink` account holds **56 npm names and 917 versions**, 49 of them active and 42 carrying a provenance attestation (measured 2026-09-24 against each name's `latest` manifest)
- **npm downloads** — **134,856 over the trailing 30 days** (npm window 08-23..09-21, the last day its daily series covers; that series returns zeros for 09-03, 09-07, 09-08, 09-15 and 09-17, so this is a floor); **[dshfind](https://dshfind.com/plugins?q=PerryLink)** independently tracks **21k+** across the 6 family plugins it currently has a download figure for — dshfind reports rounded tiers, so that is a floor rather than a total
- **DSH Desktop Market** — add the catalog source `https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json` under Market → Sources to browse the family in-app; **MCP Registry** — three servers, all published from their release workflows over GitHub OIDC: `dsh-cert-mcp`, `jevcore-mcp` and `laya-mcp`
- **GitHub Actions** — [dsh-github](https://github.com/PerryLink/dsh-github) and [dsh-test-drive](https://github.com/PerryLink/dsh-test-drive) also ship composite actions, so they install as `uses: PerryLink/dsh-test-drive@vX`

Published to a dozen-plus third-party DSH directories and curated lists — [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin), [DSH Directory](https://dsh.directory/plugins?q=perrylink), [Awesome DeepSeek Harness](https://github.com/0xsline/awesome-deepseek-harness), [walkinglabs' list](https://github.com/walkinglabs/awesome-deepseek-harness-plugins), [Zhiyuan-Fan's list](https://github.com/Zhiyuan-Fan/Awesome-DeepSeek-Harness-Plugins), the [AdamPlatin123 radar](https://github.com/AdamPlatin123/dsh-plugin-radar), [dsh-suite](https://github.com/whyihaveyou/dsh-suite), [dshfind.com](https://dshfind.com/zh/plugins/PerryLink/dsh-memento), [deepseek1024.com](https://deepseek1024.com) and [Glama](https://glama.ai/mcp/servers/PerryLink/dsh-cert-mcp) among them — and scored on [OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/PerryLink/dsh-auto-review); the GitHub [`dsh-plugin` topic](https://github.com/topics/dsh-plugin) is what most of them ingest from.

## 中文介绍

**在 DeepSeek Harness 上构建插件生态:42 个开源插件,来自一个 48 仓的家族(其中 47 个由 PerryLink 自己维护)—— 安全、工作流、研究、消息桥接、开发者体验,外加 DSH Desktop Market 目录、插件认证注册表与 dsh-plugin-doctor 这个 CI 检查器。42 个插件全部带 CI 与 Gitee 镜像,五语文档由每个仓自己的 CI 闸门守着一致(段落数、安装命令、配置键),并声明 `dsh.bundle` 契约;近 30 天 npm 下载 **134,856**(窗口 08-23..09-21)。`perrylink` 这个 npm 账号下共有 **56 个名称、917 个版本**:其中 **49 个在用**(42 个非 scoped + 6 个 `@perrylink/` scoped + pan17 的 `dsh-wechat`)、**7 个已弃用**(`dsh-plugin-upgrade` 折进 2.0.0 的三条走廊腿、作者撤回的 `dsh-personal-directive`、改名前的 scoped `@perrylink/dsh-cert-mcp`,以及三个已归档的 `layacore` 名字)、**42 个**当前 latest 版本带 provenance 证明(均按 2026-09-24 实测)。我也向上游 [Cordis](https://github.com/cordiverse/cordis)(DeepSeek Harness 所基于的插件内核框架)与 [deepseek-ai](https://github.com/deepseek-ai) 项目贡献,包括已合并的 [FlashMLA](https://github.com/deepseek-ai/FlashMLA) 修复(#224,该组织下唯一一条已合并的外部 PR);家族之外**共 36 个外部仓**带着本账号已合并的 PR 与一条归属提交,**其中 17 个在千星以上**。**

**这一家子所依赖的那项研究,现在是一篇有 DOI 的论文 —— 而且它测的很大一部分,正是这份主页上的两个项目:[laya-mcp](https://github.com/PerryLink/laya-mcp) 与 [jevcore](https://github.com/PerryLink/jevcore)。**《[当判定层的自报字段说谎时:三类判断层的成本、延迟与失效边界实测](https://doi.org/10.5281/zenodo.22902025)》在一套相同条目上实测三类判定层(Laya、TypeSafe Jev、DeepSeek-V4.1-Flash),四条主张**三条成立、一条被自己的数据否定**;判定器的接入层自报字段不可信(截断标志报「通过」却静默丢输入、概率字段把结论反号、两个判定词在真实输入下不可达),失效集中在一处 —— 答案被明确陈述时近乎完美(0.9909,n=220),必须注意到「缺席」时塌缩(0.3091,n=220);异种判定器在三个区制上都**没有**增量覆盖。**引其一即可,不要当两篇引**([英文原文](https://doi.org/10.5281/zenodo.22901853) · [中文译本](https://doi.org/10.5281/zenodo.22902025) · [制品](https://doi.org/10.5281/zenodo.22901248));两者有出入以英文为准。

**2026-09-24 轮:全家一天之内搬到 `0.1.7-rc.1` 宿主线 —— 42 个插件仓里有 36 个发了 39 个 Release,其中 23 个发布说明直接点名这条新线,同一天 44 个仓共 373 次提交**(pin 从 `0.1.7-alpha.2` 移到 `0.1.7-rc.1` 并逐仓复验;声明的 peer 区间与 `engines.dsh` **故意不动** —— 原有四段并集本来就容得下这条 RC,所以这是一次复验,不是化妆成复验的版本号变动)。[dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) 是当天最忙的一个:32 次提交、四个 Release(0.3.0 → 0.4.4)。

**laya**([NandhaKishorM/laya](https://github.com/NandhaKishorM/laya))是这个账号投入最深的外部项目:**24 条已合并的 PR** —— 我在那里提的 PR 只有一条由我自己作为重复关闭;外部贡献者里最多,仅次于直接向 `main` 提交(而非走 PR)的维护者。**第二名有 11 条。** 其中 9 条是 2026-09-23 合的,8 条集中在 84 秒之内(13:22:52Z–13:24:16Z);随后 2026-09-24 又合了 9 条,其中 7 条落在 95 秒之内(16:23:42Z–16:25:17Z)。方向不是一个,而是六个:[#211](https://github.com/NandhaKishorM/laya/pull/211)、[#210](https://github.com/NandhaKishorM/laya/pull/210)、[#222](https://github.com/NandhaKishorM/laya/pull/222)、[#368](https://github.com/NandhaKishorM/laya/pull/368)(多语言路由与评测);[#230](https://github.com/NandhaKishorM/laya/pull/230)、[#234](https://github.com/NandhaKishorM/laya/pull/234)、[#375](https://github.com/NandhaKishorM/laya/pull/375)(HTTP 服务与容器);[#94](https://github.com/NandhaKishorM/laya/pull/94)、[#169](https://github.com/NandhaKishorM/laya/pull/169)、[#227](https://github.com/NandhaKishorM/laya/pull/227)、[#371](https://github.com/NandhaKishorM/laya/pull/371)(邮件免责声明与语种判定);[#231](https://github.com/NandhaKishorM/laya/pull/231)、[#237](https://github.com/NandhaKishorM/laya/pull/237)、[#212](https://github.com/NandhaKishorM/laya/pull/212)、[#228](https://github.com/NandhaKishorM/laya/pull/228)、[#236](https://github.com/NandhaKishorM/laya/pull/236)、[#249](https://github.com/NandhaKishorM/laya/pull/249)、[#299](https://github.com/NandhaKishorM/laya/pull/299)、[#232](https://github.com/NandhaKishorM/laya/pull/232)、[#380](https://github.com/NandhaKishorM/laya/pull/380)(代码与测试修正);[#376](https://github.com/NandhaKishorM/laya/pull/376)(测试与 CI 面);[#379](https://github.com/NandhaKishorM/laya/pull/379)、[#381](https://github.com/NandhaKishorM/laya/pull/381)(prediction hooks 与批量路由);[#378](https://github.com/NandhaKishorM/laya/pull/378)(文档)—— 包括项目的**第一条 Windows CI 车道**([#212](https://github.com/NandhaKishorM/laya/pull/212)),Linux 的 16 个 suite 里 15 个现在在 `windows-latest` 上跑。另有 **14 条 PR 仍开放**,按上面的口径不计入。

**还有一条在别处:一个根本起不来的进程现在能起来了。** [claude-agent-acp #1146](https://github.com/agentclientprotocol/claude-agent-acp/pull/1146) 让 `src/index.ts` 里那处没有保护的顶层 await 不再因一次瞬时错误就中断模块求值、在发出任何一条 ACP 消息之前退出。

待业中。十一准备出去玩一圈，所以更新迭代节奏可能短期内仍然提升的有限。当然，问题和缺陷修复不会停，只是发布频率会降低一些，还请大家谅解。
