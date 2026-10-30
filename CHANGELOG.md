# Round log

The profile README used to carry its rounds inline and rotate the oldest out to git history every
edition. That kept the landing page long and made the oldest round hard to find. The rounds live
here instead; the README keeps a pointer and nothing else.

A round is a **dated snapshot**. Its counters are that round's, not the page's, so an old round is
never "corrected" when a number moves later — the correction belongs to the round that found it.
Every figure in every round below was measured on the date in its heading.

Rounds before 2026-09-25 (09-24, 09-23, 09-22, 09-21, 09-20) were rotated out before this file
existed and are recoverable from the repository's git history; the 09-21 round was where `laya-mcp`
and `dsh-laya` were introduced by name.

---

## 2026-10-30 (third round)

- **Two first-time repositories were credited.** [`langgenius/dify#44333`](https://github.com/langgenius/dify/pull/44333)
  (reject 4xx/5xx responses in `download_with_size_limit` instead of returning the error page)
  was merged by `Stream29` at 17:55:46Z, and
  [`prometheus/client_python#1231`](https://github.com/prometheus/client_python/pull/1231)
  (bind `max_fds` before using it in the process collector) by `csmarchbanks` at 18:39:55Z.
  Both merge commits carry this account as their author.
- **482 total: 448 + 34**, across **96 repositories**, **93** of them credited, re-derived with
  `00-live/_profile-derive.mjs` at 2026-10-30T22:40:00Z. **163** proposals are open across **123**
  repositories as of 2026-10-30T22:50:00Z.

## 2026-10-30 (second round)

- **Two `cordis` fixes merged by `shigma`.** [`cordiverse/cordis#277`](https://github.com/cordiverse/cordis/pull/277)
  (`perf(core): notify only the services a fiber provides`) landed at 06:02:00Z and
  [`#267`](https://github.com/cordiverse/cordis/pull/267) (`fix(loader): treat an empty string as an isolate label`)
  at 07:35:26Z. Both merge commits carry this account as their author, so both count.
- **480 total: 446 + 34**, across **94 repositories**, **91** of them credited, re-derived with
  `00-live/_profile-derive.mjs` at 2026-10-30T16:12:57Z. **163** proposals are open across **123**
  repositories: the two merges removed two, and `psf/black#5641` plus the human-filed `pandas#71776`
  added two. `cordis` was already credited, so the repository count stays at 91.

---

## 2026-10-30

- **Four merges landed overnight, all in repositories that already carried a credited commit.**
  [`psf/black#5639`](https://github.com/psf/black/pull/5639) (the B045 loop-variable lint, merged by
  `cobaltt7` after the changelog entry was dropped) and
  [`psf/black#5638`](https://github.com/psf/black/pull/5638) (optional parens for a commented
  assignment RHS) landed at 2026-10-29T21:44:42Z and 2026-10-29T21:52:45Z;
  [`docker/docker-agent#4754`](https://github.com/docker/docker-agent/pull/4754) and
  [`#4744`](https://github.com/docker/docker-agent/pull/4744) were approved and queue-merged by
  `aheritier` at 22:45:14Z and 22:46:11Z.
- **478 total: 444 + 34**, across **94 repositories**, **91** of them credited, re-derived with
  `00-live/_profile-derive.mjs` at 2026-10-30T04:45:00Z. **163** proposals are open across **121**
  repositories. `Anil-matcha/open-genjutsu` lost the commit this account had on `main` (the branch now
  holds only the initial commit, although #63 was merged on 2026-09-22), so it joins `SihanTeng` (32) and
  `Tencent/MMKV` (1) on the uncredited side: **34**.

---

## 2026-10-29

- **`ZSeven-W/openpencil#264` merged at 2026-10-29T02:46:01Z by `Kayshen-X`** — the documented
  `install-op.sh` command asked `/releases/latest`, which is a 404 while every published tag is a
  pre-release; it now falls back to the newest pre-release with a note, so the default install works
  before the first stable release. The star table was last re-measured 2026-10-28.
- **474 total: 441 + 33**, across **94 repositories**, **92** of them credited. The previous prose
  said 91 credited of 93 — the re-derivation counts one more repository, which the page's own
  49 + 43 credited rows already listed. **168** proposals are open across **120** repositories as of
  2026-10-29T10:06:23Z.

## 2026-10-28 (second round)

- **No new merges since 2026-10-28T04:38:27Z.** The 473 total, the 440 + 33 split and the 91 credited
  repositories are unchanged; 169 proposals are open across 120 repositories as of 2026-10-28T15:37:09Z.
- **Six new upstream proposals, each reproduced locally before it was sent.** `kriszyp/msgpackr#225`:
  an `AggregateError` round-trip lost its message and errors — the encoder now carries `errors` and the
  decoder rebuilds `AggregateError(errors, message, { cause })`, while a three-entry payload still decodes;
  `#226`: `-0` was packed as the positive fixint 0, so the sign was lost — it is written as float64 now.
  `pydantic/genai-prices#899`: LiteLLM's `fireworks_ai/` prefix never resolved to the Fireworks provider;
  a `provider_match` for `fireworks` fixes it, with the Python, Go, Rust and JS package data regenerated.
  `kellyjonbrazil/jc#860`: `w -h` output has neither the uptime line nor the column header, so one session
  raised `IndexError` and several parsed as `[]`; the header is optional now, with a headerless fixture.
  `ZSeven-W/openpencil#264`: the documented installer asked `/releases/latest`, which is a 404 while every
  published tag is a pre-release; it now falls back to the newest pre-release with a note.
  `docker/docker-agent#4754`: with `code_mode_tools: true`, `transfer_task` was wrapped into the JavaScript
  toolset where it could not be called, so delegation failed; runtime-handled tools stay direct now.
- **In-flight work advanced.** `redis/go-redis#4168` merged `master` after the maintainer asked for the
  conflicts to be resolved, and its CI is green; `ZSeven-W/openpencil#261` was rebased so the diff is one
  file (+109/−7) instead of 2,055 files.
- **The star table was re-measured on 2026-10-28** — all 49 rows in `README.md` and `PROJECTS.md` carry the
  current counts.

## 2026-10-28

- **Four `laya` pull requests merged within one second.** [`NandhaKishorM/laya#1397`](https://github.com/NandhaKishorM/laya/pull/1397)
  merged at 2026-10-28T04:38:27Z: a `--questions` path that cannot be read is a usage error naming the
  file, not a "could not run Laya" download diagnosis. [`#1398`](https://github.com/NandhaKishorM/laya/pull/1398):
  the `--questions`, `--batch` and evidence readers open as `utf-8-sig`, so a Windows-editor BOM is a
  signature rather than data — a valid questions file was refused as "not valid JSON", and a batch BOM
  became the first request's first character. [`#1400`](https://github.com/NandhaKishorM/laya/pull/1400):
  `assert_regression` names the delta it failed on for an incomparable coverage definition and a NaN
  tolerance, where it used to print `evaluation regressed: {}`. [`#1401`](https://github.com/NandhaKishorM/laya/pull/1401):
  `evaluate()` refuses a batch reply with fewer results than rows instead of silently under-scoring the
  report. Each carries a focused test.
- **`cordiverse/cordis#268`** merged at 2026-10-27T18:34:21Z by `shigma`: an async-generator effect
  abandoned on an epoch change never ran its `finally`; the effect is closed with `iter.return()` now.
- **`uber/kraken#730`** merged at 2026-10-27T14:43:00Z by `thijmv`: a successful piece read is recorded
  when the reader closes. `gkeesh7` asked for the two tests to be table-driven, and they are one table now.
- **`helm/chart-releaser-action#241`** merged at 2026-10-27T13:44:01Z by `cpanato` — a new credited
  repository: chart discovery no longer drops paths that are not ASCII.
- **`neuml/txtai#1472`** merged at 2026-10-27T14:30:40Z by `davidmezzetti`: `SQL.issql()` accepts a valid
  statement with extra whitespace around tokens or after the semicolon.
- **Two catalog batches landed in `walkinglabs`' list** — `#131` at 15:35:16Z and `#132` at
  2026-10-28T01:31:36Z: six data/session/bench plugins and six compliance/document tools.
- **One pull request was closed, not merged.** [`redis/ioredis#2254`](https://github.com/redis/ioredis/pull/2254)
  (a SELECT inside a discarded MULTI kept the client's db state) was closed by the maintainer: the
  contributing guide asks for an issue and an agreed approach first, and the review found the patch also
  stopped tracking a successful SELECT inside `pipeline().multi()` and left the transaction flag set
  after `DISCARD`. Both points are recorded; a real workload hitting it would start with an issue.
- **Counters.** The external set is now **473 merges across 93 repositories** (was 463 / 92), **440
  credited in 91** (was 430 / 90), the same **33 uncredited in 2** — `SihanTeng`'s list at 32 and
  `Tencent/MMKV` at 1 — and **163 open across 120** (was 162 / 123). Re-derived 2026-10-28T04:50:49Z.
- **Named table stays at 41 rows; no star row was re-read this round.**

## 2026-10-27 (second round)

- **Two long-running reviews closed.** [`modelscope/evalscope#1937`](https://github.com/modelscope/evalscope/pull/1937)
  merged at 2026-10-27T06:55:45Z by `Yunnglin`: a local model that emits tool calls inside its text
  should surface them as `tool_calls` with `finish_reason = 'tool_calls'`; the change reads them out of
  the text and the review's generate-level tests cover it. [`pydantic/pydantic-extra-types#462`](https://github.com/pydantic/pydantic-extra-types/pull/462)
  merged at 2026-10-27T10:07:25Z by `yezz123`: a coordinate with an out-of-range Decimal component was
  accepted and serialized; the bounds are checked before the value is built, and the invalid input now
  raises. Both squashed merge commits are authored by this account, so both are credited.
- **Counters.** The external set is now **463 merges across 92 repositories** (was 461 / 92), **430
  credited in 90** (was 428 / 90), the same **33 uncredited in 2** — `SihanTeng`'s list at 32 and
  `Tencent/MMKV` at 1 — and **162 open across 123** (was 164 / 125). Re-derived 2026-10-27T11:49:22Z.
- **Named table stays at 41 rows; no star row was re-read this round.**

## 2026-10-27

- **Nineteen merges landed overnight; two are code fixes, the rest are catalog entries.** [`neuml/txtai#1400`](https://github.com/neuml/txtai/pull/1400)
  merged at 2026-10-26T16:19:05Z by `davidmezzetti`: a URL with no filename made `os.path.basename()` return
  empty, so the destination resolved to the output directory and the write failed; the filename now falls
  back to `download`. [`punkpeye/fastmcp#463`](https://github.com/punkpeye/fastmcp/pull/463) merged at
  2026-10-27T04:47:03Z by `punkpeye`: an OpenAPI `$ref` pointing *into* a component
  (`#/components/schemas/Pet/properties/name`) was read as a definition named `Pet/properties/name`, so
  nothing was attached and the tool could never be called; the first pointer segment is the definition.
  The other seventeen are catalog additions — four in `awesome-dsh-plugin` (three plugins each) and
  thirteen in `imsai-sh/awesome-deepseek-harness-plugins` (one plugin each).
- **Counters.** The external set is now **461 merges across 92 repositories** (was 442 / 92), **428
  credited in 90** (was 409 / 90), the same **33 uncredited in 2** — `SihanTeng`'s list at 32 and
  `Tencent/MMKV` at 1 — and **164 open across 125** (was 160 / 123). Re-derived 2026-10-27T05:03:54Z.
- **The named table stays at 41 rows, the 1,000–2,500★ table at eight rows.** No star row was re-read this round.

## 2026-10-26 (fourth round) — full re-measure

- **A full re-measure, not another counter refresh.** The 14:09:41Z third round added
  `redis/ioredis#2248` and moved the counters to **442 merges across 92 repositories**, **409 credited
  in 90**, **33 uncredited in 2** — `SihanTeng`'s list at 32 and `Tencent/MMKV` at 1 — and **160 open
  across 123**. This round adopts those counters and re-reads every star, the npm registry, the family
  roster, the site sitemap, the Market catalogue and the dshfind index against them.
- **Stars.** Every one of the 41 rows above 2,500★ and the eight between 1,000★ and 2,500★ was read
  again. Largest moves: `ruflo` 78,629 → 79,411, `dsh-market` 8,397 → 9,026, `awesome-dsh-plugin`
  20,290 → 20,845. Two ordering swaps follow from the new values: `dsh-market` above `jc`, and
  `DSH-better-sidebar` above `agent-client-protocol`. `PROJECTS.md` had lost six named rows — `black`,
  `zoxide`, `urfave/cli`, `kraken`, `prometheus/client_golang` and `minio-go` — in an earlier edit; they
  are restored, so both tables carry the same 41.
- **Family.** The roster is **108** (110 repositories declaring `dsh.bundle.patch`, minus the two
  retired corridor legs), **100 active** (3 retired + 5 frozen) and **105 table rows**. Nine compliance
  tools published 2026-10-23 account for the move from 99 / 91 / 95, and `dsh-phone-inbox` gets its
  missing row. The 53-checker suite is unchanged; the nine sit in a separate toolchain table.
  `plugins.txt` and `data/repos.json` still carry the 2026-10-19 cut of 99 and are called out on the
  page rather than quietly redefined.
- **npm.** 117 names (+10), 1,665 versions (+64), **96** with provenance on `latest`, **105** on at
  least one, and **232,500** downloads in 2026-09-26..2026-10-25. The twelve names with no provenance
  anywhere changed by one: `dsh-customs-mcp` replaces `dsh-batch-triage`.
- **Site and registry.** The sitemap now serves 123 pages (53 checker + 56 plugin + 13 Chinese + the
  home page), up from 114; 12 new project pages were added for the nine 2026-10-23 tools and three
  support plugins. The Market catalogue is 109 packages, regenerated 2026-10-26T14:30:15Z. The MCP
  Registry now has four servers: `dsh-customs-mcp` joined `dsh-cert-mcp`, `jevcore-mcp` and `laya-mcp`.
- **dshfind.** Its sitemap now lists 1,596 plugins in two shards and only **35** of this family's
  repositories (the page previously carried 106 from a page-count probe, not from the sitemap); pages
  outside it carry `noindex`. Nine of the 35 have a download tier, adding to **45,500+** — 1,000 above
  the 44,500 the page carried, because `jevcore` moved from 1k+ to 2k+ — and the distribution is now
  3 / 2 / 2 / 1 / 1 (10k+ / 5k+ / 2k+ / 1k+ / 500+).
- **Gitee.** The workflow's list carries 101 repositories, not 99.

---

## 2026-10-26 (third round)

- **One merge landed about eighty minutes after the second round.** [`redis/ioredis#2248`](https://github.com/redis/ioredis/pull/2248)
  merged at 2026-10-26T14:07:06Z by `PavelPashov`: `sendCommand` recorded the selected database with
  `command.name === "select"`, but command names keep the casing the caller used (`call("SELECT", 2)`),
  so any spelling other than lowercase never updated `condition.select` — the reconnect handshake then
  restored the stale database and later commands ran against the wrong keyspace, silently. The check now
  lowercases the name, matching the client's other case-insensitive command-name comparisons; the
  squashed merge commit is authored by this account, so the merge is credited. `PavelPashov` replaced the
  branch's mock-server test with a shorter one against a live connection that asserts `CLIENT INFO`
  reports `db=2`.
- **Counters.** The external set is now **442 merges across 92 repositories** (was 441 / 92), **409
  credited in 90** (was 408 / 90), the same **33 uncredited in 2** — `SihanTeng`'s list at 32 and
  `Tencent/MMKV` at 1 — and **160 open across 123** (was 162 / 124). Re-derived 2026-10-26T14:09:41Z.
- **The named table stays at 41 rows, the 1,000–2,500★ table at eight rows.** `ioredis` was already in
  the named table; no star row was re-read this round.

---

## 2026-10-26 (second round)

- **One merge landed nine minutes after the morning derivation.** [`nuxt/content#3894`](https://github.com/nuxt/content/pull/3894)
  merged at 2026-10-26T12:44:39Z by `farnabaz`: the `ORDER BY` validator accepted only `[a-zA-Z_]+` while
  the `SELECT`/`WHERE` checks accepted digits, so `queryCollection(...).order('publishedAt2', 'DESC')`
  failed on the server path while the client WASM path worked; the column pattern is now `\w*` after the
  first character, with the escaping and injection controls unchanged. The repository was already credited,
  so the merged counts move without a new repository.
- **Counters.** The external set is now **441 merges across 92 repositories** (was 440 / 92), **408
  credited in 90** (was 407 / 90), the same **33 uncredited in 2** — `SihanTeng`'s list at 32 and
  `Tencent/MMKV` at 1 — and **162 open across 124** (was 163 / 125). Re-derived 2026-10-26T12:48:13Z.
- **The named table stays at 41 rows, the 1,000–2,500★ table at eight rows.** `nuxt/content` was already
  in the named table; no star row was re-read this round.

## 2026-10-26

- **Four merges landed after the 10-25 derivation.** [`urfave/cli#2503`](https://github.com/urfave/cli/pull/2503)
  merged at 2026-10-25T16:51:54Z by `Juneezee`: `extFlag.IsSet` was a stub that always returned false, so
  `Command.IsSet`, `NumFlags` and the flag-name listings ignored flags parsed through `AllowExtFlags`;
  the branch tracked the set state and, while reviewing, `Juneezee` also fixed the related gaps — undo only
  what the previous run set, don't let a Go flag hide a same-named flag, don't panic on a Go flag without
  `Get`, and record flags set directly on `flag.CommandLine`.
  [`NVIDIA/NeMo-Agent-Toolkit#2452`](https://github.com/NVIDIA/NeMo-Agent-Toolkit/pull/2452) merged at
  2026-10-25T17:45:52Z by `rapids-bot` after `willkill07` issued `/merge`: `--config_file` was applied
  before the saved channel settings, so the saved values won; the override now wins and is revalidated in
  memory, as the review asked, instead of being written back to `config.json`.
  [`AnotiaWang/deep-research-web-ui#105`](https://github.com/AnotiaWang/deep-research-web-ui/pull/105)
  merged at 2026-10-26T09:22:58Z by `AnotiaWang`: both READMEs told users to pull
  `anotia/deep-research-web-ui:latest`, but the publish workflow builds `deep-research-web`; the image
  name in the Helodata example now matches.
  [`agentclientprotocol/claude-agent-acp#1373`](https://github.com/agentclientprotocol/claude-agent-acp/pull/1373)
  merged at 2026-10-26T10:25:48Z by `benbrandt`: the acp-v2 teardown's `rm` raced with Windows file
  handles and failed the suite after the assertions had passed; it now passes `maxRetries: 10`.
- **Counters.** The external set is now **440 merges across 92 repositories** (was 436 / 91), **407
  credited in 90** (was 403 / 89), the same **33 uncredited in 2** — `SihanTeng`'s list at 32 and
  `Tencent/MMKV` at 1 — and **163 open across 125** (was 168 / 130). Re-derived 2026-10-26T12:35:07Z.
  `deep-research-web-ui` is the new credited repository: its #105 commit is authored by this account, and
  at **2,223★** it joins the 1,000–2,500★ table, which moves from seven rows to eight.
- **The named table stays at 41 rows.** Nothing crosses the 2,500★ line this round; the star column was
  last re-read on 2026-10-23, except the new 2,223★ row.

## 2026-10-25

- **Six merges landed after the 10-24 derivation.** [`psf/black#5609`](https://github.com/psf/black/pull/5609)
  merged at 03:28:27Z by `cobaltt7`: `# fmt: skip` on an opening bracket made the second formatting pass
  lose the hidden-code marker, so at a short line length it split before the operator and emitted code it
  could not parse; `cobaltt7` replaced the branch's hand-copied fields with `Leaf#clone()` and taught
  `clone()` to carry the marker (and the line-range state), so the marker now survives the copy.
  [`inference-gateway/inference-gateway#807`](https://github.com/inference-gateway/inference-gateway/pull/807)
  merged at 03:28:27Z by `edenreich`: Cohere's `/v1/models` answers `{"models":[...]}`, but the generated
  transformer only decoded the OpenAI `{object,data}` envelope, so the listing was always empty; a
  hand-maintained transformer now decodes the native envelope and is protected by `.openapi-ignore`.
  [`bytedance/deer-flow#7442`](https://github.com/bytedance/deer-flow/pull/7442) merged at 08:16:10Z by
  `WillemJiang`: one non-finite number in `staleFactsToExtend` or a consolidation confidence failed the
  whole memory-update batch and repeated the paid call; unusable entries are now dropped or defaulted.
  [`bytedance/deer-flow#7071`](https://github.com/bytedance/deer-flow/pull/7071) merged at 08:17:16Z by
  `WillemJiang`: the timestamped output-name fallbacks collided on a coarse clock and now stay distinct.
  [`urfave/cli#2497`](https://github.com/urfave/cli/pull/2497) merged at 10:24:07Z by `Juneezee`: required
  mutually-exclusive groups were checked before a subcommand parsed the inherited flags, so a flag placed
  after the subcommand name was rejected; the check now runs at the leaf, with the help and completion
  commands skipping it as they skip required flags.
  [`gofiber/fiber#4796`](https://github.com/gofiber/fiber/pull/4796) merged at 11:24:56Z by `ReneWerner87`:
  the hostauthorization port check compared digit counts instead of the value, so `:000080` was rejected.
- **Counters.** The external set is now **436 merges across 91 repositories** (was 430 / 90), **403
  credited in 89** (was 397 / 88), the same **33 uncredited in 2** — `SihanTeng`'s list at 32 and
  `Tencent/MMKV` at 1 — and **168 open across 130** (was 151 / 116). Re-derived 2026-10-25T15:34:11Z.
  `inference-gateway` is the new credited repository: its #807 squash commit is authored by this account,
  and at **217★** it enters the long tail, which moves from 41 to 42.
- **The named table stays at 41 rows.** Nothing crosses the 2,500★ line this round; the star column was
  last re-read on 2026-10-23 rather than here.

## 2026-10-24

- **One merge landed after the 10-23 derivation.** [`free5gc/ike#28`](https://github.com/free5gc/ike/pull/28)
  merged at 2026-10-24T07:50:50Z by `tim-ywliu`: `Delete.Unmarshal` read the bytes after its 4-byte header
  in fixed 4-byte strides, and the only bound was a lower bound on the body length, so a body that was
  longer than its header declared by a number of bytes that was not a multiple of 4 read past the buffer
  and panicked. The payload is parsed from an IKE_SA_INIT, which arrives before any authentication, so a
  peer could trip it. The branch rejects a body whose SPI data is not a whole number of 4-byte words.
  `tim-ywliu` then replaced the lower-bound check with an exact length match in `1ba3258`, keeping the
  multiple-of-4 guard, and corrected his own first reading of the pair while doing it: an equality check
  does not subsume the guard, because `spiSize` 2 with one SPI is a 6-byte body that matches its header and
  still is not a whole number of words. Both commits are in `main`; the first is authored by this account,
  so the repository is credited.
- **Counters.** The external set is now **430 merges across 90 repositories** (was 429 / 89), **397
  credited in 88** (was 396 / 87), the same **33 uncredited in 2** — `SihanTeng`'s list at 32 and
  `Tencent/MMKV` at 1 — and **151 open across 116** (was 149 / 114; the three pull requests opened on
  10-23 are `kellyjonbrazil/jc#802`, `modelscope/evalscope#1937` and
  `modelcontextprotocol/go-sdk#1441`). Re-derived 2026-10-24T10:33:47Z.
- **The named table stays at 41 rows.** `free5gc/ike` is credited at **3★**, so it enters the long tail,
  which moves from 40 to 41. No row crosses the 2,500★ line this round, and the star column was last
  re-read on 2026-10-23 rather than here.

## 2026-10-23

- **Two merges landed after the 10-22 derivation.** [`ajeetdsouza/zoxide#1335`](https://github.com/ajeetdsouza/zoxide/pull/1335)
  merged at 2026-10-22T23:55:13Z by `ajeetdsouza`: a bare `z` under `_ZO_ECHO=1` called `Set-Location`
  without `-Passthru`, leaving the `$dir` assignment `$null` and throwing `PropertyNotFoundException`
  under strict mode; the no-path branch now passes `-Passthru`. `ajeetdsouza` dropped the PowerShell
  regression test from the branch before merging, so the fix lands without one.
  [`prometheus/client_golang#2179`](https://github.com/prometheus/client_golang/pull/2179) merged at
  2026-10-23T07:22:07Z by `bwplotka`: `checkMetricConsistency` compared each label name with the previous
  one before the pairs were sorted, so non-adjacent duplicates passed and a scrape of the registry was
  dropped as a whole; the sort now runs before the duplicate loop, with adjacent-control and
  non-adjacent-regression subtests.
- **Counters.** The external set is now **429 merges across 89 repositories** (was 427 / 87), **396
  credited in 87** (was 394 / 85), the same **33 uncredited in 2** — `SihanTeng`'s list at 32 and
  `Tencent/MMKV` at 1 — and **149 open across 114** (was 153 / 118). Re-derived 2026-10-23T11:36:00Z.
- **The table grows to 41 rows.** `zoxide` is credited at **40,256★**, entering between `black` and
  `fiber`; `prometheus/client_golang` at **6,043★**, between `ouroboros` and `teamai-cli`. Every star
  figure in the table was re-read this round; the largest move is `ruflo` 78,357 → 78,629. The credited
  long tail stays at 40.

## 2026-10-22 (second round)

- **One merge landed after the morning derivation.** [`uber/kraken#724`](https://github.com/uber/kraken/pull/724)
  merged at 2026-10-22T09:31:25Z by `gkeesh7`: the cache file reader opened to duplicate a committed
  upload to a replica was never handed to the server's closer set, so every replica of every uploaded blob
  leaked one file descriptor; both replication paths now close it. `sambhav-jain-16` asked for the two
  cases to be folded into one table before approving, and both commits carry this account's authorship, so
  the repository is credited rather than merely merged.
- **Counters.** The external set is now **427 merges across 87 repositories** (was 426 / 86), **394 credited
  in 85** (was 393 / 84), the same **33 uncredited in 2** — `SihanTeng`'s list at 32 and `Tencent/MMKV` at
  1 — and **153 open across 118** (was 155 / 120; the drop is this merge and
  `raysan5/raygui#579`, closed unmerged on 2026-10-22T09:42:03Z). Re-derived 2026-10-22T13:49:01Z.
- **The table grows to 39 rows.** `uber/kraken` is credited at **6,770★**, so it enters the named table
  between `models.dev` and `koishi`. The long tail stays at **40**. Every star figure in the table was
  re-read this round, the largest move being `dsh-market/dsh-market` 8,049 → 8,186.

## 2026-10-22

- **One merge landed after the previous derivation, and it is the first one in this repository.**
  [`urfave/cli#2479`](https://github.com/urfave/cli/pull/2479) merged at 2026-10-21T15:40:14Z by
  `Juneezee`: `HandleExitCoder` found an `ExitCoder` with a bare type assertion, so an exit error
  wrapped with `fmt.Errorf("%w")` was never recognised — nothing printed, and the process exited 1
  instead of the intended code. `Juneezee` rebased it onto a `main` that now requires Go 1.26 (#2483),
  squashed the two golden-regenerating commits into the first one, and replaced the final lookup with
  `errors.AsType` before merging; issue #2478 is closed as completed. Two of the three commits carry this
  account's authorship, so the default branch holds our commits and the repository is credited rather
  than merely merged.
- **Counters.** The external set is now **426 merges across 86 repositories** (was 425 / 85), **393 credited
  in 84** (was 392 / 83), the same **33 uncredited in 2** — `SihanTeng`'s
  list at 32 and `Tencent/MMKV` at 1 — and **155 open across 120** (was 157 / 122; the drop is this merge
  and `NomicFoundation/hardhat#8723`, closed unmerged on 2026-10-21T16:57:28Z). Re-derived 2026-10-22T04:40:46Z.
- **The table grows to 38 rows.** `urfave/cli` is credited at **24,300★**, so it enters the named table
  between `laya` and `learn-harness-engineering`. The long tail stays at **40**. Every star figure in the
  table was re-read this round, the largest move being `dsh-tauri/deepseek-harness-desktop` 3,418 → 3,212.

## 2026-10-21

- **Three merges landed after the previous derivation.** [`awesome-dsh-plugin/awesome-dsh-plugin#8293`](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin/pull/8293)
  merged at 2026-10-20T17:28:17Z by `fkysly` — three more Phocinae entries in the catalogue;
  [`psf/black#5559`](https://github.com/psf/black/pull/5559) at 2026-10-20T23:06:23Z by `cobaltt7` —
  `_write_to_stdout()` translates `\n` into the platform newline itself, so the trailing-newline fixup
  appended a second one and CRLF input without a trailing newline could come out as `\r\r\n`; and
  [`valkey-io/valkey-go#210`](https://github.com/valkey-io/valkey-go/pull/210) at 2026-10-21T03:10:53Z by
  `rueian` — the client-side cache key concatenated the command name and arguments with nothing
  unambiguous between them, so `HGET k ALL` and `HGETALL k` (and `GETRANGE k 1 23` against
  `GETRANGE k 12 3`) shared one entry; each part is now length-prefixed.
- **Counters.** The external set is now **425 merges across 85 repositories** (was 422 / 83), **392 credited
  in 83** (was 389 / 81), the same **33 uncredited in 2** — `SihanTeng`'s list at 32 and `Tencent/MMKV` at
  1 — and **157 open across 122** (was 163 / 128). Re-derived 2026-10-21T13:15:05Z.
- **The table grows to 37 rows.** `psf/black` carries a commit of this account on its default branch
  (probe: one commit), so it is credited rather than merely merged, and at **41,967★** it enters the named
  table between `reactive-resume` and `fiber`. `valkey-io/valkey-go` is credited too but sits below the
  2,500★ floor and joins the long tail, which goes from 39 to **40**. Every star figure in the table was
  re-read this round, the largest move being `ruvnet/ruflo` 77,185 → 78,090.

## 2026-10-20 (second round)

- **One merge landed after the previous derivation, and it earns credit.** [`cobanov/teslamate-mcp#16`](https://github.com/cobanov/teslamate-mcp/pull/16)
  merged at 06:13:50Z by `cobanov`: on Windows asyncio installs a `ProactorEventLoop`, which `psycopg`'s async
  driver refuses, so the pool never opened a connection — every tool call failed while `/health` answered 503.
  At **140★** it sits below the 2,500★ floor, so the named table stays at 36 rows; default branch `main`
  carries one commit of this account (`defaultBranchRef.target.history(author:{id})`), so it is credited rather
  than merely merged, and the long tail below 1,000★ goes from 38 to **39**.
- **Counters.** The external set is now **422 merges across 83 repositories** (was 421 / 82), **389 credited in
  81** (was 388 / 80), the same **33 uncredited in 2** — `SihanTeng`'s list at 32 and `Tencent/MMKV` at 1, both
  unchanged — and **163 open across 128** (was 162 / 127). Re-derived 2026-10-20T11:30:20Z.

## 2026-10-20

- **Five merges landed after the 13:21Z derivation, and one of them clears the 2,500★ floor.** In time order:
  [`modelcontextprotocol/go-sdk#1409`](https://github.com/modelcontextprotocol/go-sdk/pull/1409) at 14:29:47Z
  (`--result_dir` was passed through unresolved, so `server-conformance.sh` wrote its output relative to the
  caller's cwd), [`minio/minio-go#2324`](https://github.com/minio/minio-go/pull/2324) at 15:01:25Z — the pull
  request the previous round recorded as *approved by `klauspost` at 11:10Z and still open*, merged by him
  four hours later: `RemoveObjects` reported one error for a whole batch and hid which object had failed, it
  now reports one result per failed object —
  [`awesome-dsh-plugin/awesome-dsh-plugin#8114`](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin/pull/8114)
  at 17:22:16Z, [`ruvnet/ruflo#4275`](https://github.com/ruvnet/ruflo/pull/4275) at 18:51:06Z (command examples
  in the user guide that fail when copied verbatim), and
  [`kriszyp/msgpackr#206`](https://github.com/kriszyp/msgpackr/pull/206) at 22:06:16Z, merged by `kriszyp`
  himself: `toJSON` was honoured on `Map` subclasses but not on `Set` subclasses.
- **Counters.** The external set is now **421 merges across 82 repositories** (was 416 / 80), **388 credited
  in 80** (was 383 / 78), the same **33 uncredited in 2** — `SihanTeng`'s list at 32 and `Tencent/MMKV` at 1,
  both unchanged — and **162 open across 127**, which is where it stood yesterday at the same reading; five
  merges and five new pull requests cancelled out exactly.
- **The table grows to 36 rows.** `minio/minio-go` carries a commit of this account on `master` (probe: one
  commit), so it is credited rather than merely merged, and at **3,008★** it enters the named table between
  `fastmcp` and `open5gs` and is the sixteenth entry in the brief list. `kriszyp/msgpackr` at **694★** is
  below the floor and joins the long tail, which goes from 37 to **38**; every star figure in the table was
  re-read this round, the largest move being `ruvnet/ruflo` 76,850 → 77,185.

---

## 2026-10-19

- **Four merges landed after the 12:09Z derivation, so the counters moved again.** Three catalog pull requests
  into `imsai-sh/awesome-deepseek-harness-plugins` (#639 `dsh-aqua-input-check`, #640 `dsh-customs-doc-check`,
  #641 `dsh-evidence-check`, all squash-merged by the repository's auto-merge bot at 13:03-13:04Z — that
  repository has now taken **44** merges of ours, was 41) and [`nuxt/content#3886`](https://github.com/nuxt/content/pull/3886),
  merged by `farnabaz` at 12:27:29Z with an approval fifteen seconds earlier: `generateItemSurround` dropped
  the previous item whenever `before` was larger than the item's index instead of returning a shorter window.
  The external set is now **416 merges across 80 repositories** (was 412 / 79), **383 credited in 78** (was
  379 / 77), the same **33 uncredited in 2**, and **162 open across 127** (the open repository count fell by
  one). `nuxt/content` is above the 2,500★ floor and joins the named table at **3,672★**, between
  `DSH-better-sidebar` and `evalscope`.
- **Two items in the same mailbox needed no action, and one is a decision.** `redis/node-redis#3521` was
  **closed, not merged**: the maintainer passed because nobody has reported a `__proto__` map key in practice
  and the patch only covered some of the paths that build objects from replies, leaving the behaviour
  inconsistent — the point is fair and the change is not to be re-proposed without a real report. And
  `minio/minio-go#2324` is **approved by `klauspost` at 11:10Z and still open**; it stays in the open count
  and is not to be bumped. `omdsh-dev/dsh-browser#120` is a third-party fork announcing that it imported our
  still-open `#99` into `graydovee/dsh-browser` as their `#11` — informational, no reply needed.
- **dshfind re-read, and the old sentence was wrong on both counts.** The page said *38.5k+ across the 8
  family plugins it has a figure for*. dshfind's own sitemap shards list **106** of the family's
  repositories (106 `…/plugins/PerryLink/<repo>` URLs, each in four locales), and its per-plugin badge
  endpoint — `/api/badge/PerryLink/<repo>?metric=downloads`, the `<img>` every plugin page embeds — returns
  a download tier for **9** of them: three at 10k+, two at 5k+, one at 2k+, two at 1k+ and one at 500+, which
  add to **44,500+**. The other 97 badges fall back to ★. The page now states the figure with its denominator
  and its floor, and the nine tiers are listed in `PROJECTS.md`. Note that dshfind's counter is *not* the
  same thing as npm's 30-day window: `dsh-auto-review` reads 10k+ there against 6,293 in the npm window, so
  no cross-check between the two is claimed.
- **Counters re-measured 2026-10-19T12:09Z; the badge row rebuilt around them.** `Tencent/MMKV#1697` merged at
  10:35Z into `dev`, so the external set is **412 merges across 79 repositories** (was 411 / 78), of which
  **379 are credited in 77 repositories** and **33 are not: 32 in SihanTeng's list and 1 in MMKV**, whose merge
  sits on `dev` rather than the default branch `master`; **162 are open across 128** (was 163 / 129). npm was
  re-measured through registry search, which now enumerates the whole account instead of 47 names: **107 names,
  1,601 versions, 95 carrying a SLSA provenance attestation on at least one version (75 on the current
  `latest`)**, and **228,164 downloads** for 2026-09-19..2026-10-18 (was 241,207 for 09-14..10-13). The plugin
  index serves **114 pages** (53 checkers, 44 plugins and a Chinese section, per its sitemap) and the Market
  catalogue carries **99 packages**, generated 2026-10-18. `Tencent/MMKV` joins the named table at 18,763★ and
  every other row's ★ was re-read; the six flagship rows move to 234 / 213 / 214 / 138 / 126 / 77. The badge row
  grows from 15 to **22** — the account-level badges upstream merges, credited repositories, checkers and npm
  provenance are new — and the one-command install block leaves the page.
- **The page is split in two: a front page and a full record.** The README keeps the badges, the six
  flagship plugins, every external repository above 2,500★ and a short retired/frozen note; the long form
  moved into `PROJECTS.md`, which the page links — the star table with its per-row merge narrative, the
  seven repositories between 1,000★ and 2,500★, the derivation of the 411, the `laya` ledger, the
  `deepseek-ai` picture, the 94-row roster, the retired and frozen tables and the npm figures with their
  caveats. **No figure changed and nothing was deleted**: every moved line is a verbatim slice. Merge dates
  leave the front page and stay in `PROJECTS.md`. 69,028 B → 21,680 B; the star table now names each
  project's owner and nothing else.
- **Live counters re-measured 2026-10-19T10:20:41Z; the named table now stops at 2,500★.** The external
  contributor set reads **77 repositories carrying at least one merged pull request of ours and a commit on
  the default branch, 379 merges inside those 77** (was 72 / 373); **411 merged outside `PerryLink/*`
  across 78 repositories** (was 405 / 73); a further **163 are open across 129 repositories** (was 161 /
  127). Four repositories joined the named tables with the six merges that arrived since the 00:41Z
  derivation: [`gofiber/fiber#4778`](https://github.com/gofiber/fiber/pull/4778),
  [`redis/ioredis#2233`](https://github.com/redis/ioredis/pull/2233),
  [`modelscope/evalscope#1877`](https://github.com/modelscope/evalscope/pull/1877) and
  [`weibocom/nginx-upsync-module#332`](https://github.com/weibocom/nginx-upsync-module/pull/332).
- **The individually named table starts at 2,500★, not 1,000★.** Thirty-three rows measure 2,500★ or more
  (the smallest is 2,660★); the seven repositories between 1,000★ and 2,500★ moved into the fold directly
  beneath it, one line each; the long tail below 1,000★ is 37. No repository left the contributor set —
  the split across the three tiers moved, the total did not.
- **The compliance-checker table moved inside the family fold.** It is no longer a separately expanded
  section under *The rest of the family*: the 53 rows keep their place at the end of the same fold as the
  nine category tables, and every roster figure is unchanged.

- **Live counters re-measured 2026-10-19T00:41:22Z.** The external contributor set reads **72 repositories
  carrying at least one merged pull request of ours and a commit on the default branch, 373 merges inside
  those 72** (was 69 / 369); **405 merged outside `PerryLink/*` across 73 repositories** (was 402 / 71); a
  further **161 are open across 127 repositories** (was 157 / 124). Three merges arrived since the last
  derivation: [`pydantic/pydantic-extra-types#453`](https://github.com/pydantic/pydantic-extra-types/pull/453),
  [`microsoft/SkillOpt#302`](https://github.com/microsoft/SkillOpt/pull/302), and
  [`awesome-dsh-plugin#7183`](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin/pull/7183), whose
  repository was already in the table, so it adds a merge but no row.
- **`kellyjonbrazil/jc` now earns credit, so its counter-example is retired.** `#783` still merged into
  `dev`, but `master` fast-forwarded to `7e67daf2` on 2026-10-18T20:39:02Z and
  `GET /compare/dev...master` returns `ahead_by: 1`, `behind_by: 0`; `b6f93354` is reachable from the
  default branch and `defaultBranchRef.target.history(author:{id})` returns **1** (was 0).
  `INSTRUMENTATION.md` records the retirement beside the DSH-better-sidebar precedent, which leaves
  `SihanTeng`'s list as the only counter-example.
- **Two rows joined the star table, one joined the long tail.** `microsoft/SkillOpt` measures **18,537★**
  and is the Microsoft row; `kellyjonbrazil/jc` measures **8,694★** and enters the table now that it is
  credited rather than in spite of it; `pydantic/pydantic-extra-types` measures **339★**, below the line,
  so it is named in the aggregate instead. The table is **36 rows** and the long tail **36 repositories**
  (72 credited − 36 named). Every star value was re-measured the same day and the rows are strictly
  descending, the smallest at 1,057★.

## 2026-10-18

- **Live counters re-measured 2026-10-18T12:42:47Z.** The external contributor set reads **69 repositories
  carrying at least one merged pull request of ours and a commit on the default branch, 369 merges inside
  those 69** (was 67 / 364); **402 merged outside `PerryLink/*` across 71 repositories** (was 396 / 68); a
  further **157 are open across 124 repositories** (was 124 across 91). Six merges arrived since the last
  derivation: [`v-modal/awesome-jev-tools#52`](https://github.com/v-modal/awesome-jev-tools/pull/52), a
  catalog, so it joins the aggregate bucket instead of the table;
  [`punkpeye/mcp-remote#381`](https://github.com/punkpeye/mcp-remote/pull/381);
  [`punkpeye/fastmcp#439`](https://github.com/punkpeye/fastmcp/pull/439);
  [`open5gs/open5gs#4880`](https://github.com/open5gs/open5gs/pull/4880);
  [`agentclientprotocol/python-sdk#167`](https://github.com/agentclientprotocol/python-sdk/pull/167); and
  [`kellyjonbrazil/jc#783`](https://github.com/kellyjonbrazil/jc/pull/783), which earns nothing — see the
  next bullet. The 69 was derived twice, once from the commit-author list probed per repository and once
  with the `defaultBranchRef.target.history(author:{id})` probe this file records as authoritative; the
  two agree on all 71 repositories.
- **A merge is credited only where it lands.** `kellyjonbrazil/jc#783` merged 2026-10-17T21:51:22Z into
  the project's **`dev`** branch, while its default branch is **`master`**; `master` carries no commit of
  this account, so the merge earns no credit even though the commit is authored by this account. This is
  the first counter-example about *where* a merge landed rather than about the repository withholding
  credit, and it now sits in `INSTRUMENTATION.md` beside `SihanTeng`'s.
- **`punkpeye/mcp-remote` is the 34th row above a thousand stars** (1,632★), added this round; every star
  value in the table was re-measured the same day, and 28 of the 33 existing rows moved.
- **One earlier counter-example retired.** `omdsh-dev/DSH-better-sidebar` was recorded in
  `INSTRUMENTATION.md` as having merged once without a commit of ours on `main`; re-probed 2026-10-18,
  `main` carries **1** such commit, which is why the row is in the star table at all. The entry was
  removed rather than left to age.

## 2026-10-17

- **Live counters re-measured 2026-10-17T13:21:42Z.** The external contributor set reads **67 repositories
  carrying at least one merged pull request of ours, 364 merges inside those 67** (was 66 / 360), and
  **396 merged outside `PerryLink/*` across 68 repositories** (was 392 / 67); a further **124 are open
  across 91 repositories** (was 136 across 88). Four merges arrived since the last derivation:
  [`yibie/awesome-autoresearch#11`](https://github.com/yibie/awesome-autoresearch/pull/11), merged
  2026-10-17T08:38:41Z by `yibie`, which is the **67th** repository — a 783★ catalog, so it joins the
  aggregate bucket rather than the table — and three more in
  [`awesome-dsh-plugin/awesome-dsh-plugin`](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin), which
  takes that row from 44 merges to 47 and was already in the table.
- **Every star value re-measured 2026-10-17T13:21:42Z.** 27 of the 33 rows moved; the largest were
  `ruvnet/ruflo` +348, `dsh-market` +130 and `walkinglabs/learn-harness-engineering` +122. One row fell:
  `NVIDIA/NeMo-Agent-Toolkit` 2,661 -> 2,659. The set of rows did not change — no repository crossed the
  thousand-star line and none fell below it.
- **The `deepseek-ai` org reads 22 pull requests opened, 1 merged, 15 open** (was 20 / 1 / 14). The open
  fifteen sit in eleven repositories: TileKernels three, DeepEP and deepseek-recipe two each, and one
  apiece in FlashMLA, DeepGEMM, 3FS, DeepSeek-MoE, DeepSeek-Prover-V1.5, DeepJIT and DeepSelect; fourteen
  of the fifteen are code fixes and the fifteenth a catalog addition.
- **The README no longer carries round narratives.** The five that were still inline — two of which were
  duplicates of rounds already recorded here — moved into this file, per the rule at its top.

## 2026-10-16

- **One row was added in the round to 2026-10-16**:
  `modelcontextprotocol/go-sdk`, whose merge landed 2026-10-16T08:56:34Z. Four merges arrived in that window and
  the table moves by one row, because the other three are in repositories it already carries. The new row is also
  what moved the credited count, from 64 to 66. **One row was replaced in this
  round**: the account had been listed under `Anil-matcha/awesome-vibecoded-saas`, which holds no merged pull
  request of ours at all and has since fallen to 8 stars, while the catalog the merge actually belongs to is
  `Anil-matcha/awesome-agent-apis` (1,056★, one merged pull request, and a commit of ours on its `main`). Both
  are by the same maintainer, which is how the substitution went unnoticed.

## 2026-10-15

- **The round to 2026-10-15T10:14:33Z added three merges, all of them upstream fixes in this list already.**
  Four pull requests in [`cordiverse/cordis`](https://github.com/cordiverse/cordis) were merged by its maintainer
  Shigma on 2026-10-14 — [`#198`](https://github.com/cordiverse/cordis/pull/198) at 05:17:57Z, [`#200`](
  https://github.com/cordiverse/cordis/pull/200) at 05:52:37Z, [`#197`](
  https://github.com/cordiverse/cordis/pull/197) at 06:30:51Z and [`#199`](
  https://github.com/cordiverse/cordis/pull/199) at 08:28:26Z — and `#197` is the one that closes a Windows
  defect. Two of them had already landed before the previous snapshot was taken, which is why the totals move by
  three rather than by four. The merged commits are authored by this account (GitHub's web flow is the committer),
  so `cordis` now carries five commits of ours on its default branch rather than one. One of them was retitled on
  merge: `#199` went in as `feat(create)` rather than the `fix(create)` it was opened as.

  **#2556 was closed, which is why the open count moved down by one in the same round.** That pull request made
  the oracle harness survive an exception whose every rendering path raises; `f24672de` (2026-10-14T10:02:16Z)
  landed the same fix upstream and closed #2555 with it, so the pull request was redundant rather than wrong. The
  two hostile-exception cases it added were re-run against current `main` before closing and both are decided
  there. Its branch was also in conflict with `main` over the region `UNRENDERABLE` was added to.

## 2026-10-14

- **Live counters re-measured 2026-10-14 except where a line says otherwise.** The family reads **97 in the
  roster / 89 actively maintained** (was 95 / 87): two repositories that declare `dsh.bundle.patch` were not in
  the last derivation — `dsh-phocinae`, which belongs to the separate Phocinae product line, and `dsh-phone-inbox`,
  which was created 2026-10-13. The npm surface reads **110 names / 1,446 versions / 102 non-deprecated `latest` /
  93 of those with SLSA provenance** (was 52 / 1,069 / 44 / 39) and the trailing-30-day aggregate **241,207** over
  the window 09-14..10-13 (was 183,886 over 09-07..10-06). The scope did not change; the 53 compliance checkers,
  published 2026-10-08, were simply not in the name list the earlier figures were summed from, and all 110 names
  were re-proved owned from `registry.npmjs.org`'s own `maintainers` field rather than inferred from a repository URL.
- **The round to 2026-10-14T04:13:17Z had already taken the merged count from 346 to 351.** Five merges, four of
  them in repositories the section already carries: [`Q00/ouroboros#2544`](https://github.com/Q00/ouroboros/pull/2544),
  merged 2026-10-14T01:45:29Z by `lee3Q` after the repository's own review agent had approved it;
  [`vvlife/awesome-deepseek-harness-plugins` #164](https://github.com/vvlife/awesome-deepseek-harness-plugins/pull/164)
  and its [#163](https://github.com/vvlife/awesome-deepseek-harness-plugins/pull/163), merged 2026-10-14T02:57:53Z and
  2026-10-13T17:37:30Z; and two catalogue entries, [`yibie/awesome-jev#368`](https://github.com/yibie/awesome-jev/pull/368)
  and [`cobanov/awesome-jev#160`](https://github.com/cobanov/awesome-jev/pull/160). None crossed the thousand-star
  line, so the table kept 32 rows and only the totals moved. The commit that credits `Q00/ouroboros` is the change
  itself, authored by this account and committed by GitHub's web flow on the squash.
- **The merged set moved from 351 to 353.** [`NandhaKishorM/laya#1179`](https://github.com/NandhaKishorM/laya/pull/1179)
  merged 2026-10-14T04:57:15Z, taking the `laya` ledger to **47 merged of the 51 opened**;
  [`cordiverse/cordis#198`](https://github.com/cordiverse/cordis/pull/198) merged 2026-10-14T05:17:57Z, so the kernel
  DeepSeek Harness vendors holds two merged pull requests of ours rather than one. The credited set moved **64 → 66**
  for a different reason: this derivation probed further and found
  [`zcx960/deepseek-desktop`](https://github.com/zcx960/deepseek-desktop) and — from the round before —
  [`Phocinae/phocinae-server`](https://github.com/Phocinae/phocinae-server) each carrying a commit of this account and
  **no pull request ever opened**, which is the one shape the merged-PR search cannot see.
- **Six repositories were excluded from the credited set after a probe, and this is the rule to reuse.** The commit
  search returns `jersonboydmilan/Laya`, `jetmiyoung/laya`, `tgundhus/laya-pro`,
  `xinglunxu76-star/awesome-dsh-plugin-deepseek-harness-` and two further re-uploads as carrying commits of this account. They are
  not forks, so no flag marks them, but every one of the commits is **byte-identical** to a commit on the upstream
  project it is named after (`POST /repos/{upstream}/commits/{sha}` returns 200 for `4bae1b32`, `c807d5de`,
  `b9e06613` and the rest). Counting them would add six repositories whose "our commits" were done elsewhere, which is
  the same padding the counter-examples exist to prevent.
- **Versions worth opening this round:** `dsh-plugin-guide` **0.3.33** / `0.3.32` / `0.3.31` (three releases in
  twenty-five minutes on 2026-10-13), `dsh-phone-inbox` **0.1.1** (its first published release), `dsh-memento`
  **0.5.25**. The badge row keeps its 21 badges in four rows and only three values moved, so its partition is unchanged.

## 2026-10-13

- **One merge arrived and nothing else moved.** [`pan17/dsh-wechat#11`](https://github.com/pan17/dsh-wechat/pull/11)
  merged 2026-10-13T11:51:58Z by the maintainer `pan17`: 29 files, a plugin-side feature release rather than a
  listing entry, and the repository was already credited and already above the thousand-star line.
- **One repository crossed the thousand-star line, which is what puts a row in the table.**
  [`open5gs/open5gs`](https://github.com/open5gs/open5gs) merged
  [#4848](https://github.com/open5gs/open5gs/pull/4848) on 2026-10-13T12:42:52Z — two files, `+2/-2`, by its
  maintainer `acetcom`, building the `tel` IMPU in canonical form — and at **2,758★** it is named individually from
  that round on. The table went from 31 rows to 32.
- **Re-derived 2026-10-13T12:37Z: 345 merges inside the credited set, 377 outside `PerryLink/*`, 116 open.** The
  profile repository itself was pushed three times that day; the round text below is what those commits wrote.

## 2026-10-12

- **Seven merges arrived, three of them new rows.** The derivation before this one was dated 2026-10-09T04:16Z and
  this one was taken 2026-10-12T10:37:23Z. The new rows are `txtai`, `models.dev` and `DSH-better-sidebar`; the first
  two clear a thousand stars, and the third is a promotion — `omdsh-dev/DSH-better-sidebar` had been carried as
  *excluded* because it took [a merge](https://github.com/omdsh-dev/DSH-better-sidebar/pull/843) on 2026-10-04 while
  crediting no commit of ours, and it now carries one (`docs(catalog)` on `main`, authored under the account's public
  address rather than its `noreply` one). Below a thousand stars, the merges were
  `agentclientprotocol/python-sdk`, which credited that repository and took two of our pull requests in one morning,
  and `8treenet/goraven`, one.
- **The star table's cells were re-measured, not carried forward**, and every row added since 2026-10-07 entered on
  the merge that reached a default branch rather than on a remembered case.

## 2026-10-09

- **The Phocinae section's figures moved to the v1.1 re-measurement, and every figure site moved with them.** The model project re-ran its release benchmark set on 2026-10-09 on the v1.1 weights, so the section's figures now read: GPU fp16 p50 **21.0 ms (RTX 5090)** per decision (was 18.6 ms), CPU single-thread **1.64 s/case** (was ~1.5 s), typed-decisions **0.906 en / 0.848 zh** (was 0.797 / 0.789; zh is machine-translated cases), option-order flip **rev150 0.0200 · rev400 0.0217** (was rev 0.0300), shipped-column ECE **0.2519** (was 0.1313), and the τ=0.6 escalate gate — **45.0% escalate, −55.0% LLM calls (79.6% at τ=0.5), kept-subset accuracy 0.9936** (was 45.7% / −54.4% / 82.8% / 0.886). JevBench now reads **0.5455 (126/231)** (was 0.5108, 118/231) and still stays below the 58.4% gate, published as-is. The 2026-10-08 round above keeps its dated figures; the correction is this round's, and the README § Phocinae and `INSTRUMENTATION.md`'s value table now carry the v1.1 set.

- **Two merges arrived after the previous round and one of them is a new row.**
  [koishijs/koishi#1554](https://github.com/koishijs/koishi/pull/1554) merged 2026-10-08T12:13:06Z at 6,248★ —
  the first `koishijs` row on the page and the largest row added since `bytedance/deer-flow`. The maintainer
  `shigma` reviewed it, found that a remainder after `$( … )` containing a newline was being dropped
  (`Argv.parse('echo $(echo foo)\nbar')` lost a token), pushed his own fix onto the branch as `aba416f`, and
  merged with it; the row therefore rests on a squash commit authored by this account and co-authored by him
  (`97d5c395`). This round verified his fix independently before replying: over 63 inputs at three revisions
  the account's own commit was 23/63 away from `master` and his was 5/63, all five being the element shapes
  the pull request exists to change, and his own six regression cases fail 4/6 without it.
  [OmniJev/awesome-jev-gallery#33](https://github.com/OmniJev/awesome-jev-gallery/pull/33) merged
  2026-10-08T13:22:47Z at 500★ and credits a repository without entering the table.
- **The `satori#420` closure did not hold, the maintainer agreed, and the backport was re-cut.** The closure
  cited cherry-pick `b228a0a6`, which carries #422 and does not touch the file #420 changes; `v4`'s
  `utils.ts` still had no `.slice(0, 25)` and the published `@satorijs/adapter-discord@4.6.2` names a
  `gitHead` that predates it. `shigma` replied "You are right" on 2026-10-08T12:34:03Z and cherry-picked
  #409 onto `v4` as `7606a0c3`, which now carries both caps. The pull request stays closed unmerged and is
  counted as closed, so no merge figure moves — a correction that changes what ships without changing what
  this page counts, which is the distinction the attribution rule is for.
- **Re-derived 2026-10-09T04:16Z: 56 external repositories carry a commit of ours on the default branch
  together with at least one merge** (was 54), **holding 332 merges** (was 330). The two repositories that
  took merges without crediting a commit still hold 33, so the total outside `PerryLink/*` is **365 merged,
  concentrated in 58 repositories**, with **102 open across 65**. **28 rows now clear a thousand stars**, up
  from 27, and all 28 star cells were re-measured rather than carried forward.
- **The largest table candidate this account has is not on the table, and this is why.**
  [AiHubCN/Awesome-Chinese-LLM#130](https://github.com/AiHubCN/Awesome-Chinese-LLM/pull/130) sits in a
  22,769★ repository, which would be the fourth-largest row on the page — and it is an **open proposal**, so
  the section above excludes it. The repository has had no push since 2026-05-10, its only two comments are
  out-of-office mail auto-replies, and `defaultBranchRef.target.history(author:{id})` returns 0. Recorded
  here so that a later round does not have to re-derive why a 22.7k★ repository is missing.

## 2026-10-08

- **The family grew by 53 compliance checkers, and every count on the page moved with it.** The plugins
  were written 2026-10-06/07 in a second workspace (`D:\Projects\dsh-plugins`, disjoint from
  `D:\Projects\dsh\plugins`) and published today, so the page had been describing a family a third of its
  actual size. They declare `dsh.bundle.patch` like every other roster entry, which is this page's own
  membership rule, so they count: **86 actively maintained** (was 33), **95 in the roster** (was 42),
  **94 rows in the category tables** (was 41), **100 PerryLink-owned** (was 47), **101 repos named**
  (was 48), **159 non-fork repos owned** (was 105, measured rather than derived). They appear as a new
  `### ✅ Compliance checkers` section with a table per domain — tendering, construction, safety, medical
  records, official documents, customs, quality, research, litigation, governance.
- **They are in the roster but not in the starter pack.** A roster plugin and a plugin a one-line installer
  should pull are different sets, and until today the same file served as both. `dsh-kit/plugins.txt` now
  marks them `# opt-in`: `install-all` installs **39** specs by default and **92** with
  `-IncludeCheckers` / `--include-checkers`. The gate derives both figures and the README heading states
  both, because "the installers cover all 92" stopped being true the moment this changed. They still count
  as actively maintained — what changed is what one command installs, not what the family contains.
- **What distinguishes them, in the page's own words:** each reads one register or record set against a
  versioned rule pack and returns the differences for a human to review; none pronounces on compliance,
  liability or clinical correctness. Every rule names the clause it rests on, and a per-repo
  `check:citations` gate holds each quotation to that repo's own `rules/evidence/` record, so a rule cannot
  cite something it cannot show. 19 quoted segments across 4 repos are still not traceable and are recorded
  as open debt rather than quietly dropped — the blockers are an anti-scraping 412 from the health
  commission's sites, a 63-page scan with no text layer, a standard whose text sits behind a viewer, and a
  publisher-only standard.

- **A fourth merge landed five hours after this round was first derived, and it credits a repository
  without adding a row.**
  [koishijs/koishi-plugin-adapter-onebot#82](https://github.com/koishijs/koishi-plugin-adapter-onebot/pull/82)
  — "don't send an Authorization header without a token" — was merged 2026-10-08T02:12:22Z with an approving
  review, twenty-eight days after it was opened on 2026-09-10. The repository is 51★, so it moves the
  contributor figures and not the star table: **52 credited repositories, 328 merges inside them, 361 merged
  outside `PerryLink/*` across 54 repositories, 100 open across 63, and 25 further repositories below the
  threshold** — was 51 / 327 / 360 / 53 / 101 / 64 / 24. The table stays at 27 rows.
- **The upstream section was re-derived twelve hours after the 2026-10-07 round, and one more company row
  entered the table.** Re-derived 2026-10-08: **51 external repositories carry a commit of ours on the
  default branch together with at least one merge** (was 49), **holding 327 merges** (was 324). The two
  repositories that took merges without crediting a commit still hold 33, so the total outside
  `PerryLink/*` is **360 merged, concentrated in 53 repositories**, with **101 open across 64** and 187
  closed unmerged. **27 rows now clear a thousand stars**, up from 26.

- **`NVIDIA/NeMo-Agent-Toolkit` (2,660★) is the new row and the first NVIDIA row this page has carried.**
  [#2293](https://github.com/NVIDIA/NeMo-Agent-Toolkit/pull/2293) — making `remove_r1_think_tags` actually
  remove think blocks — was merged 2026-10-08T00:10:02Z by NVIDIA's `rapids-bot` after maintainer
  `willkill07` issued `/merge`, and `develop`, the default branch, carries our squash commit `701454cf`. It
  took eleven comments and three further commits from this account after the first review, including moving
  the lone-`</think>` rule out of the shared helper and restoring the extractor contract. That review also
  produced a finding on someone else's pull request in the same repository:
  [#2286](https://github.com/NVIDIA/NeMo-Agent-Toolkit/pull/2286) was authored by `MohammedAlkindi`, not by
  this account, so it is **not** one of our merges and is not counted as one — the enum case this account
  reported in a comment there was confirmed and fixed by its author, which is a review contribution and not
  a merge.

- **`satorijs/satori` is credited on one branch and not on the other, and the page now says which.**
  [#422](https://github.com/satorijs/satori/pull/422) merged into `main` on 2026-10-07T14:55:26Z and is what
  credits the repository; [#421](https://github.com/satorijs/satori/pull/421) merged thirteen minutes later
  into the `v4` branch, which is not the default branch, so it credits nothing on its own. Both count in the
  merged total and the repository is named on the merge that reaches `main`. This is the first case in this
  set where one repository's merges land on two branches with different standing under the attribution rule.

- **The GitHub web editor changed one cell between the two rounds, and the re-derivation preserved it.** The
  `deer-flow` owner cell now reads **字节跳动 ByteDance**, matching the `**腾讯 Tencent**` rows, instead of
  the bare English name this account's own commit had written. This round rebuilds the star table
  mechanically from the measurement and asserts that edit is still present before writing, so a later
  re-derivation cannot silently drop it.

- **Star counts were re-measured with everything else** (2026-10-08) rather than carried forward: `laya`
  31,443, `deer-flow` 83,475, `ruflo` 74,072 and `NVIDIA/NeMo-Agent-Toolkit` 2,660 are this round's
  figures, and the previous round's numbers are left in that round where they belong.

- **A Phocinae section opened on the page — a second, model-sized line of work beyond the DSH family.** [Phocinae-Largha-150M-v1](https://github.com/Phocinae/Phocinae-Largha-150M-v1) is published (GitHub + Hugging Face + ModelScope, Apache-2.0). The section's figures are the release benchmark set, measured 2026-10-07: GPU 18.6 ms p50, CPU-only ~1.5 s, typed-decisions 0.797 en / 0.789 zh (machine-translated set), option-order flip rev 0.0300, shipped-column ECE 0.1313, and the τ=0.6 escalate gate — measured 45.7% escalate, −54.4% LLM calls (82.8% at τ=0.5), kept-subset accuracy 0.886 (figures re-verified 2026-10-08; the originally published 82%/0.7948 pairing was wrong). JevBench 0.5108 (118/231) stays below the 58.4% gate and is published as-is. Companion packages `phocinae-server` (PyPI), `dsh-phocinae` (npm) and `phocinae-guard` (npm) went out with it.

- **Two more merges landed after that bullet, and both credit a repository below the star threshold.**
  Re-derived 2026-10-08T08:52Z: **54 external repositories carry a commit of ours on the default branch
  together with at least one merge** (was 52), **holding 330 merges** (was 328). The two repositories that
  took merges without crediting a commit still hold 33, so the total outside `PerryLink/*` is **363 merged,
  concentrated in 56 repositories**, with **97 open across 61** and **188 closed unmerged**. The table stays
  at 27 rows. [satorijs/boilerplate#2](https://github.com/satorijs/boilerplate/pull/2) — a one-line CI fix
  merged 2026-10-08T07:09:11Z and opened 2026-09-19 — is the smallest repository this account is credited
  in, at 2★; [koishijs/docs#210](https://github.com/koishijs/docs/pull/210), merged 2026-10-08T07:44:12Z,
  is the most recent merge this account has anywhere, at 27★. The round also closed one proposal unmerged:
  [satorijs/satori#420](https://github.com/satorijs/satori/pull/420), approved 2026-10-07 and closed
  2026-10-08T07:26:38Z as superseded by a cherry-pick onto the `v4` branch. It is counted as closed and not
  as merged, which is what the repository's own record says; a comment on the pull request notes that the
  cited commit `b228a0a6` carries [#422](https://github.com/satorijs/satori/pull/422) and does not touch the
  file #420 changed, so whether the cap reaches `v4` is now the maintainer's call rather than an assumption
  this page makes.
- **`laya` closed its last open proposal, so its ledger reads 46 merged of 50 opened, 0 open, 4 closed.**
  [#943](https://github.com/NandhaKishorM/laya/pull/943) was closed unmerged at 2026-10-05T17:28:15Z in
  favour of [#936](https://github.com/NandhaKishorM/laya/pull/936), which had landed six minutes earlier and
  additionally forwards `hooksRaise` into the `routeBatch` call, so a per-call `hooksRaise: false` reaches
  `onRoute` as well as each request's predict lifecycle. The README's laya paragraph read "1 open and 3
  closed unmerged" from 2026-10-05 until this round, and its "the same 49" was one short of the 50 the
  query returns.
- **The README was restored after a whole-file write from a stale copy reverted the family raise and
  deleted the 53-checker section.** Commit `7ccd2052d1` ("fix param audit") is +19/-138 on `README.md`,
  and of its nineteen added lines exactly one is its own change — the Phocinae paragraph. The other
  eighteen are the pre-raise text of the badge, the intro, the family summary, the counting note and the
  Chinese block, and the 138 deleted lines are the raise itself plus the entire
  `### ✅ Compliance checkers (53)` section that `02af58b556` had added twenty-four minutes earlier.
  `INSTRUMENTATION.md` and `CHANGELOG.md` were never reverted, so for two hours the page contradicted its
  own value table — the exact failure §1 of `INSTRUMENTATION.md` exists to prevent. This round keeps the
  Phocinae line, restores the raise and the section, and adds the blob-sha precondition rule to
  `INSTRUMENTATION.md` §5.
- **The counting note's roster row count was short by one and now reads 92.** The nine family tables
  carry 41 rows and the restored compliance section carries 53, so the ten tables hold 94 rows and **92
  of the 95 roster repositories** appear in them — 39 + 53 — plus `jevcore` and the third-party
  `dsh-wechat`. The raise had written 91, which sums to 93 against the same sentence's own total of 94;
  95 roster minus the three toolchain repositories named in the support list is 92, which is the figure
  the sibling clause has always used (42 − 3 = 39 before the raise).
## 2026-10-07

- **The upstream section was re-derived from this account's own merged pull requests and three company
  rows entered the table, all of them by merge inside a single day.** The attribution rule is unchanged —
  a repository counts only when its default branch carries a commit authored by this account, probed with
  `defaultBranchRef.target.history(author:{id:MDQ6VXNlcjI1NTY2NTkwMA==})`. Re-derived 2026-10-07:
  **118 external repositories have had a pull request opened against them by this account; 49 of them
  carry a commit of ours on the default branch *and* at least one merge — the same 49 that carry a commit
  at all — holding 324 merges.** The two repositories that took merges without crediting a commit still
  hold 33 (`SihanTeng/awesome-deepseek-harness-plugins` 32, `omdsh-dev/DSH-better-sidebar` 1), so the total
  outside `PerryLink/*` is **357 merged, concentrated in 51 repositories**, with **104 open across 65** and
  187 closed unmerged. **26 rows now clear a thousand stars**, up from 23.

- **The three new rows are the first ByteDance, Apple and vLLM-project rows this page has carried.**
  `bytedance/deer-flow` (83,464★) merged [#6427](https://github.com/bytedance/deer-flow/pull/6427) — a
  one-line portability fix in a blocking-IO test — on 2026-10-07T10:22:16Z by `WillemJiang`, and it is the
  largest row the table has ever held. `apple/embedding-atlas` (4,969★) merged
  [#274](https://github.com/apple/embedding-atlas/pull/274), a line-ending normalization fix in a release
  script, on 2026-10-06T16:30:51Z by `donghaoren`. `vllm-project/aibrix` (5,126★) took two —
  [#2920](https://github.com/vllm-project/aibrix/pull/2920) on 2026-10-06T16:23:08Z and
  [#2931](https://github.com/vllm-project/aibrix/pull/2931) on 2026-10-07T11:18:42Z by `googs1025`, the
  latter the most recent merge this account has anywhere. Its default branch carries **two** commits of
  ours, so the row is a contributor row rather than a single-merge one, and it is the row that moved the
  window total by four instead of three.

- **One counter-example in `INSTRUMENTATION.md` was false and has been removed rather than softened.** The
  file listed `MoonshotAI/checkpoint-engine` (1,006★) as a repository that "merged a pull request of ours
  and carries no commit of ours". Re-probed: our only pull request there,
  [#108](https://github.com/MoonshotAI/checkpoint-engine/pull/108), is **open and was never merged**
  (`state=open`, `merged=false`), and `history(author:{id})` on its default branch returns
  `totalCount: 0`. It is not a counter-example; it is an open proposal, which the page already excludes
  by a separate sentence. Two counter-examples remain, both re-confirmed at 32 and 1 merge.

- **`bytedance/deer-flow` is a fourth case of the `/contributors` false negative** — the failure mode that
  got that probe rejected in the first place. `/repos/bytedance/deer-flow/contributors` returns **no entry**
  for this account, while the default branch demonstrably carries our commit `c7b65c5c`, the squash commit
  of the merge. `apple/embedding-atlas` reads 1 on the same endpoint and `vllm-project/aibrix` reads 2, so
  the probe agrees with history on two of the three new rows and disagrees on the third. That is the whole
  argument for the history probe, restated by a fresh case instead of a remembered one.

- **Prose that counted rows moved with them, and the "most recent merge" claims were re-ordered against a
  full listing rather than memory.** The lead paragraph now says twenty-six rows and twelve of them
  company-owned or well-known-project-owned, leaving the other fourteen unchanged; `ruflo`'s cell no longer
  claims to be the largest row in the table, because it is not any more — it is the largest row not owned by
  a company. Every star figure in the table was re-measured at the same time as the counts.
## 2026-10-05

- **The whole plugin family moved to a new host line, and the numbers below were re-measured the same day.** Every one of the 42 roster plugins was re-verified against DeepSeek Harness `0.2.1-alpha.1` and re-pinned to it, then released: 39 repositories took a patch version, published to npm and cut a GitHub Release. The host's admission gate is what forced the release rather than a source change — it evaluates each `@deepseek-ai/*` peer range with `semver.satisfies(runtime, range, { includePrerelease: true })`, and every range the family shipped ended at `<0.2.0`, so the very host the plugins were being tested on refused to load them. The declared range now carries two further clauses (`|| >=0.2.0-0 <0.3.0 || >=0.2.1-0 <0.3.0`) and no older clause was dropped. Three real incompatibilities surfaced only under the gates, not in the export surfaces: `Session.append` on that line cannot stamp the `ignorable` envelope marker (so `0.2.x` prereleases have to be classified unmarked *before* the first append, or the probe itself pollutes the log), `cordis-plugin-loader` 1.0.6 dropped the failure surface `await()` had in 1.0.4 (so a loader-composition negative regression reports the downstream symptom instead of its reason — 12 repositories carried that), and `@deepseek-ai/dsh-invariants` has no `0.2.1-alpha.1` publish, which makes an exact pin to that line install-fail.

- **The two npm figures were re-derived name by name on this date, and one had been overstated by direction of drift rather than by method.** The trailing-30-day window moved one day forward (09-05..10-04) and the total reads **152,643**, against 158,593 for the 09-04..10-03 window — a decrease, and the first one this page has recorded. The same probe now sees **52 names and 951 versions**, up from 909, of which **47 carry a non-deprecated `latest`**. Provenance moved the other way, because every release in this round went out through its repository's tag-triggered workflow — but it is **39 of those 47**, not all 52; this entry claimed all 52 when it was written and the correction is recorded here rather than quietly edited. Eight names carry no provenance on any version (`jevcore`, `jevcore-dsh`, `jevcore-mcp`, `dsh-laya`, `laya-mcp`, `dsh-personal-directive`, `layacore` and `layacore-mcp`), and 44 names carry it on at least one version — so the count depends on which version is asked about, and the README states the metric alongside the figure. Reported as measured, not as a trend: the series has zero-value days and the registry's own counters lag by up to two days.

- **The attribution test the README runs on was replaced, because both cheaper probes fail in the direction that flatters the page.** `/contributors` is a computed list capped at 100 entries and it returns no entry for `yibie/awesome-jev`, whose default branch carries one of this account's commits — the 09-25 round read that false negative into the text as an uncredited merge and printed the row anyway, so it said both things at once — and `/commits?author=<login>` returns an empty array for `pan17/dsh-wechat`, whose default branch holds three commits authored by this account. The rule now runs on the probe it actually names, `defaultBranchRef.target.history` with `author:{id}`, which reads real history: **43 external repositories carry a commit of ours, 317 merges sit inside them, two further repositories took 33 of ours with no commit credited, and 20 rows clear a thousand stars.** The single repository the old probe denied and the new one confirms is `yibie/awesome-jev` (2,124★).

- **The ten days since the 09-25 measurement moved the merged count by 29, and 22 of them are one repository.** Six of the rest landed one apiece in six repositories that were not part of this set at all before — `ruvnet/ruflo`, `walkinglabs/learn-harness-engineering`, `koishijs/koishi-plugin-booru`, `2768651338/dsh-plugin-manager`, `losebird/dsh-plugin-market` and `omdsh-dev/dsh-annotation` — which is what puts the largest row in the README's table, `ruflo` at 73,842★, in a set it was not part of on 09-25. The twenty-ninth is `omdsh-dev/DSH-better-sidebar#843`, the one merge in the window that credits this account no commit. `laya` supplies 22 of the 29: all of that account's merged pull requests landed inside a nine-day run (09-21 → 09-29) except the last, `#924`, which merged 2026-10-04T17:50:19Z.

- **The probes and counters were then re-run once more against what had actually merged, and three claims did not survive.** The account is **second** among `laya`'s merged-PR authors, not third: 46 sits between `aashish254`'s 126 and `Bruce-Yii`'s 27, so "third, behind 126 and 27" was arithmetically impossible. `laya` closed out at **46 merged of 49 opened, 0 open, 3 closed unmerged** — `#925` was closed unmerged at 2026-10-04T17:54:52Z, four minutes after `#924` merged, and the README had been describing it as still open. And of the closures only `#370` was this account's own; `#416` was closed by the maintainer in favour of another contributor's `#461`.

- **The page itself was restructured on this date** — the long blocks folded into `<details>`, the round narratives moved to this file, the instrumentation notes moved to `INSTRUMENTATION.md`, and every hand-maintained figure reduced to a single authoritative site. See `INSTRUMENTATION.md` for the authoritative-value table.

- **A merge landed later the same day and moved the contributor set by one repository, so the table gained a seventh company.** `docker/docker-agent#4372` — a two-file documentation fix — was merged 2026-10-05T12:14:03Z by Docker maintainer `aheritier`, and it is now the most recent merge this account has anywhere. That is the whole of the movement: **44 external repositories carry a commit of ours, 318 merges sit inside them**, the same two repositories still hold 33 of ours with no commit credited, and **318 + 33 = 351 merged pull requests outside `PerryLink/*`, concentrated in 46 repositories, with 102 open across 64.** **Twenty-one rows now clear a thousand stars**, up from twenty, and seven of them belong to a company or a well-governed project organization rather than to an individual — Docker joins Reactive Resume, DeepSeek, cordiverse, Tencent and the ACP project that Zed and JetBrains jointly govern, which supplies two of the twenty-one.

- **The laya count above is one round stale in its last clause.** The earlier bullet in this round recorded `0 open`; `#943`, opened 2026-10-05, is open now, which makes it **46 merged of 50 opened, 1 open, 3 closed unmerged**. `#943` is the TypeScript end of the same defect `predict_batch` had on the Python side — `Router.predictBatch` was dropping the per-call `onPredictStart`, `onPredictEnd` and `hooksRaise` arguments.

## 2026-10-04

- **The page said 36 external repositories carried my work; the same probe, run under the same rule, now returns 43 — and laya has no open pull requests at all.** Every external repository this account ever opened a pull request against (106 of them) was probed again with `/contributors`: **43 carry a commit attributed to this account, 20 of them above a thousand stars**, and the merged count outside `PerryLink/*` is **348**, up from 321. Five of the thousand-star rows are new since the last measurement — `ruvnet/ruflo` (73,833★), `walkinglabs/learn-harness-engineering` (18,892★), `dsh-market/dsh-market` (5,490★), `punkpeye/fastmcp` (3,272★) and `Anil-matcha/awesome-vibecoded-saas` (1,036★) — while `yibie/awesome-jev` moved the other way, from "merged but uncredited" to a contributor row (2,120★). The correction matters more than the growth: the page had been listing **14 pull requests as still open at laya**, and reading the repository's own pull-request connection shows **47 opened, 45 merged, 2 closed unmerged, 0 open** — those fourteen merged on 09-27 and 09-29, in two batches of eight, and the section below now says so.

- **The npm figures were re-derived name by name instead of carried forward, and the page had been overstating them.** The old line read **56 names, 917 versions, 49 active, 42 with provenance**; probing the registry directly — the search index alone is not enough, since it returns 47 names and silently omits the deprecated ones — gives **52 names, 909 versions, 46 whose `latest` is not deprecated, and 44 carrying a provenance attestation on that version**. Over the trailing 30 days the account served **158,593 downloads in the npm window 09-04..10-03**, against 134,856 in 08-23..09-21. The six scoped `@perrylink/*` names and the six deliberate deprecations both re-derived unchanged.

- **The one thing in the family that moved every single day of the window was the verification artifact.** [dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) committed ten times between 09-25 and 10-04, each one `chore: refresh verified badges` rewriting `data/verified.json` (+122/-122) against the live GitHub API — a dated, machine-generated record of which repos still pass the zero-dependency R+K static gate on their current default-branch HEAD.

## 2026-09-25

- **The family moved onto the `0.1.7-rc.2` host line: 41 repositories migrated in one pass, 482 `@deepseek-ai/dsh-*` pins moved off `0.1.7-rc.1`, and 36 packages published at the new patch.** The host window `dsh-v0.1.7-rc.1..rc.2` is 346 commits with no breaking declaration, but unlike the previous window `packages/core/*` did change source this time — an optional `displayReason` on the approval decision, `Session.toolHistory()`, and a tool-registry `developer/message` — all additive, and the one genuinely removed export (`OnboardingSurface`) is referenced nowhere in the family. Admission was re-measured with the host's **own** semver under `includePrerelease`, the predicate its compatibility gate actually uses: **298 peer ranges and 38 `engines.dsh` clauses, zero repositories blocked** — so the declared ranges were deliberately left untouched, and the move is a re-verification rather than a version bump dressed up as one.

- **The sweep found a repository that had been silently left a whole host line behind — and being two lines back was hiding a real API change.** [dsh-test-drive](https://github.com/PerryLink/dsh-test-drive) was still pinned to `0.1.5-rc.2` while the rest of the family sat on `rc.1`: the previous pass rewrote by line number, its anchors did not match that file, and a refused rule was read as "not applicable" instead of a miss. Compiling it against the current line then surfaced what four intermediate lines had absorbed — `jobs.wait`/`read`/`kill` take `caller?: SessionId` where they took `Agent` (the ownership fence compares `owner.id` to the caller directly, not to `caller.id`), and `JobHooks.readOutput` is gone, replaced by the job's own ring writer. Fixed in `src/batch.ts` plus eight test call sites. The lesson is now written into the workflow that produced it: a migration driver classifies by content, never by line number, and a rule that is expected to match but does not is an error rather than a skip.

- **Verified the way that catches a plugin which loads but never starts.** Every repackaged plugin is installed into a throwaway `DSH_HOME` and **booted**, not merely composed — `--dump-config` builds the tree without mounting it, so an activation failure is invisible there. **40 of the 41 pass**, and the one that does not is a `private` data repository with no version at all, which cannot be packed in the first place. Two long-standing red gates were repaired on the way: a repository whose own self-contained check rejects absolute paths was fighting the `/tmp` in its own CI workflow, and an npm-lockfile migration that `npm install` could not resolve needed `npm update --package-lock-only` to move first. Nine repositories were deliberately left out and each is recorded with its reason — three whose host pins live on an unmerged branch, one stopped mid-cherry-pick, one third-party fork, and four with nothing to pin.
