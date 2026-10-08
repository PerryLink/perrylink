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
<img alt="npm downloads 30d" src="https://img.shields.io/badge/npm%20downloads%2030d-183.9k-6e7781">
<a href="https://github.com/PerryLink/dsh-kit"><img alt="actively maintained plugins" src="https://img.shields.io/badge/plugins-33-6e7781"></a>
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
<a href="https://dshfind.com/plugins?q=PerryLink"><img alt="dshfind downloads across the family" src="https://img.shields.io/badge/dshfind%20downloads-38.5k%2B%20across%208%20plugins-6e7781"></a>
<a href="https://perrylink-dsh-catalog.perrylink.workers.dev/catalog-source.json"><img alt="DSH Desktop Market source" src="https://img.shields.io/badge/DSH%20Desktop%20Market-source-0969da"></a>
<a href="https://github.com/PerryLink/dsh-plugin-certification"><img alt="certified (flagship dsh-auto-review)" src="https://raw.githubusercontent.com/PerryLink/dsh-plugin-certification/main/badges/PerryLink__dsh-auto-review.svg"></a>
<a href="https://doi.org/10.5281/zenodo.22901853"><img alt="Zenodo DOI" src="https://zenodo.org/badge/DOI/10.5281/zenodo.22901853.svg"></a>
</p>

Open-source developer in Beijing. I build the
[DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness) plugin ecosystem: 33 actively
maintained Apache-2.0 plugins in a 48-repo family — security, workflows, research, messaging bridges
and developer experience — plus the DSH Desktop Market catalog, a plugin-certification registry and the
dsh-plugin-doctor CI checker. Every plugin ships CI, a Gitee mirror and five-language docs held to
the same section count by a gate in its own CI.

## 🦭 Phocinae — a 144M typed decision model

