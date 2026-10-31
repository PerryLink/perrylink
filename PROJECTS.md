# Projects, contributions and the family — the measured inventory

> This is the long form of [the profile README](README.md). The profile carries the front page: who I
> am, the flagship plugins, every external repository above 2,500★, and a short note on what is retired
> and frozen. Everything that used to sit there in full lives here — the merge-by-merge upstream
> record, the whole 105-row plugin roster, the retired and frozen tables, and the npm/Gitee/Market
> figures with their caveats.
>
> Moved out of the profile on 2026-10-19; every figure keeps the date it was measured. How each one is
> measured is in
> [INSTRUMENTATION.md](https://github.com/PerryLink/perrylink/blob/main/INSTRUMENTATION.md), and what
> each round corrected is in [CHANGELOG.md](https://github.com/PerryLink/perrylink/blob/main/CHANGELOG.md).

## 🔧 Upstream & community contributions — the full record

*Every repo below is external to `PerryLink/*`; every number is measured, merged work only, and open
proposals are deliberately not listed. The third column names the project's owner — the account alone
does not say whether that is a company, a standards body or one person.*

**★ 1,000+ — named individually, as the rule requires, each carrying the party that owns the project.**
Fifty-one external repositories above a thousand stars carry merged work — forty-five above 2,500★ in the
table below and six between 1,000★ and 2,500★ in the folded table after it. Every ★ was re-measured
2026-10-31. Some rows belong to a company or a well-known project organization — Amazon Web Services, Apple,
ByteDance, Docker, Microsoft, NVIDIA, Redis, Tencent, DeepSeek, ModelScope, the vLLM project, the `gofiber`
project, cordiverse, koishijs, NeuML's `txtai`, and the ACP project that Zed and JetBrains jointly govern —
while the rest are catalog repos, small community orgs and one-person projects, and the column says so rather
than letting the account name imply a company.

| Repository | ★ | 项目归属方 |
|---|---|---|
| [dify](https://github.com/langgenius/dify) | 160,042 | **LangGenius** — the official `langgenius` org; the open-source LLM application platform (dify.ai); `download_with_size_limit` returned the 4xx/5xx error page as the downloaded plugin, so an installation reported an invalid package — it now rejects non-2xx responses, merged 2026-10-30T17:55:46Z by `Stream29` |
| [deer-flow](https://github.com/bytedance/deer-flow) | 84,743 | **字节跳动 ByteDance** — the official `bytedance` org (deerflow.tech); a one-line portability fix in a blocking-IO test merged 2026-10-07T10:22:16Z by `WillemJiang`, and now the largest row in this table |
| [ruflo](https://github.com/ruvnet/ruflo) | 80,322 | ruvnet (rUv / Reuven Cohen) — individual maintainer; a 75k★ agent harness on a personal account, not a company repo, and the largest row here that is not owned by a company |
| [reactive-resume](https://github.com/reactive-resume/reactive-resume) | 45,110 | `reactive-resume` org — independent open-source project (rxresu.me) |
| [black](https://github.com/psf/black) | 42,083 | **Python Software Foundation** — the official `psf` org; `_write_to_stdout()` translated `\n` itself, so the trailing-newline fixup appended a second one, and CRLF input without a trailing newline could come out as `\r\r\n`; it now appends a bare `\n` and lets the writer translate it, merged 2026-10-20T23:06:23Z by `cobaltt7` |
| [zoxide](https://github.com/ajeetdsouza/zoxide) | 40,375 | ajeetdsouza (Ajeet D'Souza) — individual maintainer; a bare `z` under `_ZO_ECHO=1` called `Set-Location` without `-Passthru`, so the `$dir` assignment was `$null` and strict mode threw `PropertyNotFoundException`; the no-path branch now passes `-Passthru`, merged 2026-10-22T23:55:13Z by `ajeetdsouza`, who dropped the regression test from the branch before merging |
| [fiber](https://github.com/gofiber/fiber) | 40,235 | **the gofiber project** — the official `gofiber` org (gofiber.io), the Express-inspired Go web framework; an optional-path-parameter matching fix merged 2026-10-19T08:56:41Z by `ReneWerner87` |
| [laya](https://github.com/NandhaKishorM/laya) | 34,717 | NandhaKishorM — individual maintainer; the repo was created 2026-09-18 |
| [cli](https://github.com/urfave/cli) | 24,306 | the `urfave` org — community-maintained Go CLI framework; `HandleExitCoder` recognised an `ExitCoder` only through a bare type assertion, so an exit error wrapped with `fmt.Errorf("%w")` printed nothing and fell back to exit code 1; `Juneezee` rebased it onto a `main` that now requires Go 1.26 before merging on 2026-10-21T15:40:14Z |
| [learn-harness-engineering](https://github.com/walkinglabs/learn-harness-engineering) | 22,603 | `walkinglabs` community org — the harness-engineering tutorial site |
| [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) | 21,660 | `awesome-dsh-plugin` org — community catalog, no company behind it |
| [SkillOpt](https://github.com/microsoft/SkillOpt) | 18,785 | **Microsoft** — the official `microsoft` org; a UTF-8 state-file fix merged 2026-10-18T17:02:48Z |
| [MMKV](https://github.com/Tencent/MMKV) | 18,768 | **Tencent** — the official `Tencent` org; the mobile key-value storage framework developed by WeChat. A Win32 creation-flag fix merged 2026-10-19T10:35:44Z into `dev` by `lingol` — into `dev`, not the default branch `master`, which is why this row carries a merge and no credit |
| [ioredis](https://github.com/redis/ioredis) | 15,351 | **Redis** — the official `redis` org; the Node.js Redis client, where an auto-pipelining fix merged 2026-10-19T08:09:05Z by `PavelPashov` |
| [FlashMLA](https://github.com/deepseek-ai/FlashMLA) | 13,224 | **DeepSeek** — the official `deepseek-ai` org |
| [txtai](https://github.com/neuml/txtai) | 13,049 | **NeuML** — an independent open-source project (neuml.github.io/txtai), not a company repo; merged 2026-10-11T21:21:02Z by its maintainer `davidmezzetti`, on the third attempt and after he had asked repeatedly, over three pull requests, for the change to be cut down, which it was |
| [dsh-market](https://github.com/dsh-market/dsh-market) | 9,869 | `dsh-market` org — the community plugin market behind dshmarket.com, not a DeepSeek repo |
| [mcp](https://github.com/awslabs/mcp) | 9,853 | **Amazon Web Services (AWS)** — the official `awslabs` org; a one-file UTF-8 fix merged 2026-10-05T22:49:06Z by maintainer `markjschreiber` with two approvals |
| [dsh-web](https://github.com/zhu1090093659/dsh-web) | 9,852 | zhu1090093659 — individual maintainer |
| [BrowserSkill](https://github.com/Tencent/BrowserSkill) | 9,830 | **腾讯 Tencent** — the official `Tencent` org; merged 2026-10-06T13:45:15Z by collaborator `iuyo5678` with eight checks green |
| [Cordis](https://github.com/cordiverse/cordis) | 9,492 | **cordiverse** org; its maintainer Shigma is now at **DeepSeek**, and Cordis is the kernel DeepSeek Harness vendors as `@deepseek-ai/cordis` |
| [jc](https://github.com/kellyjonbrazil/jc) | 8,697 | kellyjonbrazil (Kelly Brazil) — individual maintainer; a Windows platform-name fix merged 2026-10-17T21:51:22Z and started counting when `master` caught up on 2026-10-18T20:39:02Z |
| [models.dev](https://github.com/anomalyco/models.dev) | 7,457 | `anomalyco` org — the model-catalogue site behind models.dev; merged 2026-10-10T23:11:09Z by `rekram1-node` |
| [kraken](https://github.com/uber/kraken) | 6,774 | **Uber** — the official `uber` org; the cache file reader opened to duplicate a committed upload to a replica was never closed, leaking one file descriptor per replica for every uploaded blob; both replication paths now register it with the server's closer set, merged 2026-10-22T09:31:25Z by `gkeesh7` |
| [koishi](https://github.com/koishijs/koishi) | 6,305 | `koishijs` org — the cross-platform chatbot framework; merged 2026-10-08T12:13:06Z by its maintainer `shigma`, who found and fixed a regression in this account's own patch before merging it |
| [ouroboros](https://github.com/Q00/ouroboros) | 6,291 | Q00 — individual maintainer (`@zep-us`) |
| [client_golang](https://github.com/prometheus/client_golang) | 6,043 | **Prometheus** — the official `prometheus` org (CNCF project); `checkMetricConsistency` compared each label name with the previous one before the pairs were sorted, so non-adjacent duplicates passed and a scrape of the registry was dropped as a whole; the sort now runs before the duplicate loop, merged 2026-10-23T07:22:07Z by `bwplotka` |
| [teamai-cli](https://github.com/Tencent/teamai-cli) | 5,718 | **腾讯 Tencent** — the official `Tencent` org, opensource.tencent.com |
| [go-sdk](https://github.com/modelcontextprotocol/go-sdk) | 5,290 | the `modelcontextprotocol` org's Go SDK for MCP |
| [aibrix](https://github.com/vllm-project/aibrix) | 5,169 | **the vLLM project** — the official `vllm-project` org behind vLLM; two flaky-test fixes merged 2026-10-06T16:23:08Z and 2026-10-07T11:18:42Z, the second by `googs1025` and the second of the two flaky-test fixes this account has merged there |
| [embedding-atlas](https://github.com/apple/embedding-atlas) | 5,005 | **Apple** — the official `apple` org (apple.github.io/embedding-atlas); a line-ending normalization fix in a release script merged 2026-10-06T16:30:51Z by `donghaoren` |
| [DSH-better-sidebar](https://github.com/omdsh-dev/DSH-better-sidebar) | 4,762 | `omdsh-dev` community org — the DeepSeek Harness sidebar plugin; added 2026-10-12, and `INSTRUMENTATION.md` records why it was previously carried as excluded |
| [docker-agent](https://github.com/docker/docker-agent) | 4,623 | **Docker, Inc.** — the official `docker` org; merged 2026-10-05 by maintainer `aheritier` |
| [agent-client-protocol](https://github.com/agentclientprotocol/agent-client-protocol) | 4,549 | `agentclientprotocol` org — governed jointly by **Zed Industries** and **JetBrains** |
| [client_python](https://github.com/prometheus/client_python) | 4,385 | **Prometheus** — the official `prometheus` org (CNCF project); the Python instrumentation client; the process collector failed the whole collection when `/proc/<pid>/limits` had no `Max open files` line — it now bounds-checks that line, merged 2026-10-30T18:39:55Z by `csmarchbanks` |
| [content](https://github.com/nuxt/content) | 3,676 | **Nuxt** — the official `nuxt` org. `generateItemSurround` dropped the previous item whenever `before` was larger than the item's index, instead of returning a shorter window; approved and merged 2026-10-19T12:27:29Z by `farnabaz` |
| [evalscope](https://github.com/modelscope/evalscope) | 3,618 | `modelscope` org — the ModelScope model-hub project; a UTF-8 BOM dataset fix merged 2026-10-19T03:42:50Z by `Yunnglin` |
| [deepseek-harness-desktop](https://github.com/dsh-tauri/deepseek-harness-desktop) | 3,379 | `dsh-tauri` community org — self-described non-official and non-commercial, not a DeepSeek repo |
| [fastmcp](https://github.com/punkpeye/fastmcp) | 3,284 | punkpeye (Frank Fiegel) — individual maintainer at Glama; the TypeScript MCP framework |
| [minio-go](https://github.com/minio/minio-go) | 3,010 | **MinIO** — the official `minio` org; `RemoveObjects` reported a single error for a whole batch, hiding which object had failed; it now reports one result per failed object, merged 2026-10-19T15:01:25Z by `klauspost` |
| [open5gs](https://github.com/open5gs/open5gs) | 2,799 | the `open5gs` open-source 5G core project — a community project rather than a company repo |
| [claude-agent-acp](https://github.com/agentclientprotocol/claude-agent-acp) | 2,710 | `agentclientprotocol` org — the same jointly-governed org as the row above, a separate repository |
| [NeMo-Agent-Toolkit](https://github.com/NVIDIA/NeMo-Agent-Toolkit) | 2,688 | **NVIDIA** — the official `NVIDIA` org; three review rounds with maintainer `willkill07` on making `remove_r1_think_tags` actually remove think blocks, merged 2026-10-08T00:10:02Z by NVIDIA's `rapids-bot` after he issued `/merge` |
| [Agents-Anywhere](https://github.com/anywhere-labs/Agents-Anywhere) | 2,531 | `anywhere-labs` community org — 3 public repos, created 2026-05, dshdesktop.cn; not a company |
| [awesome-jev](https://github.com/yibie/awesome-jev) | 2,513 | yibie — individual maintainer, community catalog for Jev; the row the 09-25 round both printed and denied, kept now on the commit the history probe finds |

<details>
<summary><b>Six more repositories between 1,000★ and 2,500★ — one line each</b></summary>

| Repository | ★ | 项目归属方 |
|---|---|---|
| [deep-research-web-ui](https://github.com/AnotiaWang/deep-research-web-ui) | 2,224 | AnotiaWang — individual maintainer; a docs fix to the Helodata image name merged 2026-10-26T09:22:58Z |
| [nginx-upsync-module](https://github.com/weibocom/nginx-upsync-module) | 1,844 | weibocom — the Weibo open-source org; an out-of-bounds write fix merged 2026-10-19T06:04:29Z, re-tested by the maintainer with a plain and an ASan build |
| [mcp-remote](https://github.com/punkpeye/mcp-remote) | 1,659 | punkpeye (Frank Fiegel) — individual maintainer at Glama, the same account as `fastmcp` above; a Windows-portability fix to the repository's own test harness merged 2026-10-17T21:06:55Z |
| [dsh-plugin-radar](https://github.com/AdamPlatin123/dsh-plugin-radar) | 1,488 | AdamPlatin123 — individual maintainer, catalog is a generated artifact |
| [awesome-deepseek-harness](https://github.com/0xsline/awesome-deepseek-harness) | 1,286 | 0xsline — individual maintainer, community catalog |
| [awesome-agent-apis](https://github.com/Anil-matcha/awesome-agent-apis) | 1,065 | Anil Chandra Naidu Matcha — individual maintainer, community catalog |

</details>

<details>
<summary><b>The rest of the contributor set, and how the 490 total is derived</b></summary>

**The rest of the contributor set** is the long tail below the 1,000★ line:
**43 further repositories**, DSH plugin directories, small upstream projects and community catalogs
([dsh-handbook](https://github.com/Electricitysheep/dsh-handbook),
[imsai-sh's list](https://github.com/imsai-sh/awesome-deepseek-harness-plugins), which alone took 44
merges, [the Jev gallery](https://github.com/OmniJev/awesome-jev-gallery) and
[the free5GC IKE daemon](https://github.com/free5gc/ike) and
[inference-gateway](https://github.com/inference-gateway/inference-gateway), among them) — most are
catalogs that ingest the family and carry no company owner, so they are named here only in aggregate.
**93 external repositories carry at least one merged pull request of ours and a commit
attributed to this account on their default branch; 456 merges were counted inside those 94 —
re-derived 2026-10-31T03:58:00Z from this account's own merged pull requests and confirmed repository by
repository with the `defaultBranchRef.target.history(author:{id})` probe, so 453 is exact rather than a
floor over a probed subset. Three repositories carry merges of ours and still earn no credit, and all are named for that reason:
[SihanTeng's list](https://github.com/SihanTeng/awesome-deepseek-harness-plugins), which took **32** and
credits no commit to this account at all — the case the rule at the top of this section was written
about — and [Tencent/MMKV](https://github.com/Tencent/MMKV), which took **1**, merged into `dev` rather than
into the default branch `master`, so no commit of this account sits where the probe looks; and [open-genjutsu](https://github.com/Anil-matcha/open-genjutsu), which took **1** in #63 but whose `main` now holds only the initial commit, so nothing of this account survives there. Two further repositories,
[phocinae-server](https://github.com/Phocinae/phocinae-server) and
[deepseek-desktop](https://github.com/zcx960/deepseek-desktop), each hold a commit of this account and no
merged pull request at all, so neither carries a merge and they are named only for that reason.
**456 + 34 = the 490 merged pull requests** this account has outside `PerryLink/*`, concentrated in
**96 repositories**; a further **155 are open across 122 repositories** as of 2026-10-31T12:40:00Z and are
deliberately not counted here.

</details>

Each re-derivation, the merges that arrived between them, the two repositories that changed sides and
the pull request this account closed after upstream fixed the same thing are recorded round by round in
[`CHANGELOG.md`](CHANGELOG.md); this page carries the current figures and none of that history.

<details>
<summary><b>laya — 47 merged pull requests, second of 146 merged-PR authors</b></summary>

**laya** — [NandhaKishorM/laya](https://github.com/NandhaKishorM/laya) — **47 merged pull requests of
the 51 this account has opened there** (re-measured 2026-10-14 over all 964 pull requests the repository
has ever had) and **second of 146 merged-PR authors**, behind `aashish254` (240) and ahead of `keemsisi`
(44) and `Bruce-Yii` (40); the maintainer NandhaKishorM holds one merged PR of his own because he
commits to `main` directly rather than through pull requests, and none of the three leaders is a
collaborator. As of 2026-10-14 it reads **0 open and 4 closed unmerged**; 45 of the 47 merged inside a
nine-day run (2026-09-21 → 2026-09-29), and the maintainer merges in batches — fifteen of them share two
timestamps, seven at `19:29:05` on 09-27 and eight at `17:40:36` on 09-29, and the two since are
[#924](https://github.com/NandhaKishorM/laya/pull/924) on 2026-10-04 and
[#1179](https://github.com/NandhaKishorM/laya/pull/1179) on 2026-10-14. The complete list is one
query away:

[`laya` pull requests by this account](https://github.com/NandhaKishorM/laya/pulls?q=is%3Apr+author%3APerryLink)
— the same 51, always current, in any language.

</details>

<details>
<summary><b>The 47 merged pull requests, by area</b></summary>

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

Four closures, and the reason is on the record for each:
[#370](https://github.com/NandhaKishorM/laya/pull/370), closed by this account as a duplicate of
[#362](https://github.com/NandhaKishorM/laya/pull/362), which opened the same fix four minutes earlier;
[#416](https://github.com/NandhaKishorM/laya/pull/416), the Routing guide, closed by the maintainer in
favour of another contributor's [#461](https://github.com/NandhaKishorM/laya/pull/461) so the project
would not carry two routing pages; and [#925](https://github.com/NandhaKishorM/laya/pull/925), closed
unmerged at 2026-10-04T17:54:52Z, four minutes after [#924](https://github.com/NandhaKishorM/laya/pull/924)
merged; and [#943](https://github.com/NandhaKishorM/laya/pull/943), closed unmerged at
2026-10-05T17:28:15Z in favour of [#936](https://github.com/NandhaKishorM/laya/pull/936), which had
landed the same two lines six minutes earlier and additionally forwards `hooksRaise` into the
`routeBatch` call, so a per-call `hooksRaise: false` reaches `onRoute` as well as each request's
predict lifecycle — the maintainer's note says explicitly that it was not closed for being wrong.

</details>

**Security** — published advisory [GHSA-j922-p6h6-p255](https://github.com/PerryLink/dsh-permission-rules/security/advisories/GHSA-j922-p6h6-p255) for dsh-permission-rules (medium, patched in 0.6.16).

<details>
<summary><b><code>deepseek-ai</code> — 22 pull requests opened across the org, 1 merged, 15 open</b></summary>

**Official harness repo** — it does not accept external pull requests, so that line runs through issues, Discussions
(the Show Your Plugins! post [#6104](https://github.com/deepseek-ai/deepseek-harness/discussions/6104)) and the plugin
ecosystem instead — while the wider `deepseek-ai` org is open to fixes, and the account now proposes them at the
systems layer rather than only in its catalogs: of the **22 pull requests it has opened across that org, FlashMLA
[#224](https://github.com/deepseek-ai/FlashMLA/pull/224) remains the only one merged**, and **15 are open**
across eleven repositories — [TileKernels](https://github.com/deepseek-ai/TileKernels) three,
[DeepEP](https://github.com/deepseek-ai/DeepEP) and
[deepseek-recipe](https://github.com/deepseek-ai/deepseek-recipe) two each, and one apiece in
[FlashMLA](https://github.com/deepseek-ai/FlashMLA),
[DeepGEMM](https://github.com/deepseek-ai/DeepGEMM), [3FS](https://github.com/deepseek-ai/3FS),
[DeepSeek-MoE](https://github.com/deepseek-ai/DeepSeek-MoE),
[DeepSeek-Prover-V1.5](https://github.com/deepseek-ai/DeepSeek-Prover-V1.5),
[DeepJIT](https://github.com/deepseek-ai/DeepJIT) and [DeepSelect](https://github.com/deepseek-ai/DeepSelect) —
fourteen of them code fixes, and the fifteenth a catalog addition.

</details>

## 📦 The family — the full roster

The rest of the family and the support repositories are one line each below. The install list is
**[dsh-kit](https://github.com/PerryLink/dsh-kit)** — its `plugins.txt` and a parity script hold the
published specs — and the machine-readable catalogue is
**[dsh-catalog](https://github.com/PerryLink/dsh-catalog)**, which is also the DSH Desktop Market source;
and each plugin's own README carries the detail this page only summarises.

<details>
<summary><b>The full family — 108 repositories in the roster, 100 of them actively maintained, plus the support repositories, one line each</b></summary>

*Counting note: **100** is the actively maintained set, and it is the figure this page's heading and badge
use. It is derived one repository at a time: **110** repositories declare `dsh.bundle.patch` (re-derived
2026-10-26 by reading each repo's own `package.json` at its default branch); removing the two retired
corridor legs leaves **108** in the roster, of which **3 are 🚫 retired** and **5 are 🧊 frozen**, leaving
**100 actively maintained**. The account owns **175** non-fork repositories; **121** carry a `package.json`
and **110** of those declare the contract. The ten categories below list **105 rows**: 103 of the 108 roster
repositories, plus `jevcore` (which declares no `dsh.bundle`) and the third-party `dsh-wechat`. The five
roster repositories left out — `dsh-plugin-kit`, `dsh-cert-mcp`, `dsh-plugin-doctor`, `dsh-checkers` and
`dsh-community-bench` — are the support and tooling repositories named above. Retired and frozen rows keep
their place with their status rather than being deleted, which is why the roster figure is larger than the
active one. The portal's
[dsh-plugin-kit/data/repos.json](https://github.com/PerryLink/dsh-plugin-kit/blob/main/data/repos.json)
still records the 2026-10-19 cut of 99 with the same three states; the nine 2026-10-23 tools are not in it
yet.*

**The 2026-10-08 addition.** 53 compliance checkers joined the roster that day — they declare
`dsh.bundle.patch` like every other entry, so by the rule above they count. They are the `### ✅ Compliance checkers & tools` tables at the end of the folded family below, and they keep
their own memory file and maintenance rules in a separate workspace. Every figure in this note was raised by exactly 53 except the
non-plugin total, which is measured rather than derived.

**The 2026-10-23 addition.** Nine more compliance tools were published — six checker packages
(`dsh-bid-health-check`, `dsh-canteen-retention-check`, `dsh-construction-doc-check`, `dsh-invoice-ledger`,
`dsh-payroll-audit`, `dsh-safety-ledger-check`) and three document tools (`dsh-excel-reconcile`,
`dsh-table-ingest`, `dsh-tender-requirements`). They are roster entries under the same rule, but they are not
part of the 53-checker suite and are listed in the toolchain table below. The roster moved 99 → 108 and the
active count 91 → 100; the 53-checker suite itself is unchanged.

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
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | Approval-gated cross-session memory protocol | | [npm](https://www.npmjs.com/package/dsh-memento) |

### 🧪 Evaluation (3)

| Plugin | One-liner | Status | npm |
|---|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | Second-model auto-review on the approval chain | | [npm](https://www.npmjs.com/package/dsh-auto-review) |
| [dsh-doublecheck](https://github.com/PerryLink/dsh-doublecheck) | Engineering-discipline guard: grill, gates, adversary review | | [npm](https://www.npmjs.com/package/dsh-doublecheck) |
| [dsh-score](https://github.com/PerryLink/dsh-score) | Plugin quality scoring across git/gh/npm | | [npm](https://www.npmjs.com/package/dsh-score) |

### 📊 Observability & cost (5)

| Plugin | One-liner | Status | npm |
|---|---|---|---|
| [dsh-autotier](https://github.com/PerryLink/dsh-autotier) | Automatic strong/cheap model-tier routing with deterministic risk guards | | [npm](https://www.npmjs.com/package/dsh-autotier) |
| [dsh-budget](https://github.com/PerryLink/dsh-budget) | Token/cost metering, budget caps, carbon estimate, latency benchmarks | 🧊 FROZEN — `dsh-cost-meter` | [npm](https://www.npmjs.com/package/dsh-budget) |
| [dsh-observe](https://github.com/PerryLink/dsh-observe) | OTel/Langfuse telemetry export | | [npm](https://www.npmjs.com/package/dsh-observe) |
| [dsh-fast](https://github.com/PerryLink/dsh-fast) | Performance diagnostics | | [npm](https://www.npmjs.com/package/dsh-fast) |
| [dsh-phocinae](https://github.com/PerryLink/dsh-phocinae) | Local non-generative decision layer: `phocinae_ask` / `phocinae_gate` on a typed decision model, plus a fail-closed approval gate | | [npm](https://www.npmjs.com/package/dsh-phocinae) |

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
holds **110 npm names** — more names than the family has repositories, because several repos publish both a plugin
and a provider package, and because the 53 compliance checkers and the two `Phocinae` packages publish under names
of their own (measured 2026-10-14).

### 📱 Messaging & bridges (4)

| Plugin | One-liner | Status | npm |
|---|---|---|---|
| [dsh-phone-inbox](https://github.com/PerryLink/dsh-phone-inbox) | Inbound phone (WeChat bridge) attachment inbox: list what this conversation actually received and adopt one into the workspace on demand | | [npm](https://www.npmjs.com/package/dsh-phone-inbox) |
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


### ✅ Compliance checkers & tools (62)

Fifty-three checkers published 2026-10-08, all Apache-2.0, all carrying SLSA provenance on npm; nine further
compliance tools followed on 2026-10-23 (the toolchain table at the end of this section).
Each reads one register, ledger or record set against a **versioned rule pack** and returns the differences
for a human to review — none of them pronounces on compliance, liability or clinical correctness. A
per-repo `check:citations` gate holds each quotation to its own `rules/evidence/` record, and the rule
packs state how many of their rules have **no verbatim clause text obtained** rather than paraphrasing the
clause — the per-domain counts are on the [checker index](https://perrylink.github.io/zh/checkers/).


#### 🧾 Tendering & procurement (7)

| Plugin | One-liner | Status | npm |
|---|---|---|---|
| [dsh-bid-ca-precheck](https://github.com/PerryLink/dsh-bid-ca-precheck) | Pre-flight check of a bid package against the responsiveness and qualification clauses before submission | | [npm](https://www.npmjs.com/package/dsh-bid-ca-precheck) |
| [dsh-bid-qual-check](https://github.com/PerryLink/dsh-bid-qual-check) | Qualification screening: does the bidder's evidence actually answer every qualification the documents demand | | [npm](https://www.npmjs.com/package/dsh-bid-qual-check) |
| [dsh-tender-extract](https://github.com/PerryLink/dsh-tender-extract) | Pulls the substantive requirements out of tender documents so nothing mandatory is missed | | [npm](https://www.npmjs.com/package/dsh-tender-extract) |
| [dsh-tender-matrix](https://github.com/PerryLink/dsh-tender-matrix) | Scoring-matrix arithmetic: weights, caps and totals reconciled against the stated evaluation method | | [npm](https://www.npmjs.com/package/dsh-tender-matrix) |
| [dsh-protest-deadline](https://github.com/PerryLink/dsh-protest-deadline) | Challenge-deadline arithmetic under the procurement regime, with the clause behind each period | | [npm](https://www.npmjs.com/package/dsh-protest-deadline) |
| [dsh-contract-stance](https://github.com/PerryLink/dsh-contract-stance) | Reads a contract for the positions it actually takes, clause by clause, and reports them without advising | | [npm](https://www.npmjs.com/package/dsh-contract-stance) |
| [dsh-rulefile-check](https://github.com/PerryLink/dsh-rulefile-check) | Internal rule-file consistency: no contradictions, no dangling references, no undefined terms | | [npm](https://www.npmjs.com/package/dsh-rulefile-check) |

#### 🏗️ Construction & environment (7)

| Plugin | One-liner | Status | npm |
|---|---|---|---|
| [dsh-site-log-check](https://github.com/PerryLink/dsh-site-log-check) | Supervision-log completeness against the supervision standard and the on-site recording rules | | [npm](https://www.npmjs.com/package/dsh-site-log-check) |
| [dsh-hazplan-check](https://github.com/PerryLink/dsh-hazplan-check) | HAZOP worksheet review: nodes, guide words, deviations and actions held to the analysis standard | | [npm](https://www.npmjs.com/package/dsh-hazplan-check) |
| [dsh-safety-brief-check](https://github.com/PerryLink/dsh-safety-brief-check) | Safety-briefing records checked for the required topics and the sign-off each one needs | | [npm](https://www.npmjs.com/package/dsh-safety-brief-check) |
| [dsh-guard-plan-qc](https://github.com/PerryLink/dsh-guard-plan-qc) | Guard-plan quality: coverage, escalation paths and the shifts the plan claims to cover | | [npm](https://www.npmjs.com/package/dsh-guard-plan-qc) |
| [dsh-soilwater-check](https://github.com/PerryLink/dsh-soilwater-check) | Soil and groundwater survey records — sampling points, analytes and the reported units | | [npm](https://www.npmjs.com/package/dsh-soilwater-check) |
| [dsh-eia-guide-check](https://github.com/PerryLink/dsh-eia-guide-check) | Environmental impact assessment against the published technical guidelines | | [npm](https://www.npmjs.com/package/dsh-eia-guide-check) |
| [dsh-permit-report-check](https://github.com/PerryLink/dsh-permit-report-check) | Permit application reports: the sections required, and whether each is filled rather than templated | | [npm](https://www.npmjs.com/package/dsh-permit-report-check) |

#### 🦺 Safety & hazardous materials (7)

| Plugin | One-liner | Status | npm |
|---|---|---|---|
| [dsh-hazchem-check](https://github.com/PerryLink/dsh-hazchem-check) | Hazardous-chemical register and major-hazard-source identification, reconciled arithmetically | | [npm](https://www.npmjs.com/package/dsh-hazchem-check) |
| [dsh-emergency-plan](https://github.com/PerryLink/dsh-emergency-plan) | Emergency plan structure and the drills, contacts and review dates it must carry | | [npm](https://www.npmjs.com/package/dsh-emergency-plan) |
| [dsh-drill-script-check](https://github.com/PerryLink/dsh-drill-script-check) | Drill scripts: scenario, roles, timeline and the corrective actions a drill has to produce | | [npm](https://www.npmjs.com/package/dsh-drill-script-check) |
| [dsh-hidden-risk-map](https://github.com/PerryLink/dsh-hidden-risk-map) | Hidden-risk map: every hazard mapped to the article it is reported under, no gaps and no inventions | | [npm](https://www.npmjs.com/package/dsh-hidden-risk-map) |
| [dsh-power-ticket-check](https://github.com/PerryLink/dsh-power-ticket-check) | Work permits for electrical isolation — the safety measures each permit class requires | | [npm](https://www.npmjs.com/package/dsh-power-ticket-check) |
| [dsh-power-loss-split](https://github.com/PerryLink/dsh-power-loss-split) | Power-loss event split across causes so the totals reconcile to the reported outage | | [npm](https://www.npmjs.com/package/dsh-power-loss-split) |
| [dsh-aqua-input-check](https://github.com/PerryLink/dsh-aqua-input-check) | Aquaculture input records: batch, dosage and withdrawal periods against the limits stated | | [npm](https://www.npmjs.com/package/dsh-aqua-input-check) |

#### 🏥 Medical records (3)

| Plugin | One-liner | Status | npm |
|---|---|---|---|
| [dsh-icd-rule-check](https://github.com/PerryLink/dsh-icd-rule-check) | ICD coding pairs — dagger and asterisk, combination codes — flagged for a coder to resolve | | [npm](https://www.npmjs.com/package/dsh-icd-rule-check) |
| [dsh-medrec-qc](https://github.com/PerryLink/dsh-medrec-qc) | Medical-record front sheets checked for field completeness and code well-formedness | | [npm](https://www.npmjs.com/package/dsh-medrec-qc) |
| [dsh-nurse-record-check](https://github.com/PerryLink/dsh-nurse-record-check) | Nursing records: the observations, timings and signatures each entry is required to carry | | [npm](https://www.npmjs.com/package/dsh-nurse-record-check) |

#### 📄 Official documents & archives (3)

| Plugin | One-liner | Status | npm |
|---|---|---|---|
| [dsh-gongwen-flow-check](https://github.com/PerryLink/dsh-gongwen-flow-check) | Official-document handling flow — drafting, review, issue — checked against the regulation | | [npm](https://www.npmjs.com/package/dsh-gongwen-flow-check) |
| [dsh-gongwen-word-check](https://github.com/PerryLink/dsh-gongwen-word-check) | Document type and reference number checked against the formatting standard | | [npm](https://www.npmjs.com/package/dsh-gongwen-word-check) |
| [dsh-archive-check](https://github.com/PerryLink/dsh-archive-check) | Archive records: retention periods, catalogue fields and transfer dates | | [npm](https://www.npmjs.com/package/dsh-archive-check) |

#### 🚢 Customs & trade (8)

| Plugin | One-liner | Status | npm |
|---|---|---|---|
| [dsh-customs-doc-check](https://github.com/PerryLink/dsh-customs-doc-check) | Customs declaration pack — the documents a declaration needs, and the fields each must carry | | [npm](https://www.npmjs.com/package/dsh-customs-doc-check) |
| [dsh-hs-classify](https://github.com/PerryLink/dsh-hs-classify) | HS classification entries: the basis recorded for each code, in the form the tariff regulation requires | | [npm](https://www.npmjs.com/package/dsh-hs-classify) |
| [dsh-origin-rvc-check](https://github.com/PerryLink/dsh-origin-rvc-check) | Regional value content arithmetic for rules of origin, including the de minimis tests | | [npm](https://www.npmjs.com/package/dsh-origin-rvc-check) |
| [dsh-export-ctl-check](https://github.com/PerryLink/dsh-export-ctl-check) | Export-control screening records against the control lists and the licence conditions | | [npm](https://www.npmjs.com/package/dsh-export-ctl-check) |
| [dsh-lc-doc-check](https://github.com/PerryLink/dsh-lc-doc-check) | Letter-of-credit documents against the terms — discrepancies listed, not adjudicated | | [npm](https://www.npmjs.com/package/dsh-lc-doc-check) |
| [dsh-demurrage-ledger](https://github.com/PerryLink/dsh-demurrage-ledger) | Demurrage and detention ledger: free days, laytime arithmetic and the tariff applied | | [npm](https://www.npmjs.com/package/dsh-demurrage-ledger) |
| [dsh-railway-window](https://github.com/PerryLink/dsh-railway-window) | Railway freight windows and the cut-off dates each booking has to clear | | [npm](https://www.npmjs.com/package/dsh-railway-window) |
| [dsh-forecast-penalty](https://github.com/PerryLink/dsh-forecast-penalty) | Forecast-versus-actual penalty arithmetic, with the formula the contract states | | [npm](https://www.npmjs.com/package/dsh-forecast-penalty) |

#### ⚙️ Quality & manufacturing (8)

| Plugin | One-liner | Status | npm |
|---|---|---|---|
| [dsh-fmea-table-check](https://github.com/PerryLink/dsh-fmea-table-check) | FMEA tables — severity, occurrence, detection and the RPN arithmetic that follows from them | | [npm](https://www.npmjs.com/package/dsh-fmea-table-check) |
| [dsh-ppap-check](https://github.com/PerryLink/dsh-ppap-check) | PPAP submission completeness against the level the customer required | | [npm](https://www.npmjs.com/package/dsh-ppap-check) |
| [dsh-spc-gbt-adapter](https://github.com/PerryLink/dsh-spc-gbt-adapter) | Control charts read against the national standard: limits, rules and out-of-control signals | | [npm](https://www.npmjs.com/package/dsh-spc-gbt-adapter) |
| [dsh-pipeline-check](https://github.com/PerryLink/dsh-pipeline-check) | Pipeline inspection records: intervals, anomalies and the repairs each anomaly triggered | | [npm](https://www.npmjs.com/package/dsh-pipeline-check) |
| [dsh-warranty-calc](https://github.com/PerryLink/dsh-warranty-calc) | Automotive three-guarantee periods and thresholds, computed from the invoice and delivery dates | | [npm](https://www.npmjs.com/package/dsh-warranty-calc) |
| [dsh-repair-order-qc](https://github.com/PerryLink/dsh-repair-order-qc) | Repair orders: the settlement list, the completion certificate and the archive a repair must produce | | [npm](https://www.npmjs.com/package/dsh-repair-order-qc) |
| [dsh-ota-review-check](https://github.com/PerryLink/dsh-ota-review-check) | Over-the-air update review records — scope, rollback plan and the sign-offs required | | [npm](https://www.npmjs.com/package/dsh-ota-review-check) |
| [dsh-review-reply-check](https://github.com/PerryLink/dsh-review-reply-check) | Responses to review comments: whether every comment received an answer and a change | | [npm](https://www.npmjs.com/package/dsh-review-reply-check) |

#### 🔬 Research & academia (5)

| Plugin | One-liner | Status | npm |
|---|---|---|---|
| [dsh-nsfc-form-check](https://github.com/PerryLink/dsh-nsfc-form-check) | Grant application forms checked for the fields, limits and attachments the call requires | | [npm](https://www.npmjs.com/package/dsh-nsfc-form-check) |
| [dsh-paper-doc-adapter](https://github.com/PerryLink/dsh-paper-doc-adapter) | Manuscript formatting against a venue's own submission requirements | | [npm](https://www.npmjs.com/package/dsh-paper-doc-adapter) |
| [dsh-essay-rubric-check](https://github.com/PerryLink/dsh-essay-rubric-check) | Rubric-based marking checked for arithmetic and for criteria that went unmarked | | [npm](https://www.npmjs.com/package/dsh-essay-rubric-check) |
| [dsh-learning-gap-check](https://github.com/PerryLink/dsh-learning-gap-check) | Learning-gap analyses: the evidence cited for each gap and the interventions proposed | | [npm](https://www.npmjs.com/package/dsh-learning-gap-check) |
| [dsh-policy-brief-draft](https://github.com/PerryLink/dsh-policy-brief-draft) | Policy briefs checked for the structure a brief is expected to carry and for unsourced claims | | [npm](https://www.npmjs.com/package/dsh-policy-brief-draft) |

#### ⚖️ Evidence & litigation (3)

| Plugin | One-liner | Status | npm |
|---|---|---|---|
| [dsh-evidence-check](https://github.com/PerryLink/dsh-evidence-check) | Evidence lists against the civil evidence rules — production deadlines, notices and exchanges | | [npm](https://www.npmjs.com/package/dsh-evidence-check) |
| [dsh-pleading-draft](https://github.com/PerryLink/dsh-pleading-draft) | Pleadings checked for the elements each claim has to plead and for internal inconsistency | | [npm](https://www.npmjs.com/package/dsh-pleading-draft) |
| [dsh-lawcite-adapter](https://github.com/PerryLink/dsh-lawcite-adapter) | Legal citations resolved to the instrument actually in force, and flagged when they are not | | [npm](https://www.npmjs.com/package/dsh-lawcite-adapter) |

#### 🏛️ Governance (2)

| Plugin | One-liner | Status | npm |
|---|---|---|---|
| [dsh-soe-decision-check](https://github.com/PerryLink/dsh-soe-decision-check) | State-owned-enterprise collective-decision records against the "three majors, one large" procedure | | [npm](https://www.npmjs.com/package/dsh-soe-decision-check) |
| [dsh-sop-sync-check](https://github.com/PerryLink/dsh-sop-sync-check) | Standard operating procedures checked against the versions and cross-references they claim | | [npm](https://www.npmjs.com/package/dsh-sop-sync-check) |

#### 🧰 Compliance toolchain (9)

Nine further compliance tools published 2026-10-23, outside the 53-checker suite: six checkers and three
document tools. They declare `dsh.bundle.patch` and count in the roster; they are listed here rather than in
the ten checker domains because their packs are not part of the suite manifest.

| Plugin | One-liner | Status | npm |
|---|---|---|---|
| [dsh-bid-health-check](https://github.com/PerryLink/dsh-bid-health-check) | Locate, requirement by requirement, where a bid appears to answer a tender pack, and where it does not | | [npm](https://www.npmjs.com/package/dsh-bid-health-check) |
| [dsh-canteen-retention-check](https://github.com/PerryLink/dsh-canteen-retention-check) | Canteen food-retention ledger: the four required elements, the 125 g minimum, the 48-hour window and leftover placeholders | | [npm](https://www.npmjs.com/package/dsh-canteen-retention-check) |
| [dsh-construction-doc-check](https://github.com/PerryLink/dsh-construction-doc-check) | Project document archive: missing required document types, stale revisions and empty files, read from names rather than contents | | [npm](https://www.npmjs.com/package/dsh-construction-doc-check) |
| [dsh-excel-reconcile](https://github.com/PerryLink/dsh-excel-reconcile) | Join two spreadsheets on a declared key and compare declared fields within declared tolerances | | [npm](https://www.npmjs.com/package/dsh-excel-reconcile) |
| [dsh-invoice-ledger](https://github.com/PerryLink/dsh-invoice-ledger) | Invoice ledger: duplicates keyed on code + number, arithmetic, payer mismatch, date anomalies and placeholders | | [npm](https://www.npmjs.com/package/dsh-invoice-ledger) |
| [dsh-payroll-audit](https://github.com/PerryLink/dsh-payroll-audit) | Payroll against published social-insurance, housing-fund and individual-income-tax parameters, with four-valued outcomes | | [npm](https://www.npmjs.com/package/dsh-payroll-audit) |
| [dsh-safety-ledger-check](https://github.com/PerryLink/dsh-safety-ledger-check) | Site safety-qualification ledger: training hours, the four record elements and certificate validity | | [npm](https://www.npmjs.com/package/dsh-safety-ledger-check) |
| [dsh-table-ingest](https://github.com/PerryLink/dsh-table-ingest) | Convert .docx/.xlsx/.xlsm/.csv/.tsv tables into the table JSON the rule checkers consume | | [npm](https://www.npmjs.com/package/dsh-table-ingest) |
| [dsh-tender-requirements](https://github.com/PerryLink/dsh-tender-requirements) | Extract deadlines, deposit, validity, ceiling, bid composition and copy counts from a tender document | | [npm](https://www.npmjs.com/package/dsh-tender-requirements) |

</details>

## 🪦 Retired & frozen — the full tables

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

Frozen because **better-adopted alternatives now exist** for that capability. Four of the five own frozen
plugins carry a `## Maintenance status: 🧊 FROZEN` section in their own README with the measured comparison —
[dsh-claude-move](https://github.com/PerryLink/dsh-claude-move) is the exception among the owned ones, and
[dsh-wechat](https://github.com/pan17/dsh-wechat) is `pan17`'s repository rather than this account's, so the
banner cannot be added there and the row is frozen here instead. Weekly npm downloads, measured 2026-10-05:

| Plugin | this repo | better-adopted alternative |
|---|---|---|
| [dsh-budget](https://github.com/PerryLink/dsh-budget) | 1,079 | [`dsh-cost-meter`](https://github.com/Han-1413141/dsh-cost-meter) — **33,526** |
| [dsh-draw](https://github.com/PerryLink/dsh-draw) | 973 | [`dsh-image-gen`](https://github.com/shanliuling/dsh-image-gen) — **7,216** |
| [dsh-claude-move](https://github.com/PerryLink/dsh-claude-move) | 843 | [`dsh-chat-import`](https://github.com/Nwflower/dsh-chat-import) — **5,111** |
| [dsh-reach](https://github.com/PerryLink/dsh-reach) | ~600 | [`@xmanrui/dsh-im`](https://github.com/xmanrui/dsh-im) — **17,384** |
| [dsh-wechat](https://github.com/pan17/dsh-wechat) | 752 | [`@xmanrui/dsh-im`](https://github.com/xmanrui/dsh-im) — **17,384** |
| [dsh-defend](https://github.com/PerryLink/dsh-defend) | 937 | [`cc-safety-net`](https://github.com/kenryu42/cc-safety-net) — **13,087** |

`dsh-defend` is the one frozen package that is still the **broader** detector — an Aho-Corasick engine over
the prompt-injection / jailbreak / secret-leaker asset sets, with three-way allow/ask/block interception on
user messages, tool arguments **and** tool results. It is frozen because the field moved, not because the
plugin is weaker.

## 🌍 Where the plugins live — the figures, with their caveats

- **GitHub** (this profile), **[Gitee](https://gitee.com/perrylink)** and **npm** — source, CI and releases here; 101
repositories are mirrored to Gitee by a daily job (default branch + all tags; the mirror list does not yet
include the nine 2026-10-23 tools), plus this profile repo; the `perrylink`
account holds **117 npm names and 1,665 versions**, every one of them with a non-deprecated `latest`; **96** carry a
SLSA provenance attestation on that version and **105** on at least one (the twelve with none anywhere are
`@perrylink/dsh-checkers`, `@perrylink/dsh-checkers-suite`, `@phocinae/js`, `dsh-context-verdict`,
`dsh-customs-mcp`, `dsh-laya`, `dsh-phocinae`, `dsh-preclaim`, `jevcore-cli`, `jevcore-dsh`, `jevcore-mcp`
and `laya-mcp` — measured 2026-10-26 from each name's own packument; the names come from registry search,
which now enumerates all 117, and the count was cross-checked against the 121 `package.json` files in the
repositories themselves)
- **npm downloads** — **232,500 over the trailing 30 days** (npm window 2026-09-26..2026-10-25, summed per name over the 117
names from the downloads point endpoint.
- **dshfind** — lists **35** of the family's repositories in its sitemap (35 `…/plugins/PerryLink/<repo>` paths,
  each published in four locales) and puts a download badge on **9** of them. Read one badge per repository from
  `https://dshfind.com/api/badge/PerryLink/<repo>?metric=downloads` — the same `<img>` every plugin page
  embeds — and the nine tiers are:

  | Plugin | dshfind tier |
  |---|---|
  | dsh-auto-review | 10k+ |
  | dsh-memento | 10k+ |
  | dsh-permission-rules | 10k+ |
  | dsh-industry-research | 5k+ |
  | dsh-research-report | 5k+ |
  | dsh-mcp-panel | 2k+ |
  | jevcore | 2k+ |
  | dsh-claude-move | 1k+ |
  | dsh-plugin-guide | 500+ |

  The floors add to **45,500**, and every badge is a rounded tier rather than a count, so that is a floor
  and not a total. The other 26 repositories have no download figure at all — their badge falls back to
  ★ — which is why the aggregate is stated over 9 and not over 35.
- **DSH Desktop Market** — add the catalog source
`https://cdn.jsdelivr.net/gh/PerryLink/dsh-catalog@main/deploy/artifacts/v1/plugins.json` under Market → Sources
to browse the family in-app (109 packages, catalogue generated 2026-10-26; the `catalog-source.json` manifest in
the same directory is a template whose `endpoint` is still the `replace-with-deploy-origin.invalid`
placeholder, and the `perrylink-dsh-catalog.perrylink.workers.dev` address before it answered `HTTP 000` on
networks that interfere with `*.workers.dev`); **MCP Registry** — four servers, all published from their release workflows over GitHub OIDC: `dsh-cert-mcp`,
`dsh-customs-mcp`, `jevcore-mcp` and `laya-mcp`
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
