# Hi, I'm PerryLink 👋

<!-- Editing note: figures stay dated and follow INSTRUMENTATION.md; rounds go to CHANGELOG.md.
     The long upstream table lives in UPSTREAM.md; the full family index lives in FAMILY.md. -->

<p align="center">
<a href="https://github.com/PerryLink?tab=repositories"><img alt="GitHub repos" src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.github.com%2Fusers%2FPerryLink&query=%24.public_repos&label=repos&color=24292f"></a>
<a href="https://github.com/PerryLink?tab=repositories"><img alt="GitHub stars" src="https://img.shields.io/github/stars/PerryLink?label=stars&affiliations=OWNER&color=24292f"></a>
<a href="https://github.com/PerryLink?tab=followers"><img alt="GitHub followers" src="https://img.shields.io/github/followers/PerryLink?label=followers&color=24292f"></a>
<a href="./FAMILY.md"><img alt="active plugins" src="https://img.shields.io/badge/active%20plugins-126-6e7781"></a>
<a href="https://www.npmjs.com/search?q=perrylink"><img alt="npm downloads 30d" src="https://img.shields.io/badge/npm%20downloads%2030d-273.6k-cb3837?logo=npm"></a>
<a href="https://github.com/PerryLink/dsh-auto-review/blob/main/LICENSE"><img alt="license" src="https://img.shields.io/badge/license-Apache--2.0-blue"></a>
<a href="https://github.com/PerryLink/dsh-auto-review/blob/main/package.json"><img alt="node" src="https://img.shields.io/badge/node-%5E22.19%20%7C%7C%20%3E%3D24-339933?logo=node.js"></a>
<a href="https://github.com/PerryLink/dsh-auto-review/blob/main/package.json"><img alt="dsh" src="https://img.shields.io/badge/dsh-%E2%89%A50.2.1%20%3C0.3.0-4B32C3"></a>
<a href="https://perrylink.github.io/"><img alt="site" src="https://img.shields.io/badge/plugin%20index-185%20pages-0b5fff"></a>
<a href="https://api.securityscorecards.dev/projects/github.com/PerryLink/dsh-auto-review"><img alt="OpenSSF Scorecard" src="https://img.shields.io/ossf-scorecard/github.com/PerryLink/dsh-auto-review?label=openssf%20scorecard"></a>
</p>

Independent open-source developer in Beijing. I fix other people's projects and maintain a plugin family
for [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness); I am not affiliated with DeepSeek.