Separate from the harness: I train small language models. **[Phocinae-Largha-150M-v1](https://github.com/Phocinae/Phocinae-Largha-150M-v1)** (Apache-2.0) is a typed decision model — no text generation; one forward pass returns a verdict per question with calibrated confidence. GPU **18.6 ms** p50 per decision, CPU-only **~1.5 s**; English typed-decisions **0.797** (400 cases / 2,000 decisions, measured 2026-10-07), Chinese (machine-translated eval set) 0.789. With a τ=0.6 escalate gate, **82%** of agent decisions stay local and combined accuracy moves 0.789 → **0.7948** — the gate makes the system better, not just cheaper. Weights on [Hugging Face](https://huggingface.co/Phocinae/Phocinae-Largha-150M-v1) and [ModelScope](https://modelscope.cn/models/PerryLink/Phocinae-Largha-150M-v1); server `pip install phocinae-server`, DSH bundle `npm i dsh-phocinae`. Reproduction ships with the repo: seeds, row-set hashes, environment and eval scripts.

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
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | Approval-gated cross-session memory (`ctx.memory` + SQLite) (139★) · 🧊 **frozen** — better-adopted alternatives exist | `dsh plugin --profile web add dsh-memento` |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Claude Code-style declarative allow/deny/ask rules plus a process-level network policy (119★) | `dsh plugin --profile web add dsh-permission-rules` |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | MCP management console: `/mcp` + Settings tab + trial calls (73★) | `dsh plugin --profile web add dsh-mcp-panel` |

## 🔧 Upstream & community contributions

*Every repo below is external to `PerryLink/*`; every number is measured, merged work only, and open
proposals are deliberately not listed. The third column names the project's owner — the account alone
does not say whether that is a company, a standards body or one person.*

**★ 1,000+ — named individually, as the rule requires, each carrying the party that owns the project.**
Twenty-seven external repos above a thousand stars carry merged work (★ measured 2026-10-08), and the newest
of them is `NVIDIA/NeMo-Agent-Toolkit` — merged 2026-10-08T00:10:02Z by NVIDIA's `rapids-bot` after
maintainer `willkill07` issued `/merge`, and the first NVIDIA row this table has carried. It is the fourth
row to arrive by merge inside two days: before it `vllm-project/aibrix` merged 2026-10-07T11:18:42Z,
`bytedance/deer-flow` 2026-10-07T10:22:16Z and `apple/embedding-atlas` 2026-10-06T16:30:51Z, and before
those `Tencent/BrowserSkill` had held the position since 2026-10-06T13:45:15Z, `awslabs/mcp` for the
fifteen hours before that and `docker/docker-agent` for the ten before that; `ruvnet/ruflo` and
`walkinglabs/learn-harness-engineering` entered the ten days before those, and `punkpeye/fastmcp` has
carried its merge since 2026-09-24 and was missing from the round before.
Thirteen of those rows belong to a company or a well-known project organization — Amazon Web Services, Apple,
ByteDance, Docker, NVIDIA, Reactive Resume, DeepSeek, cordiverse, Tencent, the vLLM project, and the ACP
project that Zed and JetBrains jointly govern, the last two of which take two rows each; the other fourteen
are catalog repos, small community orgs and one-person projects, and the column says so rather than letting
the account name imply a company:

| Repository | ★ | 项目归属方 |
|---|---|---|
| [deer-flow](https://github.com/bytedance/deer-flow) | 83,475 | **字节跳动 ByteDance** — the official `bytedance` org (deerflow.tech); a one-line portability fix in a blocking-IO test merged 2026-10-07T10:22:16Z by `WillemJiang`, and now the largest row in this table |
| [ruflo](https://github.com/ruvnet/ruflo) | 74,072 | ruvnet (rUv / Reuven Cohen) — individual maintainer; a 74k★ agent harness on a personal account, not a company repo, and the largest row here that is not owned by a company |
| [reactive-resume](https://github.com/reactive-resume/reactive-resume) | 43,959 | `reactive-resume` org — independent open-source project (rxresu.me) |
| [laya](https://github.com/NandhaKishorM/laya) | 31,443 | NandhaKishorM — individual maintainer; the repo was created 2026-09-18 |
| [learn-harness-engineering](https://github.com/walkinglabs/learn-harness-engineering) | 19,474 | `walkinglabs` community org — the harness-engineering tutorial site |
| [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) | 18,009 | `awesome-dsh-plugin` org — community catalog, no company behind it |
| [FlashMLA](https://github.com/deepseek-ai/FlashMLA) | 13,042 | **DeepSeek** — the official `deepseek-ai` org |
| [mcp](https://github.com/awslabs/mcp) | 9,761 | **Amazon Web Services (AWS)** — the official `awslabs` org; a one-file UTF-8 fix merged 2026-10-05T22:49:06Z by maintainer `markjschreiber` with two approvals |
| [Cordis](https://github.com/cordiverse/cordis) | 9,053 | **cordiverse** org; its maintainer Shigma is now at **DeepSeek**, and Cordis is the kernel DeepSeek Harness vendors as `@deepseek-ai/cordis` |
| [dsh-web](https://github.com/zhu1090093659/dsh-web) | 8,482 | zhu1090093659 — individual maintainer |
| [BrowserSkill](https://github.com/Tencent/BrowserSkill) | 8,318 | **腾讯 Tencent** — the official `Tencent` org; merged 2026-10-06T13:45:15Z by collaborator `iuyo5678` with eight checks green |
| [ouroboros](https://github.com/Q00/ouroboros) | 6,193 | Q00 — individual maintainer (`@zep-us`) |
| [dsh-market](https://github.com/dsh-market/dsh-market) | 5,753 | `dsh-market` org — the community plugin market behind dshmarket.com, not a DeepSeek repo |
| [teamai-cli](https://github.com/Tencent/teamai-cli) | 5,141 | **腾讯 Tencent** — the official `Tencent` org, opensource.tencent.com |
| [aibrix](https://github.com/vllm-project/aibrix) | 5,127 | **the vLLM project** — the official `vllm-project` org behind vLLM; two flaky-test fixes merged 2026-10-06T16:23:08Z and 2026-10-07T11:18:42Z, the second by `googs1025` and the most recent merge this account has anywhere |
| [embedding-atlas](https://github.com/apple/embedding-atlas) | 4,972 | **Apple** — the official `apple` org (apple.github.io/embedding-atlas); a line-ending normalization fix in a release script merged 2026-10-06T16:30:51Z by `donghaoren` |
| [agent-client-protocol](https://github.com/agentclientprotocol/agent-client-protocol) | 4,388 | `agentclientprotocol` org — governed jointly by **Zed Industries** and **JetBrains** |
| [docker-agent](https://github.com/docker/docker-agent) | 3,700 | **Docker, Inc.** — the official `docker` org; merged 2026-10-05 by maintainer `aheritier` |
| [fastmcp](https://github.com/punkpeye/fastmcp) | 3,273 | punkpeye (Frank Fiegel) — individual maintainer at Glama; the TypeScript MCP framework |
| [deepseek-harness-desktop](https://github.com/dsh-tauri/deepseek-harness-desktop) | 3,079 | `dsh-tauri` community org — self-described non-official and non-commercial, not a DeepSeek repo |
| [NeMo-Agent-Toolkit](https://github.com/NVIDIA/NeMo-Agent-Toolkit) | 2,660 | **NVIDIA** — the official `NVIDIA` org; three review rounds with maintainer `willkill07` on making `remove_r1_think_tags` actually remove think blocks, merged 2026-10-08T00:10:02Z by NVIDIA's `rapids-bot` after he issued `/merge` |
| [claude-agent-acp](https://github.com/agentclientprotocol/claude-agent-acp) | 2,624 | `agentclientprotocol` org — the same jointly-governed org as the row above, a separate repository |
| [awesome-jev](https://github.com/yibie/awesome-jev) | 2,211 | yibie — individual maintainer, community catalog for Jev; the row the 09-25 round both printed and denied, kept now on the commit the history probe finds |
| [Agents-Anywhere](https://github.com/anywhere-labs/Agents-Anywhere) | 1,481 | `anywhere-labs` community org — 3 public repos, created 2026-05, dshdesktop.cn; not a company |
| [dsh-plugin-radar](https://github.com/AdamPlatin123/dsh-plugin-radar) | 1,465 | AdamPlatin123 — individual maintainer, catalog is a generated artifact |
| [awesome-deepseek-harness](https://github.com/0xsline/awesome-deepseek-harness) | 1,146 | 0xsline — individual maintainer, community catalog |
| [awesome-vibecoded-saas](https://github.com/Anil-matcha/awesome-vibecoded-saas) | 1,037 | Anil Chandra Naidu Matcha — individual maintainer, community catalog |

**The rest of the contributor set** is the community catalog layer rather than upstream projects:
**24 further repositories**, DSH plugin directories and small community projects
([dsh-handbook](https://github.com/Electricitysheep/dsh-handbook) and
[imsai-sh's list](https://github.com/imsai-sh/awesome-deepseek-harness-plugins), which alone took 41
merges, among them) — the catalogs ingest the family and carry no company owner, so they are named here
only in aggregate. **51 external repositories carry at least one merged pull request of ours together
with a commit attributed to this account, and 327 merges were counted inside them** — re-derived
2026-10-08 from this account's own merged pull requests, so 327 is exact rather than a floor over a
probed subset. Two further repositories took **33 more** of our merged pull requests **without**
crediting a commit to this account on their default branches —
[SihanTeng's list](https://github.com/SihanTeng/awesome-deepseek-harness-plugins), 32 of them, which is
the case the rule at the top of this section was written about, and
[dsh-better-sidebar](https://github.com/omdsh-dev/DSH-better-sidebar), one, which merged 2026-10-04 and
carries no commit of ours on `main` — so neither sizes the contributor set. 327 + 33 = the
**360 merged pull requests** this account has outside `PerryLink/*`, concentrated in **53 repositories**;
a further **101 are open across 64 repositories** and are deliberately not counted here.

**The round since the last derivation moved the merged count by 3, the credited set by two repositories and
the table by one row** — the previous derivation was dated 2026-10-07 and this one was taken about twelve
hours later. All three merges are upstream fixes.
[NeMo-Agent-Toolkit](https://github.com/NVIDIA/NeMo-Agent-Toolkit) merged
[#2293](https://github.com/NVIDIA/NeMo-Agent-Toolkit/pull/2293) on 2026-10-08T00:10:02Z and carries our
commit on `develop`, its default branch, so it is both the new row and the new most-recent merge.
[satori](https://github.com/satorijs/satori) took two — [#422](https://github.com/satorijs/satori/pull/422)
on 2026-10-07T14:55:26Z into `main`, which is what credits the repository, and
[#421](https://github.com/satorijs/satori/pull/421) on 2026-10-07T15:06:01Z into the `v4` branch, which is
**not** the default branch and therefore credits nothing by itself — so `satori` is named here on the merge
that reaches `main`, and #421 is counted in the merged total rather than being allowed to look like a second
credited repository. The most recent merge before this window remains
[aibrix#2931](https://github.com/vllm-project/aibrix/pull/2931), merged 2026-10-07T11:18:42Z.

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

The rest of the family and the five support repos are one line each below. The roster's source of truth
is **[dsh-kit](https://github.com/PerryLink/dsh-kit)** — its `plugins.txt` and a parity script hold the
family to that file; the machine-readable catalogue is
**[dsh-catalog](https://github.com/PerryLink/dsh-catalog)**, which is also the DSH Desktop Market source;
and each plugin's own README carries the detail this page only summarises.

<details>
<summary><b>The full family — 42 plugins in the roster, 33 of them actively maintained, plus 5 support repos, one line each</b></summary>

*Counting note: **33** is the actively maintained set, and it is the figure this page's heading and badge
use. It is derived one repository at a time: **42** repositories declare `dsh.bundle.patch` (re-derived
2026-10-07 by reading each repo's own `package.json` at its default branch), of which **3 are 🚫 retired**
and **6 are 🧊 frozen**, leaving **33 actively maintained**. Measured against the 47 PerryLink-owned
repositories this page names: **42 declare the contract and 5 do not** — the support trio
[dsh-catalog](https://github.com/PerryLink/dsh-catalog), [dsh-kit](https://github.com/PerryLink/dsh-kit) and
[dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification) (the certification registry, whose
MCP server publishes from [dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) instead), plus
[jevcore](https://github.com/PerryLink/jevcore) (no `dsh.bundle`; only its `jevcore-dsh` workspace member is a plugin)
and [laya-mcp](https://github.com/PerryLink/laya-mcp) (an MCP sidecar, not a plugin). The third-party
[pan17/dsh-wechat](https://github.com/pan17/dsh-wechat) carries a plugin row but is not one of them: 47 + 1 = the 48
repos this page names. A naive scan of the account finds two more than the 42 — the retired
[dsh-plugin-upgrade](https://github.com/PerryLink/dsh-plugin-upgrade) corridor legs `dsh-plugin-upgrade-015` (**not**
archived) and `dsh-plugin-upgrade-016` (archived), both still carrying the manifest and neither an active plugin:
42 + 2 = the **44** such a scan returns. The nine tables below list **41 rows**: 39 of the 42 roster repositories,
plus `jevcore` (which declares no `dsh.bundle`) and the third-party `dsh-wechat` — the three left out
(`dsh-plugin-kit`, `dsh-cert-mcp`, `dsh-plugin-doctor`) are the toolchain repositories named in the support
list above. Retired and frozen rows keep their place with
their status rather than being deleted, which is why the roster figure is larger than the active one. The same
42 repositories and the same three states are recorded once, in
[dsh-plugin-kit/data/repos.json](https://github.com/PerryLink/dsh-plugin-kit/blob/master/data/repos.json), which
the portal renders and the certification registry counts.*

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
holds **52 npm names** — more names than the family has repositories, because several repos publish both a plugin
and a provider package (measured 2026-10-04).

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

Frozen because **better-adopted alternatives now exist** for that capability. Six of the seven carry a
`## Maintenance status: 🧊 FROZEN` section in their own README with the measured comparison —
[dsh-wechat](https://github.com/pan17/dsh-wechat) is the exception, because it is `pan17`'s repository rather than
this account's, so the banner cannot be added there and the row is frozen here instead. Weekly npm downloads,
measured 2026-10-05:

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
account holds **52 npm names and 1,069 versions**, 44 of them with a non-deprecated `latest` and **39 of those
carrying a SLSA provenance attestation on that version** (45 names carry it on at least one version; the seven with
none anywhere are `jevcore-dsh`, `jevcore-mcp`, `dsh-laya`, `laya-mcp` and the three archived `layacore` names —
measured 2026-10-07 against each name's own packument, and the registry
**search** endpoint is not authoritative here, since it returns only 47 names and omits the deprecated ones)
- **npm downloads** — **183,886 over the trailing 30 days** (npm window 09-07..10-06, summed per name from the
downloads point endpoint; **[dshfind](https://dshfind.com/plugins?q=PerryLink)** independently tracks **38.5k+**
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

**在 DeepSeek Harness 上构建插件生态:33 个活跃维护的开源插件,来自一个 48 仓的家族(其中 47 个由 PerryLink 自己维护)** —— 安全、工作流、研究、消息桥接、开发者体验,外加 DSH Desktop
Market 目录、插件认证注册表与 dsh-plugin-doctor 这个 CI 检查器。33 个插件全部带 CI、Gitee 镜像与五语文档,文档的段落数、安装命令、配置键由每个仓自己的 CI 闸门守着一致,并声明
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

**斑海豹 Phocinae-Largha-150M-v1**
([Phocinae org](https://github.com/Phocinae/Phocinae-Largha-150M-v1),Apache-2.0)是插件生态之外的另一条线:一个 144.3M
参数的结构化决策模型,不生成文本,一次前向输出判定与校准置信度;GPU 单次判定 p50
**18.6ms**、纯 CPU 约 **1.5s**,英文 typed-decisions **0.797**(400 用例 / 2000 决策,2026-10-07
实测),中文(机译评测集)**0.789**;τ=0.6 升级门让 **82%** 的 agent 决策留在本地、组合准确率
0.789→**0.7948**。权重在 [Hugging
Face](https://huggingface.co/Phocinae/Phocinae-Largha-150M-v1) 与[魔搭](https://modelscope.cn/models/PerryLink/Phocinae-Largha-150M-v1),配套 `pip install phocinae-server` 与 `npm i dsh-phocinae`;复现四件套(seed/行集/环境/脚本)随仓库发货。


</details>

---

**This page is re-measured, not remembered.** Every figure carries the date it was measured, and the
round log records what each re-measurement corrected — including three claims of this page's own that
did not survive. [Round log](https://github.com/PerryLink/perrylink/blob/main/CHANGELOG.md) · [How every figure was measured](https://github.com/PerryLink/perrylink/blob/main/INSTRUMENTATION.md).
