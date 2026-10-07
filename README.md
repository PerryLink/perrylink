# Hi, I'm PerryLink 👋

<!-- Editing note: every figure on this page is measured and dated, and each one has exactly one
     authoritative site. Read INSTRUMENTATION.md before changing a number -- it holds the values, the
     probe that produced them, and the rules that keep the page honest. Round narratives live in
     CHANGELOG.md; this page links to them and carries none. Keep it short: fold, do not delete. -->

<p align="center">
<a href="https://github.com/PerryLink?tab=repositories"><img alt="GitHub stars" src="https://img.shields.io/github/stars/PerryLink?label=stars&affiliations=OWNER&color=24292f"></a>
<a href="https://github.com/PerryLink?tab=followers"><img alt="GitHub followers" src="https://img.shields.io/github/followers/PerryLink?label=followers&color=24292f"></a>
<a href="https://github.com/PerryLink?tab=repositories"><img alt="GitHub repos" src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.github.com%2Fusers%2FPerryLink&query=%24.public_repos&label=repos&color=24292f"></a>
<a href="https://www.npmjs.com/search?q=perrylink"><img alt="npm names" src="https://img.shields.io/badge/npm-52%20names-cb3837?logo=npm"></a>
<img alt="npm downloads 30d" src="https://img.shields.io/badge/npm%20downloads%2030d-157.6k-6e7781">
<a href="https://github.com/PerryLink/dsh-kit"><img alt="plugins" src="https://img.shields.io/badge/plugins-42-6e7781"></a>
<br>
<a href="https://github.com/PerryLink/dsh-auto-review/blob/main/LICENSE"><img alt="license" src="https://img.shields.io/badge/license-Apache--2.0-blue"></a>
<a href="https://github.com/PerryLink/dsh-plugin-doctor#readme"><img alt="OpenSSF Scorecard (flagship dsh-auto-review)" src="https://img.shields.io/ossf-scorecard/github.com/PerryLink/dsh-auto-review?label=openssf%20scorecard"></a>
<a href="https://glama.ai/mcp/servers/PerryLink/jevcore"><img alt="Glama (flagship MCP server jevcore)" src="https://glama.ai/mcp/servers/PerryLink/jevcore/badges/score.svg"></a>
<a href="https://registry.modelcontextprotocol.io/v0/servers?search=perrylink"><img alt="MCP Registry" src="https://img.shields.io/badge/MCP%20Registry-3%20servers-6f42c1"></a>
<a href="https://awesome-dsh-plugin.com"><img alt="awesome-dsh-plugin" src="https://awesome-dsh-plugin.com/badge.svg"></a>
<br>
<a href="https://dsh.directory/plugins?q=perrylink"><img alt="DSH Directory" src="https://dsh.directory/badges/listed.svg"></a>
<a href="https://dsh.market/?q=PerryLink"><img alt="DSH Market" src="https://raw.githubusercontent.com/2BingLing/dsh-market/master/assets/readme/badge-listed-en.svg"></a>
<a href="https://gitee.com/perrylink"><img alt="Gitee mirror" src="https://img.shields.io/badge/Gitee-mirror-c71d23?logo=gitee"></a>
<a href="https://github.com/PerryLink/dsh-mcp-panel/blob/main/package.json"><img alt="dsh host corridor" src="https://img.shields.io/badge/dsh-%E2%89%A50.1.2--rc.1%20%3C0.3.0-4B32C3"></a>
<a href="https://github.com/PerryLink/dsh-mcp-panel/blob/main/package.json"><img alt="node" src="https://img.shields.io/badge/node-%E2%89%A522.19-339933?logo=node.js"></a>
<br>
<a href="https://dshfind.com/plugins?q=PerryLink"><img alt="dshfind downloads across the family" src="https://img.shields.io/badge/dshfind%20downloads-22.5k%2B%20across%208%20plugins-6e7781"></a>
<a href="https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json"><img alt="DSH Desktop Market source" src="https://img.shields.io/badge/DSH%20Desktop%20Market-source-0969da"></a>
<a href="https://github.com/PerryLink/dsh-plugin-certification"><img alt="certified (flagship dsh-auto-review)" src="https://raw.githubusercontent.com/PerryLink/dsh-plugin-certification/main/badges/PerryLink__dsh-auto-review.svg"></a>
<a href="https://doi.org/10.5281/zenodo.22901853"><img alt="Zenodo DOI" src="https://zenodo.org/badge/DOI/10.5281/zenodo.22901853.svg"></a>
</p>

Open-source developer in Beijing. I build the
[DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness) plugin ecosystem: 42 Apache-2.0
plugins in a 48-repo family — security, workflows, research, messaging bridges and developer
experience — plus the DSH Desktop Market catalog, a plugin-certification registry and the
dsh-plugin-doctor CI checker. Every plugin ships CI, a Gitee mirror and five-language docs held to
the same section count by a gate in its own CI.

## ▶ Start here