My work runs in three lines: **upstream fixes** (AWS, Apple, Docker, Microsoft, NVIDIA, Prometheus, Redis,
Tencent, the vLLM project, and one-person projects); the **DSH plugin family** (126 active Apache-2.0
plugins, plus the three-level standards and guides); and **[Phocinae](https://github.com/Phocinae)**, my
typed-decision model lab.

## ▶ Start here

| What | Where |
|---|---|
| **Full family index** — 149 active + 11 archived own DSH repositories, 9 groups | [FAMILY.md](./FAMILY.md) · [site page](https://perrylink.github.io/dsh-plugins/family.html) |
| **Standards & guides** — ENTRY/FLOW/BOOST, the checker, the rule text | [dsh-standards](https://github.com/PerryLink/dsh-standards) · [dsh-plugin-guide](https://github.com/PerryLink/dsh-plugin-guide) · [dsh-plugin-spec](https://github.com/PerryLink/dsh-plugin-spec) |
| **Install the mainline** — one command, 43 defaults + 53 opt-in checkers | [dsh-kit](https://github.com/PerryLink/dsh-kit) |
| **Phocinae** — local typed decisions, no text generation | [github.com/Phocinae](https://github.com/Phocinae) |

## 🧩 What I maintain

- **DSH plugin family.** 126 active Apache-2.0 plugins: 32 runtime, 62 compliance checkers (53 core +
  9 newer), 29 domain tools, 8 developer-toolchain packages, and the 7 standards/checks plus 2 guides.
  The domain tools are a task-first market: 11 task families, five scenario packs, two suites. Start at
  [FAMILY.md](./FAMILY.md) or the [market](https://perrylink.github.io/dsh-plugins/market.html).
- **Standards and guides.** Three layers, three questions: ENTRY (can it install and start), FLOW (can a
  user use it), BOOST (does it use Cordis well). [dsh-standards](https://github.com/PerryLink/dsh-standards)
  ships the checker; [dsh-plugin-spec](https://github.com/PerryLink/dsh-plugin-spec) holds the rule text;
  [dsh-plugin-guide](https://github.com/PerryLink/dsh-plugin-guide) explains the layers;
  [dsh-clinic](https://github.com/PerryLink/dsh-clinic) diagnoses installs. None is official, and none
  certifies, scores or ranks a plugin.
- **Phocinae.** A 144.3M bilingual typed-decision model (one forward pass, calibrated confidence) plus
  the local server, guard, MCP server, CLI and DSH verdict plugins. The org profile is the full map:
  [github.com/Phocinae](https://github.com/Phocinae).

## ⭐ Selected plugins

| Plugin | What it gives you |
|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | Second-model auto-review on the approval chain, fail-closed by default (247★) |
| [dsh-research-report](https://github.com/PerryLink/dsh-research-report) | Verifiable reports: content-addressed evidence ledger, manifest seal, byte-level citations (212★) |
| [dsh-industry-research](https://github.com/PerryLink/dsh-industry-research) | Industry/company research: chain map, timeline, company cards, adversarial review (216★) |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | Approval-gated cross-session memory (`ctx.memory` + SQLite) (142★) |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | Claude Code-style allow/deny/ask rules plus a process-level network policy (134★) |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | MCP management console: `/mcp`, Settings tab, trial calls (91★) |
| [dsh-phocinae](https://github.com/PerryLink/dsh-phocinae) | Local, non-generative verdicts for the approval chain with fail-closed escalation (1★) |

```sh
dsh plugin --profile web add dsh-auto-review   # or any name above
```

## 📦 Full family at a glance

| Group | What it covers | Count | Start here |
|---|---|---:|---|
| 🧭 Three-level standards & checks | ENTRY/FLOW conformance, rule text, certification, clinic, score, preflight, checker installer | 7 | [dsh-standards](https://github.com/PerryLink/dsh-standards) |
| 📘 Three-level guides | ENTRY/FLOW/BOOST guide and the practical primer | 2 | [dsh-plugin-guide](https://github.com/PerryLink/dsh-plugin-guide) |
| 🛠️ Developer toolchain | start / ready / tools / dev / scaffold / codemod / test-drive / migration | 8 | [dsh-plugin-dev](https://github.com/PerryLink/dsh-plugin-dev) |
| 🧩 Runtime plugins | security, workflow, UX, research, observability, messaging, developer experience | 32 | [taxonomy view](https://perrylink.github.io/dsh-plugins/taxonomy.html) |
| ✅ Compliance checkers | the 53-checker suite plus the newer checker/audit tools | 62 | [checker index](https://perrylink.github.io/zh/checkers/) |
| 🏢 Domain operations | finance, legal, trade, HR, construction, ESG, quality, documents | 29 | [task-first market](https://perrylink.github.io/dsh-plugins/market.html) |
| 🦭 Phocinae | server, guard, MCP, CLI, rulepack, DSH verdict plugins | 12 | [Phocinae](https://github.com/Phocinae) |
| 📦 Catalogs & install | dsh-kit, catalog, portal, family site | 5 | [dsh-kit](https://github.com/PerryLink/dsh-kit) |

The runtime/domain roster is **137 rows: 126 active, 8 frozen, 3 retired**. Standards, guides, toolchain,
Phocinae and catalogs sit outside that roster and are counted separately above. Every repository and every
retired/moved pointer is in **[FAMILY.md](./FAMILY.md)**; install scopes are in
[ROSTER.md](https://github.com/PerryLink/dsh-plugins/blob/main/ROSTER.md).

## 🔧 Upstream

**508 merged pull requests across 99 credited repositories**; 161 proposals were open across 123
repositories as of 2026-11-03. The verified list — 19 repositories above 10,000★ and 38 between 1,000★
and 10,000★, each with its owning party — is in **[UPSTREAM.md](./UPSTREAM.md)**. I also contribute to
**[Cordis](https://github.com/cordiverse/cordis)**, the plugin kernel DeepSeek Harness vendors as
`@deepseek-ai/cordis` (nine merged).

## 🌍 Where it lives

- **Source & mirrors** — [GitHub](https://github.com/PerryLink) · [Gitee](https://gitee.com/perrylink) ·
  [GitCode](https://gitcode.com/PerryLink); the `perrylink` npm account holds **180 names and 2,296
  versions**, 156 with a SLSA provenance attestation on at least one version (123 on `latest`).
- **Downloads** — **273,579 over the trailing 30 days** (2026-10-01..10-30); dshfind publishes rounded
  badges for 9 plugins that add to **45,500+**.
- **Site** — [perrylink.github.io](https://perrylink.github.io/) (185 pages, 114 in the checker tree);
  the family page is [dsh-plugins/family.html](https://perrylink.github.io/dsh-plugins/family.html).
- **DSH Desktop Market** — catalog source:
  `https://cdn.jsdelivr.net/gh/PerryLink/dsh-catalog@main/deploy/artifacts/v1/plugins.json`.
- **MCP Registry** — four servers: `dsh-cert-mcp` (frozen reference), `dsh-customs-mcp`, `jevcore-mcp`,
  `laya-mcp`.
- **GitHub Actions** — [dsh-github](https://github.com/PerryLink/dsh-github) and
  [dsh-test-drive](https://github.com/PerryLink/dsh-test-drive) ship composite actions.

## 🪦 Retired & frozen

3 retired and 8 frozen plugins. Compatibility updates stop, existing installs keep working, and no second
implementation is maintained. The linked list, with reasons, is [FAMILY.md §9](./FAMILY.md#9-frozen-moved-and-retired).

<details>
<summary><b>中文介绍</b></summary>

独立开源开发者，在北京，与 DeepSeek 无隶属关系。三条线：**给别人的项目修 bug**；**维护 DeepSeek Harness
插件家族**（126 个活跃 Apache-2.0 插件，含 62 个合规核查器、29 个业务工具，以及三级标准与指南）；**Phocinae**，
我自己的本地 typed-decision 模型与工具 org。

插件目录在 [perrylink.github.io](https://perrylink.github.io/)，完整家族与退役清单见 [FAMILY.md](./FAMILY.md)。
数字只在英文部分维护一份；上游贡献明细见 [UPSTREAM.md](./UPSTREAM.md)。

</details>

---

*Measured, not remembered.* Measurement rules: [INSTRUMENTATION.md](INSTRUMENTATION.md) · round log:
[CHANGELOG.md](CHANGELOG.md).
