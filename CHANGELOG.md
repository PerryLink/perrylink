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
