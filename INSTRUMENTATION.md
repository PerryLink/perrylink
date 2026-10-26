# Instrumentation

Everything that used to sit in `README.md` as invisible HTML comments lives here, plus the rules
that keep the page's numbers honest. **Read this before editing any figure in the README.**

The README carries one pointer comment to this file and nothing else. Round narratives live in
[`CHANGELOG.md`](CHANGELOG.md).

---

## 1. Authoritative value table — one site per figure

The page drifted badly when the same figure was restated in five or six places: as of 2026-10-05
`README.md` asserted the merged-PR total as **350** in one place and **348** in four others, the
laya merged count as 46 and 45, and described `laya#925` as still open after it had been closed
unmerged. **A figure may live in exactly one prose site.** Everything else either links or is
absent. The two sanctioned exceptions are marked.

| Figure | Authoritative site | Update trigger |
|---|---|---|
| 100 actively maintained / 108 in the roster / 175 non-fork owned / 121 with a `package.json` | README § intro sentence for 100; README § family note for 108 | a repo joins, leaves, freezes or retires |
| **plugins badge** *(exception: badge row is the live copy)* | README badge row — carries the actively maintained count, 100 | same |
| Family roster (which plugins exist, and each one's status) | [`dsh-kit/plugins.txt`](https://github.com/PerryLink/dsh-kit) — the install roster, with `scripts/check-parity.mjs` deriving every count and failing on a retired package or a lost status cell | any release |
| Per-repo maintenance status (`active` / `frozen` / `retired`) | [`dsh-plugin-kit/data/repos.json`](https://github.com/PerryLink/dsh-plugin-kit/blob/main/data/repos.json) — the machine-readable roster the portal renders and the certification registry counts | when a repo freezes or retires |
| npm 30-day downloads | README § Where the plugins live | monthly |
| **npm downloads badge** *(exception)* | README badge row | same |
| npm names / versions / non-deprecated latest | README § Where the plugins live | monthly |
| npm provenance — **state the metric**: **96** names carry SLSA provenance on their non-deprecated `latest`; **105** carry it on at least one version; the twelve with none anywhere are named in the page (measured 2026-10-26, over the 117 names registry search now enumerates) | README § Where the plugins live | monthly |
| dshfind aggregate tier — **how to read it**: dshfind publishes a badge per plugin at `/api/badge/<owner>/<repo>?metric=downloads` (the `<img>` every plugin page embeds). Nine of the family's repositories answer with a download tier, 26 fall back to ★. The 35 indexed repositories are counted from its sitemap shards (`/sitemap/plugins-N.xml`), not from the search page, which is client-side | README § Where the plugins live; the nine tiers in `PROJECTS.md` | when dshfind re-renders |
| dsh host corridor / node engine / license | README badge row (each links to the file it is read from) | when the declared range or the engines change |
| external contributor repos / merges / above-1,000★ | README § Upstream, the "rest of the contributor set" paragraph | on re-derivation |
| The named star table — **41 rows above 2,500★**, and the eight between 1,000★ and 2,500★ that live in `PROJECTS.md` | README § Upstream (the table itself) | on re-derivation |
| The long form — upstream narrative, the 105-row roster, the retired/frozen tables, the npm caveats | [`PROJECTS.md`](PROJECTS.md), which the front page links | when the front page is split further |
| laya merged / opened / open / closed | README § Upstream, the laya paragraph | on re-derivation |
| `deepseek-ai` totals | README § Upstream, the "Official harness repo" paragraph | on re-derivation |
| The 1,000★ threshold and the attribution rule | README § Upstream, the lead paragraph | rule change only |
| Round narratives | [`CHANGELOG.md`](CHANGELOG.md) | every round |
| rule-pack size and rules with no verbatim clause text | [`catalog.json`](https://perrylink.github.io/catalog.json), rendered per domain at [the checker index](https://perrylink.github.io/zh/checkers/) | when a rule pack is rebuilt |
| the DSH Desktop Market catalog source URL | [`dsh-catalog`](https://github.com/PerryLink/dsh-catalog) `deploy/artifacts/v1/plugins.json` | when the catalogue is regenerated |
| Phocinae figures (21.0 ms (RTX 5090) / 1.64 s / 0.906 / 0.848 / flip150 0.0200 · flip400 0.0217 / ECE 0.2519 / τ=0.6 → 45.0% escalate, −55.0% LLM calls, kept-subset 0.9936) | README § Phocinae | a Phocinae release re-benchmarks |

**Never** restate an authoritative figure in the intro, in a round, or in the Chinese block. The
Chinese block is a mirror of the story, not a second home for numbers — if it needs a figure, it
links to the English site.

---

## 2. The attribution rule and its probes

The README's upstream section counts a repository only when **its default branch carries at least
one commit authored by this account**. That is the rule; the probe is an implementation detail, and
two implementations were tried and rejected before the current one.

| Probe | Result | Verdict |
|---|---|---|
| `/repos/{r}/contributors` | computed list, **capped at 100 entries**; returns no entry for `yibie/awesome-jev` although that branch carries one of our commits | **rejected** — false negatives |
| `/repos/{r}/commits?author=<login>` | returns `[]` for `pan17/dsh-wechat`, whose default branch holds **three** commits authored by this account | **rejected** — false negatives |
| `defaultBranchRef.target.history(author:{id:<node id>})` | reads real history; agrees with the raw commit-author list on every case tested | **in use** |

The node id for this account is `U_kgDODz0m7A` (GraphQL `user.id`, read 2026-10-26).

### Counter-examples are load-bearing — do not delete them

- **`SihanTeng/awesome-deepseek-harness-plugins`** took **32** of this account's merged pull
  requests and credits **no** commit on its default branch.

That one exists to answer "your 56 is padded". Removing it turns a rule into a sales pitch.

`omdsh-dev/DSH-better-sidebar` was the second entry here until 2026-10-18, recorded as having merged once
(2026-10-04) with no commit of ours on `main`. Re-probed that day: `main` carries **1** commit of this
account, which is why its row sits in the star table at all. It was removed rather than left to age — a
counter-example that has stopped being true is worse than none.

`kellyjonbrazil/jc` was the third, added 2026-10-18 and removed 2026-10-19 for the same reason. Its merge
([#783](https://github.com/kellyjonbrazil/jc/pull/783), 2026-10-17T21:51:22Z) landed on `dev` while the
default branch is `master`; re-probed 2026-10-19, `master` had advanced to `7e67daf2` on
2026-10-18T20:39:02Z and `GET /compare/dev...master` returns `ahead_by: 1`, `behind_by: 0`, so `b6f93354`
is reachable from the default branch and `defaultBranchRef.target.history(author:{id})` returns **1**. It
now earns credit like any other merge.

**A third case was listed here until 2026-10-07 and it was simply wrong.** `MoonshotAI/checkpoint-engine`
(1,006★) was recorded as having merged a pull request of ours while carrying no commit of ours. Re-probed
2026-10-07: this account's only pull request there,
[#108](https://github.com/MoonshotAI/checkpoint-engine/pull/108), is **open and was never merged**
(`state=open`, `merged=false`), and `defaultBranchRef.target.history(author:{id})` returns
`totalCount: 0`. It is not a counter-example at all — it is an open proposal, which the section below
already excludes — so its absence from the star table never needed this entry. The lesson is the one the
table above already taught twice: a remembered case is not a measured one.

### Open proposals are deliberately not listed

The star table is merged work only. Every repository carrying an open proposal is excluded from it
by design, and the README says so in both the lead paragraph and the "rest of the contributor set"
paragraph. Keep both sentences.

---

## 3. The 100 / 108 / 110 / 105 / 175 / 121 counting note

The page's most attackable number, so the note in the README's family section is the defence. **The
heading and the badge carry the actively maintained count (100). The roster figure (108) is stated once,
inside that note** — the intro sentence is the authoritative prose site for 100, not for 108.

Measured one repo at a time from each repo's own `package.json` at its default branch (re-derived 2026-10-26):

| Count | Meaning |
|---|---|
| **100** | actively maintained — the roster minus 3 🚫 retired and 5 🧊 frozen. **This is the number the heading and the badge carry.** |
| **108** | the roster: canonical plugins that declare `dsh.bundle.patch`, excluding the 2 retired corridor legs. `dsh-plugin-kit/data/repos.json` still records the previous **99** cut (2026-10-19); `dsh-kit/plugins.txt` lists 96 published specs (the 99 minus the 3 retired) and does not yet carry the nine 2026-10-23 tools |
| **110** | a naive scan of the account — 108 canonical **+ 2 retired corridor legs** (`dsh-plugin-upgrade-015`, not archived; `dsh-plugin-upgrade-016`, archived; both still carrying the manifest) |
| **105** | rows in the ten categories: 103 of the 108 roster + 2 rows that are not roster plugins (`jevcore`, which declares no `dsh.bundle`, and the third-party `pan17/dsh-wechat`). Five support/tooling roster entries are left out: `dsh-plugin-kit`, `dsh-cert-mcp`, `dsh-plugin-doctor`, `dsh-checkers`, `dsh-community-bench` |
| **175** | non-fork repositories this account owns in total; **121** carry a `package.json` and **110** of those declare `dsh.bundle.patch`, so 65 are outside the contract |
| **121** | `package.json` files at the default branch — the cross-check for the npm-name set, not a page figure |

**2026-10-08: the roster grew by 53.** A set of 53 compliance checkers was published that day
(`dsh-hazchem-check`, `dsh-tender-matrix`, `dsh-icd-rule-check` and so on — the full list is the
`### ✅ Compliance checkers` section of the README). They declare `dsh.bundle.patch` like every other
roster entry, so under this page's own membership rule they are roster plugins, and the counts above
were raised accordingly: 33 → 86, 42 → 95, 41 → 94, 47 → 100, 48 → 101, 105 → 159. The count of
non-plugin repos fell from 58 to 57 because one previously-unclassified repository is accounted for
in the new total.

**2026-10-19: re-derived again.** Two more repositories began declaring `dsh.bundle.patch`
(`dsh-checkers`, `dsh-community-bench`), which moves the roster 97 → 99, the naive scan 99 → 101 and
the actively maintained set 89 → 91; the figures in the table above supersede the 10-08 line. The
non-fork repository total was re-counted the same day: 164, of which 63 declare no
`dsh.bundle.patch`.

**2026-10-20: `dsh-phocinae` moved from the exclusion list into the tables.** It is a roster plugin (its own
`package.json` declares `dsh.bundle.patch`, npm `dsh-phocinae`) that the family note had been leaving out as an
"other product line" repository, so it carried no row, no "Start here" row and no link at all — the page named it
only as an install command. It now has a row, a "Start here" row and a link from the Phocinae section, which moves
the row count to **95** (93 of the 99 roster + `jevcore` + `dsh-wechat`), leaves **six** exclusions, and takes the
linked PerryLink-owned repositories to **103** and the named ones to **104**. The 99 / 91 / 101 figures are unchanged:
the roster it belongs to did not grow.

**2026-10-26: nine new tools and a full re-derivation.** Nine compliance tools published 2026-10-23
(`dsh-bid-health-check`, `dsh-canteen-retention-check`, `dsh-construction-doc-check`, `dsh-excel-reconcile`,
`dsh-invoice-ledger`, `dsh-payroll-audit`, `dsh-safety-ledger-check`, `dsh-table-ingest`,
`dsh-tender-requirements`) declare `dsh.bundle.patch` and are published with a non-deprecated latest. The
naive scan moves 101 → 110, the roster 99 → 108 and the actively maintained set 91 → 100; the tables gain
ten rows (nine tools plus `dsh-phone-inbox`), 95 → 105. The account now owns 175 non-fork repositories, 121
of which carry a `package.json`, and 110 of those declare the contract. The 53-checker suite is unchanged —
the nine are a separate toolchain table. These figures supersede every earlier line in this section.

They are a second workspace on disk (`D:\Projects\dsh-plugins`, disjoint from `D:\Projects\dsh\plugins`)
and carry their own memory file; their maintenance rules, version policy and citation-gate discipline
are recorded there rather than here.

**Reconciled 2026-10-07.** The figure previously drifted: `dsh-kit`'s own repository description said
**41**, its README headline said 42, its family table carried 45 rows, and the per-plugin family tables
said **44** over 45 rows. All of them now derive from one file. `dsh-kit/plugins.txt` then listed **39 npm
specs** — 33 actively maintained plus the 6 frozen, each frozen line carrying a trailing `# 🧊 FROZEN`,
and the 5 retired names documented in the file's header as forbidden. `scripts/check-parity.mjs` derived
33 / 6 / 39 / 42 from that file at the time, fails if a retired package is added back, and fails if a family-table
row's cell count stops matching its header — the defect that had been silently dropping every 🧊 FROZEN
annotation from GitHub's rendering.

---

## 4. Badge row

**The criterion is scope: this is a personal profile, so a badge must describe the account or the
family it maintains, never one repository.** Measured from each badge's own SVG `width`/`height` at
the 20px render height, then partitioned into balanced rows under the cap below.

**Current, re-solved 2026-10-26 for 22 badges in four rows** — every width read from the badge's own
SVG on that date. Twenty-one answered; the Zenodo DOI badge is unreachable from this network (it has
rendered on the page since 2026-10-05 and its width below is the published badge width, not a
measurement).

| Row | px | Badges |
|---|---|---|
| 1 — reach and counters | 686 | stars (90), followers (112), repos (72), upstream merges 442 (138), credited repos 90 (112), plugins 100 (80), checkers 53 (82) |
| 2 — npm and stack | 728 | npm 117 names (123), npm downloads 30d 232.5k (170), npm provenance 105/117 (160), license (120), node (155) |
| 3 — quality and registry | 668 | dsh host corridor (146), OpenSSF Scorecard (136), Glama (110), certified (132), MCP Registry 4 servers (144) |
| 4 — index, mirror, feeds | 787 | plugin index 123 pages (144), Gitee (101), dshfind 45.5k+ across 9 (256), Desktop Market source (172), Zenodo DOI (~114) |

Four hand-written badges joined on that date — `upstream merges`, `credited repos`, `checkers` and
`npm provenance` — because the account-level facts the page argues from had no badge of their own,
while three of the row-2/3 badges describe a single repository. The scope rule above still applies to
`OpenSSF Scorecard` and `certified` only as far as their `alt` text says which repository they name.

Re-solved 2026-10-08 for **21 badges in four rows** (historical). Every width below was re-measured from
each badge's own SVG at the 20px render height:

| Row | px | Badges |
|---|---|---|
| 1 — reach | 748 | stars, followers, repos, npm names, npm downloads 30d, plugins, node |
| 2 — quality, licence, registry | 678 | license, OpenSSF Scorecard, Glama, MCP Registry, awesome-dsh-plugin |
| 3 — listings, mirror, toolchain | 781 | DSH Directory, plugin index, DSH Market, Gitee, dsh host corridor |
| 4 — footprint & research | 753 | dshfind aggregate, Desktop Market source, certified, Zenodo DOI |

**Why `node` moved out of row 3.** Adding the `plugin index` badge (144px) to its natural row — the
listings row — took it to 919px, and every other row was already within 75px of the ~800px cap, so
the new badge had nowhere to go without a swap. `node` (138px) is the toolchain badge whose subject
is least tied to the listings, so it moved to row 1 and the listings row landed at 781px. Moving the
new badge itself to row 1 would also have fit (754px) but would have split the four listings across
two rows, which is the grouping a reader actually uses.

Previously, 2026-10-05, **20 badges in four rows (2,808px)**:

| Row | px | Badges |
|---|---|---|
| 1 — reach | 627 | stars, followers, repos, npm names, npm downloads 30d, plugins |
| 2 — quality, licence, registry | 678 | license, OpenSSF Scorecard, Glama, MCP Registry, awesome-dsh-plugin |
| 3 — listings, mirror, toolchain | 750 | DSH Directory, DSH Market, Gitee, dsh host corridor, node |
| 4 — footprint & research | 753 | dshfind aggregate, Desktop Market source, certified, Zenodo DOI |

**No external source may appear twice.** An expansion to 28 badges had violated that: two Glama
badges (one per MCP server) and two dshfind badges (downloads and score for the same repository),
plus four numbers that belonged to a single repository — `forks 2`, `release v0.12.11`,
`last commit` and `contributors 3`, all of them `dsh-auto-review`'s. A reader sees "forks: 2" on a
personal page and cannot tell whose forks those are or why they matter. Eight were removed:

| Removed | Why |
|---|---|
| Glama (dsh-cert-mcp) | same site as the Glama badge kept, second server — a duplicate, not a second fact |
| dshfind downloads, dshfind score | both are `dsh-auto-review`'s; the family aggregate says the same thing at the right scope |
| `forks 2` | one repository's fork count |
| `release v0.12.11` | one repository's version tag |
| `last commit` | one repository's last commit |
| `contributors 3` | one repository's contributor count |
| `dsh-plugin topic` | a global topic with 17,592 repositories; not this account's property |

Two badges are **kept but scoped in their alt text** — OpenSSF Scorecard and `certified` both point
at the flagship `dsh-auto-review`, and their `alt` now says so, so the badge cannot be read as an
account-wide claim. They are the family's only external quality signal and its own certification
programme, and both were in the original 17.

**The sizing rule is a cap, not a target.** An earlier solve packed five rows and let the widest
reach 836px; that exceeded the ~811px which earlier editions had already proven renders as one row,
so the last badge on it wrapped and was **stranded alone on the following line**. Keep every row at
or under ~800px. The two surfaces are not the same width — the file view is ~888px and the profile
column, which is the one that matters, is narrower — so solve against the narrower one. A row that
is merely "balanced" is not enough: balance is exactly what produced the 836px row.

**Hand-written values** (each mirrors a README site and must move with it):

| Badge | Value | Mirrors |
|---|---|---|
| upstream merges | 442 | "Upstream" and `PROJECTS.md` |
| credited repos | 90 | "Upstream" and `PROJECTS.md` |
| plugins | 100 | the intro sentence |
| checkers | 53 | the 53-checker suite (the nine 2026-10-23 tools are not counted here) |
| npm names | 117 | "Where the plugins live" |
| npm downloads 30d | 232.5k | "Where the plugins live" (232,500) |
| npm provenance | 105/117 | "Where the plugins live" |
| MCP Registry | 4 servers | "Where the plugins live" |
| DSH Desktop Market source | (no number) | the catalog URL — reached over jsDelivr, see the reachability note in §4 |
| Gitee mirror | (no number) | the mirror claim |
| dsh host corridor | ≥0.1.2-rc.1 <0.3.0 | the union of the six `engines.dsh` clauses in any plugin's `package.json` |
| node | ≥22.19 | the same file's `engines.node` (`^22.19.0 \|\| >=24.0.0`) |
| license | Apache-2.0 | the `LICENSE` file |
| dshfind aggregate | 45,500+ over the 9 repositories that carry a badge, of 35 listed | "Where the plugins live"; per-plugin tiers listed in `PROJECTS.md` |

Live badges (stars, followers, repos, OpenSSF Scorecard, Glama, certified, Zenodo DOI) need no
maintenance; the counters, aggregates and third-party listing badges above are hand-written.

Three candidates were probed and **not** included, with reasons: a GitHub Sponsors badge
(`.github/FUNDING.yml` is `github: [PerryLink]`, but the badge renders the sponsor count, which is
0 — a counter that reads as a negative is not recognition), and badges for the other DSH
directories this account is listed in (`0xsline`, `walkinglabs`, `AdamPlatin123`, `dsh-suite` and
`deepseek1024.com` all return 404 or HTML for a badge path — they publish none).

Rules that still hold:

- The shields.io badges use the default `flat` style, matching the family. The Gitee red `c71d23`
  and npm `cb3837` are the sources' own.
- **Do not append a badge to a row.** Adding one changes the total and loses the partition; re-solve
  it and re-measure the widths.
- Do not reuse the widths above after a label change — a single label edit shifts a row.
- The rows are **one `<p>`, not three**, joined by `<br>`: three separate `<p>` blocks each pay
  GitHub's 16px paragraph margin, and a 20px image also shows the font's descent under the text
  baseline. Measured ink-to-ink on the live profile: 21px with three `<p>`, 5px with one.
- The profile renders the README at 14px/21px while the file view uses 16px/24px, so anything tied
  to the line box lands differently on each surface. `align="top"` measured 1px on the profile
  against 4px in the file view and was left off. **Re-measure both surfaces before touching this.**
- The counts, aggregates and third-party listing badges above have no live source and must be updated by
  hand; the star/follower/repo/OpenSSF/Glama/certified/Zenodo badges update themselves.

### Reachability, measured 2026-10-08

A link on this page is only worth its URL if the reader can open it. Most of this project's audience
is in mainland China, where some hosts are interfered with, so the host matters as much as the path:

| Host | Result | Note |
|---|---|---|
| `perrylink-dsh-catalog.perrylink.workers.dev` | **HTTP 000, repeatedly** | DNS resolves to Meta ranges (`66.220.147.11`, `2a03:2880:…:face:b00c:…`), which `*.workers.dev` cannot legitimately be. Interference, not an outage. Replaced by the jsDelivr URL below. |
| `cdn.jsdelivr.net/gh/<owner>/<repo>@<ref>/<path>` | **HTTP 200** | Now carries the catalog source. Has mainland nodes. **Prefer this for any GitHub-hosted file a reader must fetch.** |
| `raw.githubusercontent.com` | **HTTP 200, 6 of 6** | ✅ Reachable. An earlier `HTTP 000` on one request was transient, **not** a block — do not act on a single failure here. |
| `cdn.statically.io` | HTTP 000 | Do not use. |

**Rule:** test a host with repeated requests before concluding it is blocked. One failure is noise;
the `workers.dev` verdict rests on repeated failures plus the DNS evidence, and the
`raw.githubusercontent.com` verdict was corrected the same way after a single failure misled a
first reading.

---

## 5. Round rule

Rounds are **narrative only** — no snapshot or counter lines. Live counts belong to the badge row
and to "Where the plugins live", and per-edition copies go stale.

- A round is a **dated snapshot**. Its counters are that round's, not the page's. **Never "fix" an
  old round's numbers when a later round moves them** — the correction belongs to the later round.
  That is the entire purpose of the rule, and it is what lets dated contradictions coexist on the
  page without either being a lie.
- Rounds live in [`CHANGELOG.md`](CHANGELOG.md). The README links to it and carries no round text.
- Long-lived references — security advisories, and anything else expected to outlive a round —
  belong in the README's Upstream section, not in a round. The GHSA advisory is the worked example.
- **Write date-stamped phrasing, never current-tense phrasing, for anything that moves.** "One is
  open there" rotted within four minutes on 2026-10-04; "as of `<date>`, one was open" cannot.
- **Never commit a whole-file replacement built from a copy you did not re-fetch.** On 2026-10-08 a
  `README.md` written from a pre-raise copy reverted every family figure that the same day's raise had
  moved and deleted the whole 53-checker section, while this file and `CHANGELOG.md` kept the new
  values — so for two hours the page contradicted its own value table. Edit the file you just fetched,
  and write through the Git Data API with a **blob-sha precondition** on every file plus a non-forced
  ref update, so a race aborts the write instead of silently reverting whatever landed in between.

---

## 6. Prose rules

The 2026-10-05 audit measured the page at **337 lines / ~4,300 visible English words / 297 links /
89 table rows**, against a median among 29 well-known maintainer profile READMEs of **26 lines /
125 words / 0 table rows** — 34× the median word count and longer than the largest README in that
sample. The restructure targets roughly 150 lines and a 6–7 minute read.

- Keep the visible page short; **fold, do not delete**. `<details>` is GitHub's only built-in length
  control and is [officially recommended for profile READMEs](https://github.blog/developer-skills/github/5-tips-for-making-your-github-profile-page-accessible/).
- Every figure keeps its **date stamp**. Removing the date turns "measured" into "claimed".
- Keep the **floor and rounding disclaimers** (npm download series has zero-value days; dshfind
  reports rounded tiers). Writing a floor as an exact count is a false claim.
- Split sentences before adding words: the audit found a median sentence of 37 words and five over
  100. One sentence carried nine separate claims.
- Prefer the measured figure over the adjective. "Widely used" is not a measurement.
