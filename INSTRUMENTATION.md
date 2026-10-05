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
| 42 plugins / 48-repo family / 47 owned | README § intro sentence | a repo joins or leaves the family |
| **plugins badge** *(exception: badge row is the live copy)* | README badge row | same |
| Family roster (which plugins exist) | [`dsh-kit/plugins.txt`](https://github.com/PerryLink/dsh-kit) — already the roster's source of truth, with a parity script | any release |
| npm 30-day downloads | README § Where the plugins live | monthly |
| **npm downloads badge** *(exception)* | README badge row | same |
| npm names / versions / non-deprecated latest | README § Where the plugins live | monthly |
| npm provenance — **state the metric**: 39 names carry SLSA provenance on their non-deprecated `latest`; 44 carry it on at least one version; 41 on their `latest` whatever its state | README § Where the plugins live | monthly |
| dshfind aggregate tier | README § Where the plugins live | when dshfind re-renders |
| dsh host corridor / node engine / license | README badge row (each links to the file it is read from) | when the declared range or the engines change |
| external contributor repos / merges / above-1,000★ | README § Upstream, the "rest of the contributor set" paragraph | on re-derivation |
| The 20-row star table | README § Upstream (the table itself) | on re-derivation |
| laya merged / opened / open / closed | README § Upstream, the laya paragraph | on re-derivation |
| `deepseek-ai` totals | README § Upstream, the "Official harness repo" paragraph | on re-derivation |
| The 1,000★ threshold and the attribution rule | README § Upstream, the lead paragraph | rule change only |
| Round narratives | [`CHANGELOG.md`](CHANGELOG.md) | every round |

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

The node id for this account is `MDQ6VXNlcjI1NTY2NTkwMA==` (user id 255665900).

### Counter-examples are load-bearing — do not delete them

- **`SihanTeng/awesome-deepseek-harness-plugins`** took **32** of this account's merged pull
  requests and credits **no** commit on its default branch.
- **`omdsh-dev/DSH-better-sidebar`** took **1** merge (2026-10-04) with no commit of ours on `main`.
- **`MoonshotAI/checkpoint-engine`** (1,006★) merged a pull request of ours and carries no commit of
  ours, so it is **absent** from the star table.

These three exist to answer "your 43 is padded". Removing them turns a rule into a sales pitch.

### Open proposals are deliberately not listed

The star table is merged work only. Every repository carrying an open proposal is excluded from it
by design, and the README says so in both the lead paragraph and the "rest of the contributor set"
paragraph. Keep both sentences.

---

## 3. The 42 / 44 / 47 / 48 counting note

The page's most attackable number, so the note in the README's family section is the defence.

Measured one repo at a time from each repo's own `package.json` at its default branch:

| Count | Meaning |
|---|---|
| **42** | canonical plugins that declare `dsh.bundle.patch` |
| **44** | a naive scan of the account — 42 canonical **+ 2 retired corridor legs** (`dsh-plugin-upgrade-015`, not archived; `dsh-plugin-upgrade-016`, archived; both still carrying the manifest) |
| **47** | PerryLink-owned repositories the README names |
| **48** | the repositories the README names, including the third-party `pan17/dsh-wechat` |
| **105** | non-fork repositories this account owns in total — 58 of them are not DSH plugins at all (the `loop-*` collection and a set of small LLM utility tools) and are outside this page's scope by design |

`dsh-kit`'s own repository description says **41**; the README and the badge say **42**. Reconcile
these before the next public claim about family size.

---

## 4. Badge row

Re-solved 2026-10-05 for **28 badges in six rows (3,737px)** — a deliberate reversal of the same-day
cut to 6. The badge block is a recognition surface, and every source that resolves is shown rather
than curated down. Measured from each badge's own SVG `width`/`height` at the 20px render height:

| Row | px | Badges |
|---|---|---|
| 1 — reach | 627 | stars, followers, repos, npm names, npm downloads 30d, plugins |
| 2 — quality, licence, registry | 620 | license, OpenSSF Scorecard, Glama (jevcore), Glama (dsh-cert-mcp), MCP Registry |
| 3 — third-party listings | 566 | awesome-dsh-plugin, DSH Directory, DSH Market |
| 4 — mirror, toolchain, catalog | 524 | Gitee, dsh host corridor, node, Desktop Market source |
| 5 — dshfind footprint | 664 | dshfind downloads, dshfind score, dshfind aggregate, certified |
| 6 — activity & research | 736 | dsh-plugin topic, last commit, release, contributors, forks, Zenodo DOI |

**The sizing rule is a cap, not a target.** The first solve packed five rows and let the widest reach
836px; that exceeded the ~811px which earlier editions had already proven renders as one row, so the
last badge on it wrapped and was **stranded alone on the following line**. Keep every row at or under
~800px. Note the two surfaces are not the same width — the file view is ~888px and the profile
column, which is the one that matters here, is narrower — so solve against the narrower one.
A row that is merely "balanced" is not enough: balance is exactly what produced the 836px row.

Rows are grouped by meaning and sized so that no row can wrap. Do **not** append (see the rules
below).

**Hand-written values in the badge row** (each mirrors a README site, and must move with it):

| Badge | Value | Mirrors |
|---|---|---|
| npm names | 52 | "Where the plugins live" |
| npm downloads 30d | 152.6k | "Where the plugins live" (152,643) |
| plugins | 42 | the intro sentence |
| MCP Registry | 3 servers | "Where the plugins live" |
| DSH Desktop Market source | (no number) | the catalog URL |
| Gitee mirror | (no number) | the mirror claim |
| dsh host corridor | ≥0.1.2-rc.1 <0.3.0 | the union of the six `engines.dsh` clauses in any plugin's `package.json` |
| node | ≥22.19 | the same file's `engines.node` (`^22.19.0 \|\| >=24.0.0`) |
| license | Apache-2.0 | the `LICENSE` file |
| dshfind aggregate | 22.5k+ across 8 | "Where the plugins live" |
| dsh-plugin topic | (no number) | the topic page |

Live badges (stars, followers, repos, OpenSSF Scorecard, both Glama scores, MCP-related listings,
dshfind, last commit, release, contributors, forks, Zenodo DOI) need no maintenance.

Two candidates were probed and **not** included, with reasons: a GitHub Sponsors badge
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
- Four figures have no live source and must be updated by hand: the plugin count, the 30-day npm
  download aggregate, the dshfind aggregate, and the third-party listing badges.

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
