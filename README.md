# Hi, I'm PerryLink 👋

<!-- Editing note: every figure on this page is measured and dated, and each one has exactly one
     authoritative site. Read INSTRUMENTATION.md before changing a number. The long form of this page
     -- the merge-by-merge upstream record, the 95-row plugin roster, the retired/frozen tables and the
     npm figures with their caveats -- is PROJECTS.md; rounds go to CHANGELOG.md. -->

<p align="center">
<a href="https://github.com/PerryLink?tab=repositories"><img alt="GitHub stars" src="https://img.shields.io/github/stars/PerryLink?label=stars&affiliations=OWNER&color=24292f"></a>
<a href="https://github.com/PerryLink?tab=followers"><img alt="GitHub followers" src="https://img.shields.io/github/followers/PerryLink?label=followers&color=24292f"></a>
<a href="https://github.com/PerryLink?tab=repositories"><img alt="GitHub repos" src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.github.com%2Fusers%2FPerryLink&query=%24.public_repos&label=repos&color=24292f"></a>
<a href="https://github.com/PerryLink/perrylink/blob/main/PROJECTS.md"><img alt="merged upstream" src="https://img.shields.io/badge/upstream%20merges-440-6e7781"></a>
<a href="https://github.com/PerryLink/perrylink/blob/main/PROJECTS.md"><img alt="repositories where a merge is credited" src="https://img.shields.io/badge/credited%20repos-90-6e7781"></a>
<a href="https://github.com/PerryLink/dsh-kit"><img alt="actively maintained plugins" src="https://img.shields.io/badge/plugins-91-6e7781"></a>
<a href="https://github.com/PerryLink/perrylink/blob/main/PROJECTS.md"><img alt="compliance checkers" src="https://img.shields.io/badge/checkers-53-6e7781"></a>
<br>
<a href="https://www.npmjs.com/search?q=perrylink"><img alt="npm names" src="https://img.shields.io/badge/npm-107%20names-cb3837?logo=npm"></a>
<img alt="npm downloads 30d" src="https://img.shields.io/badge/npm%20downloads%2030d-228.2k-6e7781">
<a href="https://github.com/PerryLink/perrylink/blob/main/PROJECTS.md"><img alt="npm provenance" src="https://img.shields.io/badge/npm%20provenance-95%2F107-6e7781"></a>
<a href="https://github.com/PerryLink/dsh-auto-review/blob/main/LICENSE"><img alt="license" src="https://img.shields.io/badge/license-Apache--2.0-blue"></a>
<a href="https://github.com/PerryLink/dsh-mcp-panel/blob/main/package.json"><img alt="node" src="https://img.shields.io/badge/node-%5E22.19%20%7C%7C%20%3E%3D24-339933?logo=node.js"></a>
<br>
<a href="https://github.com/PerryLink/dsh-mcp-panel/blob/main/package.json"><img alt="dsh host corridor" src="https://img.shields.io/badge/dsh-%E2%89%A50.1.2--rc.1%20%3C0.3.0-4B32C3"></a>
<a href="https://api.securityscorecards.dev/projects/github.com/PerryLink/dsh-auto-review"><img alt="OpenSSF Scorecard — dsh-auto-review" src="https://img.shields.io/ossf-scorecard/github.com/PerryLink/dsh-auto-review?label=openssf%20scorecard"></a>
<a href="https://glama.ai/mcp/servers/PerryLink/jevcore"><img alt="Glama (flagship MCP server jevcore)" src="https://glama.ai/mcp/servers/PerryLink/jevcore/badges/score.svg"></a>
<a href="https://github.com/PerryLink/dsh-plugin-certification"><img alt="certified (flagship dsh-auto-review)" src="https://raw.githubusercontent.com/PerryLink/dsh-plugin-certification/main/badges/PerryLink__dsh-auto-review.svg"></a>
<a href="https://registry.modelcontextprotocol.io/v0/servers?search=perrylink"><img alt="MCP Registry" src="https://img.shields.io/badge/MCP%20Registry-3%20servers-6f42c1"></a>
<br>
<a href="https://perrylink.github.io/"><img alt="plugin index" src="https://img.shields.io/badge/plugin%20index-114%20pages-0b5fff"></a>
<a href="https://gitee.com/perrylink"><img alt="Gitee mirror" src="https://img.shields.io/badge/Gitee-mirror-c71d23?logo=gitee"></a>
<a href="https://dshfind.com/plugins?q=PerryLink"><img alt="dshfind downloads across the family" src="https://img.shields.io/badge/dshfind%20downloads-44.5k%2B%20across%209%20plugins-6e7781"></a>
<a href="https://cdn.jsdelivr.net/gh/PerryLink/dsh-catalog@main/deploy/catalog-source.json"><img alt="DSH Desktop Market source" src="https://img.shields.io/badge/DSH%20Desktop%20Market-source-0969da"></a>
<a href="https://doi.org/10.5281/zenodo.22901853"><img alt="Zenodo DOI" src="https://zenodo.org/badge/DOI/10.5281/zenodo.22901853.svg"></a>
</p>