One command installs the core family — **[dsh-kit](https://github.com/PerryLink/dsh-kit)**:

```sh
./install-all.sh web              # Linux / macOS
.\install-all.ps1 -Profile web   # Windows PowerShell
```

| Plugin | What it gives you | Install |
|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | Second-model auto-review on the approval chain, fail-closed by default (234★) | `dsh plugin --profile web add dsh-auto-review` |
| [dsh-research-report](https://github.com/PerryLink/dsh-research-report) | Verifiable research reports: content-addressed evidence ledger, manifest seal hash, byte-level citation checks, drift detection, disproof ledger (214★) | `dsh plugin --profile web add dsh-research-report` |
| [dsh-industry-research](https://github.com/PerryLink/dsh-industry-research) | Industry/company research: chain-map SVG with bottleneck detection, timeline, company cards, adversarial review (213★) | `dsh plugin --profile web add dsh-industry-research` |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | Approval-gated cross-session memory (`ctx.memory` + SQLite) (139★) | `dsh plugin --profile web add dsh-memento` |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Claude Code-style declarative allow/deny/ask rules plus a process-level network policy (119★) | `dsh plugin --profile web add dsh-permission-rules` |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | MCP management console: `/mcp` + Settings tab + trial calls (73★) | `dsh plugin --profile web add dsh-mcp-panel` |

## 🔧 Upstream & community contributions

*Every repo below is external to `PerryLink/*`; every number is measured, merged work only, and open
proposals are deliberately not listed. The third column names the project's owner — the account alone
does not say whether that is a company, a standards body or one person.*

**★ 1,000+ — named individually, as the rule requires, each carrying the party that owns the project.**
Twenty-three external repos above a thousand stars carry merged work (★ measured 2026-10-07), and the newest of them is not a row that merely drifted over the line: `Tencent/BrowserSkill` merged
2026-10-06T13:45:15Z — the most recent of the three, as of that measurement; `awslabs/mcp` had held the
position for the fifteen hours before it and `docker/docker-agent` for the ten before that; `ruvnet/ruflo` and
`walkinglabs/learn-harness-engineering` entered the ten days before those, and `punkpeye/fastmcp` has
carried its merge since 2026-09-24 and was missing from the round before.
Nine of those rows belong to a company or a well-known project organization — Amazon Web Services, Docker, Reactive Resume, DeepSeek,
cordiverse, Tencent, and the ACP project that Zed and JetBrains jointly govern, the last two of which take
two rows each; the other fourteen are catalog repos, small community orgs and one-person projects, and the
column says so rather than letting the account name imply a company:

| Repository | ★ | 项目归属方 |
|---|---|---|
| [ruflo](https://github.com/ruvnet/ruflo) | 74,013 | ruvnet (rUv / Reuven Cohen) — individual maintainer; a 73.8k★ agent harness on a personal account, not a company repo, and the largest row in this table |
| [reactive-resume](https://github.com/reactive-resume/reactive-resume) | 43,919 | `reactive-resume` org — independent open-source project (rxresu.me) |
| [laya](https://github.com/NandhaKishorM/laya) | 31,248 | NandhaKishorM — individual maintainer; the repo was created 2026-09-18 |
| [learn-harness-engineering](https://github.com/walkinglabs/learn-harness-engineering) | 19,415 | `walkinglabs` community org — the harness-engineering tutorial site |
| [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) | 17,932 | `awesome-dsh-plugin` org — community catalog, no company behind it |
| [FlashMLA](https://github.com/deepseek-ai/FlashMLA) | 13,041 | **DeepSeek** — the official `deepseek-ai` org |
| [mcp](https://github.com/awslabs/mcp) | 9,758 | **Amazon Web Services (AWS)** — the official `awslabs` org; a one-file UTF-8 fix merged 2026-10-05T22:49:06Z by maintainer `markjschreiber` with two approvals |
| [BrowserSkill](https://github.com/Tencent/BrowserSkill) | 8,219 | **腾讯 Tencent** — the official `Tencent` org; merged 2026-10-06T13:45:15Z by collaborator `iuyo5678` with eight checks green |
| [Cordis](https://github.com/cordiverse/cordis) | 9,041 | **cordiverse** org; its maintainer Shigma is now at **DeepSeek**, and Cordis is the kernel DeepSeek Harness vendors as `@deepseek-ai/cordis` |
| [dsh-web](https://github.com/zhu1090093659/dsh-web) | 8,441 | zhu1090093659 — individual maintainer |
| [ouroboros](https://github.com/Q00/ouroboros) | 6,189 | Q00 — individual maintainer (`@zep-us`) |
| [dsh-market](https://github.com/dsh-market/dsh-market) | 5,683 | `dsh-market` org — the community plugin market behind dshmarket.com, not a DeepSeek repo |
| [teamai-cli](https://github.com/Tencent/teamai-cli) | 5,136 | **腾讯 Tencent** — the official `Tencent` org, opensource.tencent.com |
| [agent-client-protocol](https://github.com/agentclientprotocol/agent-client-protocol) | 4,382 | `agentclientprotocol` org — governed jointly by **Zed Industries** and **JetBrains** |
| [docker-agent](https://github.com/docker/docker-agent) | 3,377 | **Docker, Inc.** — the official `docker` org; merged 2026-10-05 by maintainer `aheritier` |
| [fastmcp](https://github.com/punkpeye/fastmcp) | 3,272 | punkpeye (Frank Fiegel) — individual maintainer at Glama; the TypeScript MCP framework |
| [deepseek-harness-desktop](https://github.com/dsh-tauri/deepseek-harness-desktop) | 3,058 | `dsh-tauri` community org — self-described non-official and non-commercial, not a DeepSeek repo |
| [claude-agent-acp](https://github.com/agentclientprotocol/claude-agent-acp) | 2,623 | `agentclientprotocol` org — the same jointly-governed org as the row above, a separate repository |
| [awesome-jev](https://github.com/yibie/awesome-jev) | 2,186 | yibie — individual maintainer, community catalog for Jev; the row the 09-25 round both printed and denied, kept now on the commit the history probe finds |
| [dsh-plugin-radar](https://github.com/AdamPlatin123/dsh-plugin-radar) | 1,465 | AdamPlatin123 — individual maintainer, catalog is a generated artifact |
| [Agents-Anywhere](https://github.com/anywhere-labs/Agents-Anywhere) | 1,463 | `anywhere-labs` community org — 3 public repos, created 2026-05, dshdesktop.cn; not a company |
| [awesome-deepseek-harness](https://github.com/0xsline/awesome-deepseek-harness) | 1,141 | 0xsline — individual maintainer, community catalog |
| [awesome-vibecoded-saas](https://github.com/Anil-matcha/awesome-vibecoded-saas) | 1,037 | Anil Chandra Naidu Matcha — individual maintainer, community catalog |

**The rest of the contributor set** is the community catalog layer rather than upstream projects:
**23 further repositories**, DSH plugin directories and small community projects
([dsh-handbook](https://github.com/Electricitysheep/dsh-handbook) and
[imsai-sh's list](https://github.com/imsai-sh/awesome-deepseek-harness-plugins), which alone took 41
merges, among them) — the catalogs ingest the family and carry no company owner, so they are named here
only in aggregate. **46 external repositories carry at least one merged pull request of ours together
with a commit attributed to this account, and 320 merges were counted inside them** — re-derived
2026-10-06 from this account's own merged pull requests, so 320 is exact rather than a floor over a
probed subset. Two further repositories took **33 more** of our merged pull requests **without**
crediting a commit to this account on their default branches —
[SihanTeng's list](https://github.com/SihanTeng/awesome-deepseek-harness-plugins), 32 of them, which is
the case the rule at the top of this section was written about, and
[dsh-better-sidebar](https://github.com/omdsh-dev/DSH-better-sidebar), one, which merged 2026-10-04 and
carries no commit of ours on `main` — so neither sizes the contributor set. 320 + 33 = the
**353 merged pull requests** this account has outside `PerryLink/*`, concentrated in **48 repositories**;
a further **92 are open across 54 repositories** and are deliberately not counted here.

**The ten days since the last round moved the merged count by 30** (2026-09-25 → 2026-10-05, the
window this round re-measured), and 22 of those 30 are `laya` alone — the last of them
[#924](https://github.com/NandhaKishorM/laya/pull/924), which merged 2026-10-04T17:50:19Z and is the
most recent merge this account has anywhere. Six more landed one apiece in six repositories that were
not part of this set at all before — [ruflo](https://github.com/ruvnet/ruflo),
[learn-harness-engineering](https://github.com/walkinglabs/learn-harness-engineering),
[koishi-plugin-booru](https://github.com/koishijs/koishi-plugin-booru),
[dsh-plugin-manager](https://github.com/2768651338/dsh-plugin-manager),
[dsh-plugin-market](https://github.com/losebird/dsh-plugin-market) and
[dsh-annotation](https://github.com/omdsh-dev/dsh-annotation) — which is what puts the largest row in the
table above, `ruflo` at 73,901★, in a set it was not part of ten days ago. The twenty-ninth is
[dsh-better-sidebar](https://github.com/omdsh-dev/DSH-better-sidebar/pull/843), merged
2026-10-04T17:26:07Z, and it is the one merge in the window that credits this account no commit —
which is why it is named in the paragraph above instead of being counted with the other 29. The thirtieth,
and the most recent of all, is [docker-agent#4372](https://github.com/docker/docker-agent/pull/4372) — a
two-file documentation fix merged 2026-10-05T12:14:03Z by Docker maintainer `aheritier`, which is both the
+1 in the total above and the row that puts a seventh company in the table.

**laya** — [NandhaKishorM/laya](https://github.com/NandhaKishorM/laya) — **46 merged pull requests of
the 50 this account has opened there** and **second among merged-PR authors**, behind `aashish254` (126)
and ahead of `Bruce-Yii` (27); the maintainer NandhaKishorM holds one merged PR of his own because he
commits to `main` directly rather than through pull requests, and none of the three leaders is a
collaborator. As of 2026-10-05 it reads **1 open and 3 closed unmerged** — the open one is [#943](https://github.com/NandhaKishorM/laya/pull/943), opened 2026-10-05, where `Router.predictBatch` dropped the per-call `onPredictStart`/`onPredictEnd`/`hooksRaise` arguments; 45 of the 46 merged inside a
nine-day run (2026-09-21 → 2026-09-29), and the maintainer merges in batches — fifteen of them share two
timestamps, seven at `19:29:05` on 09-27 and eight at `17:40:36` on 09-29. The complete list is one
query away:

[`laya` pull requests by this account](https://github.com/NandhaKishorM/laya/pulls?q=is%3Apr+author%3APerryLink)
— the same 49, always current, in any language.

<details>
<summary><b>The 46 merged pull requests, by area</b></summary>

- **Multilingual routing and evaluation** — a caller-supplied language hint
([#211](https://github.com/NandhaKishorM/laya/pull/211)), a reproducible per-language harness
([#210](https://github.com/NandhaKishorM/laya/pull/210)), a re-run of the 51-language sweep in both temperature
regimes ([#222](https://github.com/NandhaKishorM/laya/pull/222)), the multilingual columns refreshed from that re-run
([#389](https://github.com/NandhaKishorM/laya/pull/389)), letters counted for the scripts no range claims
([#169](https://github.com/NandhaKishorM/laya/pull/169)), and a `Router` that no longer picks a checkpoint from a
language code naming no language ([#368](https://github.com/NandhaKishorM/laya/pull/368)).
- **HTTP serving and containers** — inference moved off the event loop
([#230](https://github.com/NandhaKishorM/laya/pull/230)), the Compose `laya-serve` service
([#234](https://github.com/NandhaKishorM/laya/pull/234)), the inference failure the client is not allowed to see now
reaching the operator's log ([#375](https://github.com/NandhaKishorM/laya/pull/375)), a request with no state no
longer answered about the literal text `null` ([#427](https://github.com/NandhaKishorM/laya/pull/427)), and a lone
surrogate in the body returning 400 instead of 500 ([#454](https://github.com/NandhaKishorM/laya/pull/454)).
- **Email disclaimers and names** — the request kept when a disclaimer footer shares its paragraph
([#94](https://github.com/NandhaKishorM/laya/pull/94)), "confidential" no longer read as a disclaimer
([#227](https://github.com/NandhaKishorM/laya/pull/227)), a `From:` line opening ordinary prose no longer deleting the
request ([#371](https://github.com/NandhaKishorM/laya/pull/371)), and a name class that excluded lowercase in every
script ([#503](https://github.com/NandhaKishorM/laya/pull/503)).
- **Correctness across the call surface** — three assertions that could not fail
([#231](https://github.com/NandhaKishorM/laya/pull/231)), the load-time and budget errors no suite reached
([#237](https://github.com/NandhaKishorM/laya/pull/237)), an ECE that binned differently from its siblings
([#232](https://github.com/NandhaKishorM/laya/pull/232)), non-ASCII characters kept in non-string instructions
([#228](https://github.com/NandhaKishorM/laya/pull/228)), a README link pointing at a heading that does not exist
([#236](https://github.com/NandhaKishorM/laya/pull/236)), a choice label with no description that came back as a
non-string ([#380](https://github.com/NandhaKishorM/laya/pull/380)), a nested choice label reported as a named caller
error instead of a bare `TypeError` ([#425](https://github.com/NandhaKishorM/laya/pull/425)), a score legend that
echoed the caller's own type instead of level text ([#420](https://github.com/NandhaKishorM/laya/pull/420)),
`hooks_installed` removing a hook it did not install ([#424](https://github.com/NandhaKishorM/laya/pull/424)), a null
`choice` label that made the answer undecodable ([#508](https://github.com/NandhaKishorM/laya/pull/508)), a short
temperature list that now fails at load rather than at the first decode
([#502](https://github.com/NandhaKishorM/laya/pull/502)), [#249](https://github.com/NandhaKishorM/laya/pull/249),
where a `noul` criteria dict that cannot be read raises instead of silently falling back to defaults — the line the
project's 0.3.11 release note calls "stricter noul criteria" — and
[#299](https://github.com/NandhaKishorM/laya/pull/299), two parity cells in the benchmark table that did not match the
JSON they cite.
- **The test and CI surface** — the Windows lane ([#212](https://github.com/NandhaKishorM/laya/pull/212)) and
[#376](https://github.com/NandhaKishorM/laya/pull/376), six pytest suites that every lane invoked in a way that exited
0 without running a single test, including the only coverage of the HTTP surface.
- **Prediction hooks and batched routing** — process-wide default hooks never reaching `predict_batch`
([#379](https://github.com/NandhaKishorM/laya/pull/379)), `predict_batch` dropping each request's `lang`, so
per-language temperatures never applied ([#381](https://github.com/NandhaKishorM/laya/pull/381)), and
`lang_temperatures` crashing on the inputs it exists to reject
([#428](https://github.com/NandhaKishorM/laya/pull/428)).
- **The TypeScript front end** — the `From:` header rules the Python side already had, ported rather than re-derived
([#422](https://github.com/NandhaKishorM/laya/pull/422)); the Azerbaijani schwa counted as a non-English letter
([#423](https://github.com/NandhaKishorM/laya/pull/423)); and a score legend that echoed the caller's own types,
unlike the Python backends ([#556](https://github.com/NandhaKishorM/laya/pull/556)).
- **CLI, packaging and serving edges** — `--preset` sending the request under a key no question set names
([#426](https://github.com/NandhaKishorM/laya/pull/426)); the onnx extra missing its `onnxscript` dependency
([#504](https://github.com/NandhaKishorM/laya/pull/504)); the packaging test scanning `.venv` for broken links
([#500](https://github.com/NandhaKishorM/laya/pull/500)); and two over-budget messages that each named a knob which
makes the problem worse rather than the one that fixes it ([#455](https://github.com/NandhaKishorM/laya/pull/455),
[#501](https://github.com/NandhaKishorM/laya/pull/501)).
- **Documentation** — [#378](https://github.com/NandhaKishorM/laya/pull/378), which stopped the README presenting a
confidence threshold as permission to act on its own, and the pages the project's docs-structure issue asked
contributors to write: the fine-tuning guide ([#505](https://github.com/NandhaKishorM/laya/pull/505)), the Questions
and answers guide ([#418](https://github.com/NandhaKishorM/laya/pull/418)), and the reference entry for
`answer_confidence`, which no page documented ([#419](https://github.com/NandhaKishorM/laya/pull/419)).

*The nine area headings above are this account's own grouping of its 45 nine-day merges, not the
project's taxonomy; the merge counts are the repository's own.*

Three closures, and the reason is on the record for each:
[#370](https://github.com/NandhaKishorM/laya/pull/370), closed by this account as a duplicate of
[#362](https://github.com/NandhaKishorM/laya/pull/362), which opened the same fix four minutes earlier;
[#416](https://github.com/NandhaKishorM/laya/pull/416), the Routing guide, closed by the maintainer in
favour of another contributor's [#461](https://github.com/NandhaKishorM/laya/pull/461) so the project
would not carry two routing pages; and [#925](https://github.com/NandhaKishorM/laya/pull/925), closed
unmerged at 2026-10-04T17:54:52Z, four minutes after [#924](https://github.com/NandhaKishorM/laya/pull/924)
merged.

</details>

**Security** — published advisory [GHSA-j922-p6h6-p255](https://github.com/PerryLink/dsh-permission-rules/security/advisories/GHSA-j922-p6h6-p255) for dsh-permission-rules (medium, patched in 0.6.16).

**Official harness repo** — it does not accept external pull requests, so that line runs through issues, Discussions
(the Show Your Plugins! post [#6104](https://github.com/deepseek-ai/deepseek-harness/discussions/6104)) and the plugin
ecosystem instead — while the wider `deepseek-ai` org is open to fixes, and the account now proposes them at the
systems layer rather than only in its catalogs: of the **20 pull requests it has opened across that org, FlashMLA
[#224](https://github.com/deepseek-ai/FlashMLA/pull/224) remains the only one merged**, and **16 are open**, 14 of
them code fixes carrying a reproduction across ten repositories — [DeepEP](https://github.com/deepseek-ai/DeepEP)
three, [FlashMLA](https://github.com/deepseek-ai/FlashMLA) and
[deepseek-recipe](https://github.com/deepseek-ai/deepseek-recipe) two each, and one apiece in
[DeepGEMM](https://github.com/deepseek-ai/DeepGEMM), [3FS](https://github.com/deepseek-ai/3FS),
[TileKernels](https://github.com/deepseek-ai/TileKernels),
[DeepSeek-MoE](https://github.com/deepseek-ai/DeepSeek-MoE),
[DeepSeek-Prover-V1.5](https://github.com/deepseek-ai/DeepSeek-Prover-V1.5),
[DeepJIT](https://github.com/deepseek-ai/DeepJIT) and [DeepSelect](https://github.com/deepseek-ai/DeepSelect) — the
other two are catalog additions.

## 📦 The rest of the family

The other 36 plugins and the five support repos are one line each below. The roster's source of truth
is **[dsh-kit](https://github.com/PerryLink/dsh-kit)** — its `plugins.txt` and a parity script hold the
family to that file; the machine-readable catalogue is
**[dsh-catalog](https://github.com/PerryLink/dsh-catalog)**, which is also the DSH Desktop Market source;
and each plugin's own README carries the detail this page only summarises.

<details>
<summary><b>The full family — 42 plugins + 5 support repos, one line each</b></summary>

*Counting note: "42 plugins" counts every repo that declares `dsh.bundle.patch`, re-derived one repo at a time on
2026-10-04 by reading each repo's own `package.json` at its default branch. Measured against the 47 PerryLink-owned
repositories this page names: **42 declare the contract and 5 do not** — the support trio
[dsh-catalog](https://github.com/PerryLink/dsh-catalog), [dsh-kit](https://github.com/PerryLink/dsh-kit) and
[dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification) (the certification registry, whose
MCP server publishes from [dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) instead), plus
[jevcore](https://github.com/PerryLink/jevcore) (no `dsh.bundle`; only its `jevcore-dsh` workspace member is a plugin)
and [laya-mcp](https://github.com/PerryLink/laya-mcp) (an MCP sidecar, not a plugin). The third-party
[pan17/dsh-wechat](https://github.com/pan17/dsh-wechat) carries a plugin row but is not one of them: 47 + 1 = the 48
repos this page names. A naive scan of the account finds two more than the heading claims — the retired
[dsh-plugin-upgrade](https://github.com/PerryLink/dsh-plugin-upgrade) corridor legs `dsh-plugin-upgrade-015` and
`dsh-plugin-upgrade-016`, both archived, both still carrying the manifest, and neither an active plugin: 42 active + 2
retired = the 44 such a scan returns. The heading and the badge keep the active figure.*

### 🔒 Security (4)

| Plugin | One-liner | Status | npm |
|---|---|---|---|
| [dsh-defend](https://github.com/PerryLink/dsh-defend) | Injection/jailbreak/secret detection + destructive-delete gate | 🧊 FROZEN — broader detector, but frozen | [npm](https://www.npmjs.com/package/dsh-defend) |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Declarative allow/deny/ask rules + a local HTTP/CONNECT network policy | | [npm](https://www.npmjs.com/package/dsh-permission-rules) |
| [dsh-mask](https://github.com/PerryLink/dsh-mask) | PII masking/sanitization | | [npm](https://www.npmjs.com/package/dsh-mask) |
| [dsh-skill-pack-security](https://github.com/PerryLink/dsh-skill-pack-security) | Security-audit skill pack + supply-chain gate | | [npm](https://www.npmjs.com/package/@perrylink/dsh-skill-pack-security-provider) |

### 🔁 Workflows (8)

| Plugin | One-liner | Status | npm |
|---|---|---|---|
| [dsh-background-agents](https://github.com/PerryLink/dsh-background-agents) | Durable background child agents with a Web UI sidebar, messaging and interrupt | 🚫 RETIRED — native continuable subagents | [npm](https://www.npmjs.com/package/dsh-background-agents) |
| [dsh-team-rooms](https://github.com/PerryLink/dsh-team-rooms) | Cross-session team rooms: shared message bus, task board, approval-gated handoffs and a timeline that survive restarts | 🚫 RETIRED — native Agent Teams | [npm](https://www.npmjs.com/package/dsh-team-rooms) |
| [dsh-checkpoint-rewind](https://github.com/PerryLink/dsh-checkpoint-rewind) | Snapshots, forks, one-shot restore | | [npm](https://www.npmjs.com/package/dsh-checkpoint-rewind) |
| [dsh-github](https://github.com/PerryLink/dsh-github) | GitHub PR/issue integration + Action, writes approval-gated | | [npm](https://www.npmjs.com/package/@perrylink/dsh-github) |
| [dsh-claude-move](https://github.com/PerryLink/dsh-claude-move) | Migrate Claude Code/Codex/OpenCode/Hermes into DSH | 🧊 FROZEN — `dsh-chat-import` | [npm](https://www.npmjs.com/package/dsh-claude-move) |
| [dsh-click](https://github.com/PerryLink/dsh-click) | Desktop control tools (Windows/macOS) | | [npm](https://www.npmjs.com/package/dsh-click) |
| [dsh-session-sync](https://github.com/PerryLink/dsh-session-sync) | Git-backed session synchronization | | [npm](https://www.npmjs.com/package/dsh-session-sync) |
| [dsh-test-drive](https://github.com/PerryLink/dsh-test-drive) | Install→smoke→uninstall test driver for plugins | | [npm](https://www.npmjs.com/package/dsh-test-drive) |

### ✨ Experience & UX (4)

| Plugin | One-liner | Status | npm |
|---|---|---|---|
| [dsh-composer-history](https://github.com/PerryLink/dsh-composer-history) | Terminal-style input history for the web composer | | [npm](https://www.npmjs.com/package/dsh-composer-history) |
| [dsh-output-styles](https://github.com/PerryLink/dsh-output-styles) | Runtime-switchable model output styles | | [npm](https://www.npmjs.com/package/dsh-output-styles) |
| [dsh-session-pin](https://github.com/PerryLink/dsh-session-pin) | Pin sessions in the Web sidebar | 🚫 RETIRED — native session pinning | [npm](https://www.npmjs.com/package/dsh-session-pin) |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | Approval-gated cross-session memory protocol | 🧊 FROZEN — `@openviking/dsh-memory-plugin` | [npm](https://www.npmjs.com/package/dsh-memento) |

### 🧪 Evaluation (3)

| Plugin | One-liner | Status | npm |
|---|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | Second-model auto-review on the approval chain | | [npm](https://www.npmjs.com/package/dsh-auto-review) |
| [dsh-doublecheck](https://github.com/PerryLink/dsh-doublecheck) | Engineering-discipline guard: grill, gates, adversary review | | [npm](https://www.npmjs.com/package/dsh-doublecheck) |
| [dsh-score](https://github.com/PerryLink/dsh-score) | Plugin quality scoring across git/gh/npm | | [npm](https://www.npmjs.com/package/dsh-score) |

### 📊 Observability & cost (4)

| Plugin | One-liner | Status | npm |
|---|---|---|---|
| [dsh-autotier](https://github.com/PerryLink/dsh-autotier) | Automatic strong/cheap model-tier routing with deterministic risk guards | | [npm](https://www.npmjs.com/package/dsh-autotier) |
| [dsh-budget](https://github.com/PerryLink/dsh-budget) | Token/cost metering, budget caps, carbon estimate, latency benchmarks | 🧊 FROZEN — `dsh-cost-meter` | [npm](https://www.npmjs.com/package/dsh-budget) |
| [dsh-observe](https://github.com/PerryLink/dsh-observe) | OTel/Langfuse telemetry export | | [npm](https://www.npmjs.com/package/dsh-observe) |
| [dsh-fast](https://github.com/PerryLink/dsh-fast) | Performance diagnostics | | [npm](https://www.npmjs.com/package/dsh-fast) |

### 🎨 Content & knowledge (5)

| Plugin | One-liner | Status | npm |
|---|---|---|---|
| [dsh-draw](https://github.com/PerryLink/dsh-draw) | Image-generation routing | 🧊 FROZEN — `dsh-image-gen` | [npm](https://www.npmjs.com/package/dsh-draw) |
| [dsh-translate](https://github.com/PerryLink/dsh-translate) | Translation + JSON repair | | [npm](https://www.npmjs.com/package/dsh-translate) |
| [dsh-talk](https://github.com/PerryLink/dsh-talk) | Speech recognition and voice I/O | | [npm](https://www.npmjs.com/package/dsh-talk) |
| [dsh-library](https://github.com/PerryLink/dsh-library) | Local knowledge-base RAG | | [npm](https://www.npmjs.com/package/dsh-library) |
| [dsh-local-ai](https://github.com/PerryLink/dsh-local-ai) | Ollama LLM provider and routing | | [npm](https://www.npmjs.com/package/dsh-local-ai) |

### 🛠️ Developer experience (6)

| Plugin | One-liner | Status | npm |
|---|---|---|---|
| [dsh-lsp-actions](https://github.com/PerryLink/dsh-lsp-actions) | LSP diagnostics/formatting/completion/actions | | [npm](https://www.npmjs.com/package/dsh-lsp-actions) |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | MCP management console | | [npm](https://www.npmjs.com/package/dsh-mcp-panel) |
| [dsh-plugin-guide](https://github.com/PerryLink/dsh-plugin-guide) | Plugin-dev knowledge base + CLI toolchain + release-engineering guide | | [npm](https://www.npmjs.com/package/dsh-plugin-guide) |
| [dsh-plugin-upgrade](https://github.com/PerryLink/dsh-plugin-upgrade) | Plugin-author upgrade skill: one package, one corridor index that detects the caller's peer band and routes to the matching closed card (`0.1.3-alpha.1 → 0.1.5-rc.1`, `0.1.5-rc.2 → 0.1.6-alpha.2`), plus a zero-dependency seam scanner (bundle skill + npx CLI) | | [npm](https://www.npmjs.com/package/dsh-plugin-upgrade) |
| [jevcore](https://github.com/PerryLink/jevcore) | TypeSafe Jev as typed decisions instead of prose (`noul`/`choice`/`score` with calibrated probabilities): offline by default, every transmission named before it happens, disabled gates register nothing (the DSH adapter `jevcore-dsh`, plus `jevcore` core and `jevcore-mcp` for non-DSH MCP hosts) | | [npm](https://www.npmjs.com/package/jevcore-dsh) |
| [dsh-laya](https://github.com/PerryLink/dsh-laya) | Laya typed decisions (`noul`/`choice`/`score`) as a first-class Cordis service (`ctx.laya`) plus `laya_ask`/`laya_plan` tools; a client of a `laya-mcp serve` sidecar, so it installs and downloads nothing, and reports whether state stays on this machine as a fact rather than a policy | | [npm](https://www.npmjs.com/package/dsh-laya) |

*Support repos:* [dsh-plugin-kit](https://github.com/PerryLink/dsh-plugin-kit) (review-rule meta package) ·
[dsh-catalog](https://github.com/PerryLink/dsh-catalog) (DSH Desktop Market catalog source) ·
[dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) (certification MCP server) ·
[dsh-kit](https://github.com/PerryLink/dsh-kit) (one-command installer) ·
[dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) (plugin health checker). Five of these repos and
plugins publish under a `@perrylink/` npm name rather than their repo name — the support repos
`@perrylink/dsh-plugin-kit` and `@perrylink/dsh-plugin-doctor`, and the plugins `@perrylink/dsh-github`,
`@perrylink/dsh-ticktick` and `@perrylink/dsh-skill-pack-security-provider` — and a sixth name,
`@perrylink/dsh-cert-mcp`, is the deprecated scoped predecessor of `dsh-cert-mcp`; the `perrylink` account therefore
holds **52 npm names** while the family has 42 plugin repos (measured 2026-10-04).

### 📱 Messaging & bridges (3)

| Plugin | One-liner | Status | npm |
|---|---|---|---|
| [dsh-wechat](https://github.com/pan17/dsh-wechat) | WeChat ↔ DSH bridge (Tencent iLink bot): text/image/file/voice, approvals in chat — developed with [pan17](https://github.com/pan17/dsh-wechat), who now hosts the repo and publishes the npm package | 🧊 FROZEN — `@xmanrui/dsh-im` | [npm](https://www.npmjs.com/package/dsh-wechat) |
| [dsh-ticktick](https://github.com/PerryLink/dsh-ticktick) | TickTick/Dida365 task bridge: session-header panel + 11 tools | | [npm](https://www.npmjs.com/package/@perrylink/dsh-ticktick) |
| [dsh-reach](https://github.com/PerryLink/dsh-reach) | Multi-channel approval/question bridge: WeChat/Telegram/Feishu, session console | 🧊 FROZEN — `@xmanrui/dsh-im` | [npm](https://www.npmjs.com/package/dsh-reach) |

### 🔬 Research (4)

| Plugin | One-liner | Status | npm |
|---|---|---|---|
| [dsh-data-quality](https://github.com/PerryLink/dsh-data-quality) | Data profiling/cleaning/verification | | [npm](https://www.npmjs.com/package/dsh-data-quality) |
| [dsh-fund-research](https://github.com/PerryLink/dsh-fund-research) | Mutual-fund research, sealed traceable snapshots | | [npm](https://www.npmjs.com/package/dsh-fund-research) |
| [dsh-industry-research](https://github.com/PerryLink/dsh-industry-research) | Industry/company research domain pack | | [npm](https://www.npmjs.com/package/dsh-industry-research) |
| [dsh-research-report](https://github.com/PerryLink/dsh-research-report) | Verifiable research-report engine | | [npm](https://www.npmjs.com/package/dsh-research-report) |

</details>

## 🪦 Retired & frozen (2026-10-05)

A maintainer review of the whole family against the official harness and the wider plugin ecosystem
concluded that three of these plugins duplicate capabilities the **official harness now implements
natively**, and one was reclassified as internal tooling. Retirement here has a precise meaning:
**compatibility updates stop because the capability is now official, or because a better-adopted
alternative exists** — these are not abandoned or broken, and they keep working for existing installs.

### Retired — the official harness now implements this

| Plugin | Why | Use instead |
|---|---|---|
| [dsh-background-agents](https://github.com/PerryLink/dsh-background-agents) | The official harness ships **native continuable subagents** — `subagent` with `backgroundMode: continuable`, plus `send_message` / `interrupt_agent` / `list_agents` / `job_*`, mounted inside `dsh-base` | the native continuable subagents |
| [dsh-session-pin](https://github.com/PerryLink/dsh-session-pin) | The official harness **ships session pinning natively** — the row menu and hover button in `dsh-client-ui-workspace`, with the pin set persisted on the Host and mounted in the default Web bundle | the built-in session pin |
| [dsh-team-rooms](https://github.com/PerryLink/dsh-team-rooms) | The official harness ships the **Agent Teams** subsystem (`dsh-experimental-agent-team`): implicit-root roster, durable peer mailbox and a shared task DAG. Well-adopted community alternatives exist too | native Agent Teams, or [`@nanmicoder/dsh-agent-teams`](https://github.com/NanmiCoder/dsh-agent-teams) |

**Reclassified, not retired:** [dsh-catalog](https://github.com/PerryLink/dsh-catalog) is now treated as
**family-internal tooling** rather than a product. It is live infrastructure feeding the DSH Desktop
Community Market, and its job is to inventory this family — so it does not compete with third-party
catalogs and needs no retirement.

### Frozen — no new features, only real breakages fixed

Frozen because **better-adopted alternatives now exist** for that capability. Each repo's README records
the measured comparison. Weekly npm downloads, measured 2026-10-05:

| Plugin | this repo | better-adopted alternative |
|---|---|---|
| [dsh-budget](https://github.com/PerryLink/dsh-budget) | 1,079 | [`dsh-cost-meter`](https://github.com/Han-1413141/dsh-cost-meter) — **33,526** |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | 1,202 | [`@openviking/dsh-memory-plugin`](https://github.com/volcengine/OpenViking) — **10,160** |
| [dsh-draw](https://github.com/PerryLink/dsh-draw) | 973 | [`dsh-image-gen`](https://github.com/shanliuling/dsh-image-gen) — **7,216** |
| [dsh-claude-move](https://github.com/PerryLink/dsh-claude-move) | 843 | [`dsh-chat-import`](https://github.com/Nwflower/dsh-chat-import) — **5,111** |
| [dsh-reach](https://github.com/PerryLink/dsh-reach) | ~600 | [`@xmanrui/dsh-im`](https://github.com/xmanrui/dsh-im) — **17,384** |
| [dsh-wechat](https://github.com/pan17/dsh-wechat) | 752 | [`@xmanrui/dsh-im`](https://github.com/xmanrui/dsh-im) — **17,384** |
| [dsh-defend](https://github.com/PerryLink/dsh-defend) | 937 | [`cc-safety-net`](https://github.com/kenryu42/cc-safety-net) — **13,087** |

`dsh-defend` is the one frozen package that is still the **broader** detector — an Aho-Corasick engine over
the prompt-injection / jailbreak / secret-leaker asset sets, with three-way allow/ask/block interception on
user messages, tool arguments **and** tool results. It is frozen because the field moved, not because the
plugin is weaker.

---

## 🌍 Where the plugins live

- **GitHub** (this profile), **[Gitee](https://gitee.com/perrylink)** and **npm** — source, CI and releases here; 46
family repos mirrored to Gitee by a daily job (default branch + all tags), plus this profile repo; the `perrylink`
account holds **52 npm names and 951 versions**, 47 of them with a non-deprecated `latest` and **39 of those
carrying a SLSA provenance attestation on that version** (44 names carry it on at least one version; the eight with
none anywhere are `jevcore`, `jevcore-dsh`, `jevcore-mcp`, `dsh-laya`, `laya-mcp`, `dsh-personal-directive` and the
three archived `layacore` names — measured 2026-10-05 against each name's own packument, and the registry
**search** endpoint is not authoritative here, since it returns only 47 names and omits the deprecated ones)
- **npm downloads** — **152,643 over the trailing 30 days** (npm window 09-05..10-04, summed per name from the
downloads point endpoint; **[dshfind](https://dshfind.com/plugins?q=PerryLink)** independently tracks **22.5k+**
across the 8 family plugins it currently has a download figure for — dshfind reports rounded tiers, so that is a floor
rather than a total
- **DSH Desktop Market** — add the catalog source
`https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json` under Market → Sources to browse the family
in-app; **MCP Registry** — three servers, all published from their release workflows over GitHub OIDC: `dsh-cert-mcp`,
`jevcore-mcp` and `laya-mcp`
- **GitHub Actions** — [dsh-github](https://github.com/PerryLink/dsh-github) and
[dsh-test-drive](https://github.com/PerryLink/dsh-test-drive) also ship composite actions, so they install as `uses:
PerryLink/dsh-test-drive@vX`

Published to a dozen-plus third-party DSH directories and curated lists —
[awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin), [DSH
Directory](https://dsh.directory/plugins?q=perrylink), [Awesome DeepSeek
Harness](https://github.com/0xsline/awesome-deepseek-harness), [walkinglabs'
list](https://github.com/walkinglabs/awesome-deepseek-harness-plugins), [Zhiyuan-Fan's
list](https://github.com/Zhiyuan-Fan/Awesome-DeepSeek-Harness-Plugins), the [AdamPlatin123
radar](https://github.com/AdamPlatin123/dsh-plugin-radar), [dsh-suite](https://github.com/whyihaveyou/dsh-suite),
[dshfind.com](https://dshfind.com/zh/plugins/PerryLink/dsh-memento), [deepseek1024.com](https://deepseek1024.com) and
[Glama](https://glama.ai/mcp/servers/PerryLink/dsh-cert-mcp) among them — and scored on [OpenSSF
Scorecard](https://api.securityscorecards.dev/projects/github.com/PerryLink/dsh-auto-review); the GitHub [`dsh-plugin`
topic](https://github.com/topics/dsh-plugin) is what most of them ingest from.

<details>
<summary><b>中文介绍</b></summary>

**在 DeepSeek Harness 上构建插件生态:42 个开源插件,来自一个 48 仓的家族(其中 47 个由 PerryLink 自己维护)** —— 安全、工作流、研究、消息桥接、开发者体验,外加 DSH Desktop
Market 目录、插件认证注册表与 dsh-plugin-doctor 这个 CI 检查器。42 个插件全部带 CI、Gitee 镜像与五语文档,文档的段落数、安装命令、配置键由每个仓自己的 CI 闸门守着一致,并声明
`dsh.bundle` 契约。npm 账号、Gitee 镜像、DSH Desktop Market、MCP Registry 与 GitHub Actions 的入口见上节「Where the plugins
live」。**我也向上游 [Cordis](https://github.com/cordiverse/cordis)(DeepSeek Harness 所基于的插件内核框架)与
[deepseek-ai](https://github.com/deepseek-ai) 项目贡献:该组织下 20 条 PR 里,已合并的仍是
[FlashMLA](https://github.com/deepseek-ai/FlashMLA) 修复(#224,唯一一条),另有 16 条开放,其中 14 条是带复现的系统层修复。**

**本页所有实测数字只在英文部分维护一份**(外部仓与合并数、千星仓、npm 名称与下载、laya 台账),中文这里不复述,以免两处走样;需要数字请看上方的 Upstream 一节,那里每个数字都带测量日期。

**这一家子所依赖的那项研究,现在是一篇有 DOI 的论文 —— 而且它测的很大一部分,正是这份主页上的两个项目:[laya-mcp](https://github.com/PerryLink/laya-mcp) 与
[jevcore](https://github.com/PerryLink/jevcore)。**《[当判定层的自报字段说谎时:三类判断层的成本、延迟与失效边界实测](https://doi.org/10.5281/zenodo.22902025)》在一套相同条目上实测三类判定层(Laya、TypeSafe
Jev、DeepSeek-V4.1-Flash),四条主张**三条成立、一条被自己的数据否定**;判定器的接入层自报字段不可信(截断标志报「通过」却静默丢输入、概率字段把结论反号、两个判定词在真实输入下不可达),失效集中在一处 ——
答案被明确陈述时近乎完美(0.9909,n=220),必须注意到「缺席」时塌缩(0.3091,n=220);异种判定器在三个区制上都**没有**增量覆盖。**引其一即可,不要当两篇引**([英文原文](https://doi.org/10.5281/zenodo.22901853)
· [中文译本](https://doi.org/10.5281/zenodo.22902025) · [制品](https://doi.org/10.5281/zenodo.22901248));两者有出入以英文为准。

**laya**([NandhaKishorM/laya](https://github.com/NandhaKishorM/laya))是这个账号投入最深的外部项目:提了 **49 条 PR,其中 46
条已合并**,合并数在该仓**排第二**;45 条集中在 2026-09-21 至 09-29
这九天里合掉。逐条清单与九个方向见上方英文部分折叠块,或直接看[这个筛选列表](https://github.com/NandhaKishorM/laya/pulls?q=is%3Apr+author%3APerryLink)。

**还有一条在别处:一个根本起不来的进程现在能起来了。** [claude-agent-acp #1146](https://github.com/agentclientprotocol/claude-agent-acp/pull/1146) 让 `src/index.ts` 里那处没有保护的顶层 await 不再因一次瞬时错误就中断模块求值、在发出任何一条 ACP 消息之前退出。

待业中。十一准备出去玩一圈，所以更新迭代节奏可能短期内仍然提升的有限。当然，问题和缺陷修复不会停，只是发布频率会降低一些，还请大家谅解。

</details>

---

**This page is re-measured, not remembered.** Every figure carries the date it was measured, and the
round log records what each re-measurement corrected — including three claims of this page's own that
did not survive. [Round log](https://github.com/PerryLink/perrylink/blob/main/CHANGELOG.md) · [How every figure was measured](https://github.com/PerryLink/perrylink/blob/main/INSTRUMENTATION.md).