I fix other people's projects, and I maintain a plugin family for
[DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness). Independent open-source developer in
Beijing — not affiliated with DeepSeek, and not a DeepSeek employee.

**Upstream** — 440 merged pull requests in 92 repositories that are not mine, from AWS, Apple, Docker,
Microsoft, NVIDIA, Prometheus, Redis, Tencent and the vLLM project down to one-person projects. **The
family** — 91 actively maintained Apache-2.0 plugins in a 104-repo family: security, workflows, research,
messaging bridges, developer experience, and since 2026-10-08 a set of 53 compliance checkers that read a
register or record set against a versioned rule pack and report the differences. Every plugin has one page at
**[perrylink.github.io](https://perrylink.github.io/)** — 114 pages, complete in the served HTML
with no JavaScript rendering them, so a reader who arrives from a search result sees the text rather than
a loading state.

## ▶ Start here

| Plugin | What it gives you | Install |
|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | Second-model auto-review on the approval chain, fail-closed by default (234★) | `dsh plugin --profile web add dsh-auto-review` |
| [dsh-research-report](https://github.com/PerryLink/dsh-research-report) | Verifiable research reports: content-addressed evidence ledger, manifest seal hash, byte-level citation checks, drift detection, disproof ledger (213★) | `dsh plugin --profile web add dsh-research-report` |
| [dsh-industry-research](https://github.com/PerryLink/dsh-industry-research) | Industry/company research: chain-map SVG with bottleneck detection, timeline, company cards, adversarial review (213★) | `dsh plugin --profile web add dsh-industry-research` |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | Approval-gated cross-session memory (`ctx.memory` + SQLite) (138★) | `dsh plugin --profile web add dsh-memento` |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Claude Code-style declarative allow/deny/ask rules plus a process-level network policy (120★) | `dsh plugin --profile web add dsh-permission-rules` |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | MCP management console: `/mcp` + Settings tab + trial calls (84★) | `dsh plugin --profile web add dsh-mcp-panel` |
| [dsh-phocinae](https://github.com/PerryLink/dsh-phocinae) | Local, non-generative verdicts for the approval chain: a small typed decision model behind `phocinae_ask` / `phocinae_gate`, with fail-closed escalation for everything it does not answer (1★) | `dsh plugin --profile web add dsh-phocinae` |

## 🦭 Phocinae — a 144.3M typed decision model

Separate from the harness: I train small language models. **[Phocinae-Largha-150M-v1](https://github.com/Phocinae/Phocinae-Largha-150M-v1)** (Apache-2.0) is a typed decision model — no text generation; one forward pass returns a verdict per question with calibrated confidence. GPU **21.0 ms** (RTX 5090) p50 per decision, CPU-only **1.64 s per case**; English typed-decisions **0.906** (400 cases / 2,000 decisions, re-measured 2026-10-09), Chinese (machine-translated eval set) 0.848. With a τ=0.6 escalate gate, **55.0%** of agent decisions stay local (79.6% at τ=0.5) and kept-subset accuracy moves 0.906 → **0.9936** (+0.0876) — the gate makes the system better, not just cheaper. Weights on [Hugging Face](https://huggingface.co/Phocinae/Phocinae-Largha-150M-v1) and [ModelScope](https://modelscope.cn/models/PerryLink/Phocinae-Largha-150M-v1); server `pip install phocinae-server`, DSH bundle [`dsh-phocinae`](https://github.com/PerryLink/dsh-phocinae) (`npm i dsh-phocinae`). Reproduction ships with the repo: seeds, row-set hashes, environment and eval scripts.

## 🧭 dsh-score — public evidence for good plugins

The family publishes **public evidence and scores** instead of another star ranking:

- **[dsh-score](https://github.com/PerryLink/dsh-attention-index)** — per-surface evidence registry, badges, bench runner and contribution receipts. Live: <https://perrylink.github.io/dsh-attention-index/>. Prior-only rows are **E0 / unrated**; paired `with` / `without` bench results are the only path to a quality slot. Repo rename to `dsh-score-index` pending.
- **[dsh-community-bench](https://github.com/PerryLink/dsh-community-bench)** — the in-app consumer: **Settings → Plugins → Community Bench**. It reads the public registry; it does **not** compute a local score.

```sh
dsh plugin --profile web add dsh-community-bench
```

## 🔧 Upstream & community contributions

*Every repository below is external to `PerryLink/*`, every row is merged work, and open proposals are
deliberately not listed. ★ re-measured 2026-10-23 for every row; the third column names the party that
owns the project, because the account name alone does not say whether that is a company, a standards body
or one person. Every external repository above 2,500★ that carries merged work is listed.*

| Repository | ★ | 项目归属方 |
|---|---|---|
| [deer-flow](https://github.com/bytedance/deer-flow) | 84,320 | **ByteDance** — the official `bytedance` org |
| [ruflo](https://github.com/ruvnet/ruflo) | 78,629 | ruvnet (rUv / Reuven Cohen) — individual maintainer |
| [reactive-resume](https://github.com/reactive-resume/reactive-resume) | 44,746 | `reactive-resume` org — independent open-source project (rxresu.me) |
| [black](https://github.com/psf/black) | 41,989 | **Python Software Foundation** — the official `psf` org; the Black formatter |
| [zoxide](https://github.com/ajeetdsouza/zoxide) | 40,256 | ajeetdsouza (Ajeet D'Souza) — individual maintainer; the smarter `cd` command |
| [fiber](https://github.com/gofiber/fiber) | 40,229 | **the gofiber project** — the official `gofiber` org (gofiber.io), the Express-inspired Go web framework |
| [laya](https://github.com/NandhaKishorM/laya) | 34,041 | NandhaKishorM — individual maintainer |
| [cli](https://github.com/urfave/cli) | 24,304 | the `urfave` org — community-maintained Go CLI framework |
| [learn-harness-engineering](https://github.com/walkinglabs/learn-harness-engineering) | 21,197 | `walkinglabs` community org — the harness-engineering tutorial site |
| [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) | 20,290 | `awesome-dsh-plugin` org — community catalog, no company behind it |
| [MMKV](https://github.com/Tencent/MMKV) | 18,767 | **Tencent** — the official `Tencent` org; the key-value store behind WeChat |
| [SkillOpt](https://github.com/microsoft/SkillOpt) | 18,646 | **Microsoft** — the official `microsoft` org |
| [ioredis](https://github.com/redis/ioredis) | 15,347 | **Redis** — the official `redis` org; the Node.js Redis client |
| [FlashMLA](https://github.com/deepseek-ai/FlashMLA) | 13,168 | **DeepSeek** — the official `deepseek-ai` org |
| [txtai](https://github.com/neuml/txtai) | 13,029 | **NeuML** — the `txtai` project of NeuML, an independent open-source project |
| [mcp](https://github.com/awslabs/mcp) | 9,820 | **Amazon Web Services (AWS)** — the official `awslabs` org |
| [BrowserSkill](https://github.com/Tencent/BrowserSkill) | 9,437 | **Tencent** — the official `Tencent` org |
| [dsh-web](https://github.com/zhu1090093659/dsh-web) | 9,361 | zhu1090093659 — individual maintainer |
| [Cordis](https://github.com/cordiverse/cordis) | 9,345 | **cordiverse** org — the kernel DeepSeek Harness vendors as `@deepseek-ai/cordis` |
| [jc](https://github.com/kellyjonbrazil/jc) | 8,694 | kellyjonbrazil (Kelly Brazil) — individual maintainer |
| [dsh-market](https://github.com/dsh-market/dsh-market) | 8,397 | `dsh-market` org — the community plugin market behind dshmarket.com |
| [models.dev](https://github.com/anomalyco/models.dev) | 7,356 | `anomalyco` org — the model-catalogue site behind models.dev |
| [kraken](https://github.com/uber/kraken) | 6,771 | **Uber** — the official `uber` org; the Kraken P2P Docker registry |
| [koishi](https://github.com/koishijs/koishi) | 6,281 | `koishijs` org — the cross-platform chatbot framework |
| [ouroboros](https://github.com/Q00/ouroboros) | 6,264 | Q00 (`@zep-us`) — individual maintainer |
| [client_golang](https://github.com/prometheus/client_golang) | 6,043 | **Prometheus** — the official `prometheus` org (CNCF project); the Go instrumentation client |
| [teamai-cli](https://github.com/Tencent/teamai-cli) | 5,631 | **Tencent** — the official `Tencent` org |
| [go-sdk](https://github.com/modelcontextprotocol/go-sdk) | 5,264 | the `modelcontextprotocol` org — the Go SDK for MCP |
| [aibrix](https://github.com/vllm-project/aibrix) | 5,160 | **the vLLM project** — the official `vllm-project` org |
| [embedding-atlas](https://github.com/apple/embedding-atlas) | 4,994 | **Apple** — the official `apple` org |
| [docker-agent](https://github.com/docker/docker-agent) | 4,601 | **Docker, Inc.** — the official `docker` org |
| [agent-client-protocol](https://github.com/agentclientprotocol/agent-client-protocol) | 4,491 | `agentclientprotocol` org — governed jointly by **Zed Industries** and **JetBrains** |
| [DSH-better-sidebar](https://github.com/omdsh-dev/DSH-better-sidebar) | 4,465 | `omdsh-dev` community org — the DeepSeek Harness sidebar plugin |
| [content](https://github.com/nuxt/content) | 3,671 | **Nuxt** — the official `nuxt` org |
| [evalscope](https://github.com/modelscope/evalscope) | 3,580 | `modelscope` org — the ModelScope model-hub project |
| [fastmcp](https://github.com/punkpeye/fastmcp) | 3,277 | punkpeye (Frank Fiegel) — individual maintainer at Glama |
| [deepseek-harness-desktop](https://github.com/dsh-tauri/deepseek-harness-desktop) | 3,241 | `dsh-tauri` community org — self-described non-official and non-commercial |
| [minio-go](https://github.com/minio/minio-go) | 3,011 | **MinIO** — the official `minio` org; the Go client for MinIO and S3-compatible storage |
| [open5gs](https://github.com/open5gs/open5gs) | 2,787 | the `open5gs` 5G core project — community, no company owner |
| [claude-agent-acp](https://github.com/agentclientprotocol/claude-agent-acp) | 2,685 | `agentclientprotocol` org — governed by Zed and JetBrains |
| [NeMo-Agent-Toolkit](https://github.com/NVIDIA/NeMo-Agent-Toolkit) | 2,670 | **NVIDIA** — the official `NVIDIA` org |

<details>
<summary><b>Twenty-one of them, briefly — what was broken and who merged it</b></summary>

- **deer-flow** — a portability fix in a blocking-IO test, merged by `WillemJiang`; the largest row in the
  table.
- **zoxide** — a bare `z` under `_ZO_ECHO=1` called `Set-Location` without `-Passthru`, so the `$dir`
  assignment was `$null` and strict mode threw `PropertyNotFoundException`; the no-path branch now passes
  `-Passthru`. Merged by `ajeetdsouza`, who dropped the regression test from the branch before merging.
- **prometheus/client_golang** — `checkMetricConsistency` compared each label name with the previous one
  before the pairs were sorted, so non-adjacent duplicates passed and a scrape of the registry was dropped
  as a whole; the sort now runs before the duplicate loop, with an adjacent control and a non-adjacent
  regression test. Merged by `bwplotka`.
- **fiber** — an optional path parameter swallowed the `/` after it, so `/api/:day-:month?-:year?` matched
  one segment too many; merged by `ReneWerner87`.
- **black** — `_write_to_stdout()` already translates `\n` into the platform newline, so the
  trailing-newline fixup appended a second one: CRLF input without a trailing newline could come out as
  `\r\r\n`. It now appends a bare `\n` and lets the writer translate it; merged by `cobaltt7`.
- **urfave/cli** — `HandleExitCoder` recognised an `ExitCoder` only through a bare type assertion, so an
  exit error wrapped with `fmt.Errorf("%w")` printed nothing and fell back to exit code 1. The
  `MultiError` ordering is unchanged; `Juneezee` rebased it onto a `main` that now requires Go 1.26,
  squashed the two golden-regenerating commits, and switched the last lookup to `errors.AsType` before
  merging.
- **kraken** — the cache file reader opened to duplicate a committed upload to a replica was never closed,
  leaking one file descriptor per replica for every uploaded blob; both replication paths now register it
  with the server's closer set. Merged by `gkeesh7` after `sambhav-jain-16` asked for the two cases to be
  one table.
- **ioredis** — an auto-pipelining fix, merged by `PavelPashov`.
- **nuxt/content** — `generateItemSurround` dropped the previous item whenever `before` was larger than the
  item's index, instead of returning a shorter window; approved and merged by `farnabaz` minutes apart.
- **MMKV** — the Win32 flag mapper put the *creation disposition* into `dwDesiredAccess`, so restoring over
  an existing mapped file failed; it now goes to `dwCreationDisposition`, with a test that does the restore.
  Merged into `dev` by `lingol`, so no commit of this account sits on `master`.
- **txtai** — cut down over three pull requests after the maintainer asked three times; merged by
  `davidmezzetti`.
- **AWS `awslabs/mcp`** — a one-file UTF-8 fix, merged by `markjschreiber` with two approvals.
- **Tencent BrowserSkill** — merged by `iuyo5678` with eight checks green.
- **Apple embedding-atlas** — line-ending normalization in a release script, merged by `donghaoren`.
- **vLLM aibrix** — two flaky-test fixes.
- **Microsoft SkillOpt** — a UTF-8 state-file fix.
- **koishi** — the maintainer found and fixed a regression in this account's own patch before merging it.
- **NVIDIA NeMo-Agent-Toolkit** — three review rounds to make `remove_r1_think_tags` actually remove think
  blocks; merged by NVIDIA's `rapids-bot`.
- **jc** — a Windows platform-name fix; it started counting when `master` caught up the next day.
- **modelscope evalscope** — a UTF-8 BOM dataset fix, merged by `Yunnglin`.
- **MinIO `minio-go`** — `RemoveObjects` reported a single error for a whole batch, hiding which object had
  failed; it now reports one result per failed object, merged by `klauspost`.

</details>

Eight more repositories between 1,000★ and 2,500★, the long tail below that, the per-merge record behind
the 440, the `laya` ledger and the `deepseek-ai` picture are all in **[PROJECTS.md](PROJECTS.md)**.

## 📦 The rest of the family

**99 repositories declare the `dsh.bundle.patch` contract and 91 are actively maintained** (3 retired, 5
frozen), plus the support repositories — `dsh-kit`, `dsh-catalog`, the certification registry and the CI
checker — and one third-party plugin carried as a row. The roster's source of truth is `plugins.txt` in
**[dsh-kit](https://github.com/PerryLink/dsh-kit)**, with a parity script holding the family to that file;
the machine-readable catalogue is **[dsh-catalog](https://github.com/PerryLink/dsh-catalog)**, which is
also the DSH Desktop Market source. One line per plugin, with its status and npm name, is in
**[PROJECTS.md](PROJECTS.md)** — 95 rows in ten tables.

| | # | Some of what is in it |
|---|---|---|
| 🔒 Security | 4 | [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) · [dsh-mask](https://github.com/PerryLink/dsh-mask) · [dsh-defend](https://github.com/PerryLink/dsh-defend) |
| 🔁 Workflows | 8 | [dsh-checkpoint-rewind](https://github.com/PerryLink/dsh-checkpoint-rewind) · [dsh-github](https://github.com/PerryLink/dsh-github) · [dsh-test-drive](https://github.com/PerryLink/dsh-test-drive) |
| ✨ Experience & UX | 4 | [dsh-memento](https://github.com/PerryLink/dsh-memento) · [dsh-composer-history](https://github.com/PerryLink/dsh-composer-history) · [dsh-output-styles](https://github.com/PerryLink/dsh-output-styles) |
| 🧪 Evaluation | 3 | [dsh-doublecheck](https://github.com/PerryLink/dsh-doublecheck) · [dsh-score](https://github.com/PerryLink/dsh-attention-index) · [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) |
| 📊 Observability & cost | 5 | [dsh-observe](https://github.com/PerryLink/dsh-observe) · [dsh-autotier](https://github.com/PerryLink/dsh-autotier) · [dsh-fast](https://github.com/PerryLink/dsh-fast) · [dsh-phocinae](https://github.com/PerryLink/dsh-phocinae) |
| 🎨 Content & knowledge | 5 | [dsh-talk](https://github.com/PerryLink/dsh-talk) · [dsh-translate](https://github.com/PerryLink/dsh-translate) · [dsh-library](https://github.com/PerryLink/dsh-library) |
| 🛠️ Developer experience | 6 | [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) · [dsh-plugin-guide](https://github.com/PerryLink/dsh-plugin-guide) · [jevcore](https://github.com/PerryLink/jevcore) |
| 📱 Messaging & bridges | 3 | [dsh-ticktick](https://github.com/PerryLink/dsh-ticktick) · [dsh-reach](https://github.com/PerryLink/dsh-reach) · [dsh-wechat](https://github.com/pan17/dsh-wechat) |
| 🔬 Research | 4 | [dsh-research-report](https://github.com/PerryLink/dsh-research-report) · [dsh-industry-research](https://github.com/PerryLink/dsh-industry-research) · [dsh-fund-research](https://github.com/PerryLink/dsh-fund-research) |
| ✅ Compliance checkers | 53 | A register or record set read against a versioned rule pack, ten domains from tendering to litigation — the list is in [PROJECTS.md](PROJECTS.md) |

## 🪦 Retired & frozen (2026-10-05)

A maintainer review against the official harness and the wider ecosystem retired three plugins because
the **harness now implements the capability natively** — [dsh-background-agents](https://github.com/PerryLink/dsh-background-agents)
(native continuable subagents), [dsh-session-pin](https://github.com/PerryLink/dsh-session-pin) (built-in
session pinning) and [dsh-team-rooms](https://github.com/PerryLink/dsh-team-rooms) (Agent Teams) — and
froze six because **a better-adopted alternative now exists**: `dsh-budget`, `dsh-draw`, `dsh-claude-move`,
`dsh-reach`, `dsh-wechat` and `dsh-defend`.

Retired does not mean broken: compatibility updates stop, existing installs keep working, and the
capability is either official now or served better elsewhere. The per-plugin measurements — this
repository's weekly downloads against the alternative's, and what each row was retired in favour of — are
in **[PROJECTS.md](PROJECTS.md)**, under "Retired & frozen — the full tables".

## 🌍 Where the plugins live

- **GitHub** (this profile), **[Gitee](https://gitee.com/perrylink)** and **npm** — source, CI and releases
  here; 99 family repos mirrored to Gitee by a daily job (default branch and all tags). The `perrylink` npm
  account holds **107 names and 1,601 versions**; **95** of them carry a SLSA provenance attestation on at
  least one version, **75** on the current `latest`.
- **npm downloads** — **228,164 over the trailing 30 days** (window 2026-09-19..10-18).
  [dshfind](https://dshfind.com/plugins?q=PerryLink) indexes **106** of the family's repositories and
  publishes a download badge for **9** of them — three at 10k+, two at 5k+, one at 2k+, two at 1k+ and one
  at 500+ — which add to **44,500+**. The badges are rounded tiers, so that is a floor and not a total.
- **DSH Desktop Market** — add
  `https://cdn.jsdelivr.net/gh/PerryLink/dsh-catalog@main/deploy/artifacts/v1/plugins.json` under
  Market → Sources to browse the family in-app (99 packages, catalogue generated 2026-10-18).
- **MCP Registry** — three servers, all published from their release workflows over GitHub OIDC:
  `dsh-cert-mcp`, `jevcore-mcp` and `laya-mcp`.
- **GitHub Actions** — [dsh-github](https://github.com/PerryLink/dsh-github) and
  [dsh-test-drive](https://github.com/PerryLink/dsh-test-drive) also ship composite actions, so they
  install as `uses: PerryLink/dsh-test-drive@vX`.
- **Third-party directories** — a dozen-plus DSH lists and indexes ingest the
  [`dsh-plugin` topic](https://github.com/topics/dsh-plugin); the family is scored on
  [OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/PerryLink/dsh-auto-review).

<details>
<summary><b>中文介绍</b></summary>

独立开源开发者，在北京，与 DeepSeek 无隶属关系。两条线：**给别人的项目修 bug**（AWS、Apple、Docker、
Microsoft、NVIDIA、Redis、Tencent、vLLM，也包括一个人的小项目），以及**给 DeepSeek Harness 维护一套
Apache-2.0 插件生态** —— 安全、工作流、研究、消息桥接、开发者体验，加上一批合规核查插件。

每个插件都有一页静态介绍：**[perrylink.github.io](https://perrylink.github.io/)**，正文直接写在 HTML
里，不靠 JavaScript 渲染。也向上游 [Cordis](https://github.com/cordiverse/cordis)（DeepSeek Harness 所基于的
插件内核框架）与 [deepseek-ai](https://github.com/deepseek-ai) 提交修复，逐条清单在 PROJECTS.md。

还有一条在别处：一个根本起不来的进程现在能起来了。[claude-agent-acp #1146](https://github.com/agentclientprotocol/claude-agent-acp/pull/1146)
让 `src/index.ts` 里那处没有保护的顶层 await 不再因一次瞬时错误就中断模块求值、在发出任何一条 ACP 消息
之前退出。

数字只在上面的英文部分维护一份，逐条清单、名册与退役表在 [PROJECTS.md](PROJECTS.md)；这里不重复，
以免两处走样。

</details>

---

*Measured, not remembered.* The full inventory — the merge-by-merge upstream record, the 95-row plugin
roster, the retired and frozen tables, and the npm and registry figures with their caveats — is in
**[PROJECTS.md](PROJECTS.md)**. How every figure is measured is in
[INSTRUMENTATION.md](https://github.com/PerryLink/perrylink/blob/main/INSTRUMENTATION.md), and what each
round corrected is in [CHANGELOG.md](https://github.com/PerryLink/perrylink/blob/main/CHANGELOG.md).
