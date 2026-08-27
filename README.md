# PerryLink · DeepSeek Harness Plugin Ecosystem

33 open-source plugins for [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness), built to one quality bar: five-language docs, CI + monthly compat gates, self-contained verification, and npm publishing with provenance. Gitee mirrors sync automatically.

## Latest — 2026-08-27 audit round

- **33/33 plugins pass the full audit**: install · load · keyless boot · reversible uninstall, all green.
- Fresh npm releases this round: `dsh-budget@0.3.1` · `dsh-checkpoint-rewind@0.6.1` · `dsh-draw@0.2.1` · `dsh-mcp-panel@0.6.1` · `dsh-output-styles@0.6.1` · `dsh-permission-rules@0.6.1` · `dsh-session-pin@0.6.1` · `dsh-talk@0.2.1`
- Republished this round: `dsh-claude-move@0.3.0` · `dsh-library@0.2.0` · `dsh-lsp-actions@0.4.0` · `dsh-background-agents@0.6.0` · `@perrylink/dsh-github@0.7.0`

## Plugin catalog

**Capability & governance**
[permission-rules](https://github.com/PerryLink/dsh-permission-rules) — declarative rules + process-level network policy · [defend](https://github.com/PerryLink/dsh-defend) — destructive-command & key-leak guard · [doublecheck](https://github.com/PerryLink/dsh-doublecheck) — grill / tdd / adversary review gates · [auto-review](https://github.com/PerryLink/dsh-auto-review) — reviewer-subagent approval answerer · [budget](https://github.com/PerryLink/dsh-budget) — metering, caps, alerts, carbon estimates · [observe](https://github.com/PerryLink/dsh-observe) — OTel/Langfuse export

**Sessions & memory**
[checkpoint-rewind](https://github.com/PerryLink/dsh-checkpoint-rewind) — git-level snapshots + one-shot rollback · [memento](https://github.com/PerryLink/dsh-memento) — memory seam with protocol conformance · [composer-history](https://github.com/PerryLink/dsh-composer-history) — history, recall & search · [session-pin](https://github.com/PerryLink/dsh-session-pin) — pin board with tags & colors · [session-sync](https://github.com/PerryLink/dsh-session-sync) — git-backed session mirroring

**Agents & workflow**
[background-agents](https://github.com/PerryLink/dsh-background-agents) — durable subagents + team rooms · [lsp-actions](https://github.com/PerryLink/dsh-lsp-actions) — LSP-powered editor actions · [github](https://github.com/PerryLink/dsh-github) — GitHub tool + Action · [claude-move](https://github.com/PerryLink/dsh-claude-move) — 4-ecosystem migration tooling

**Knowledge & research**
[library](https://github.com/PerryLink/dsh-library) — local RAG knowledge base · [data-quality](https://github.com/PerryLink/dsh-data-quality) — dataset profile/clean/verify · [fund-research](https://github.com/PerryLink/dsh-fund-research) — fund research with hash-traceable snapshots · [industry-research](https://github.com/PerryLink/dsh-industry-research) — industry/company domain pack · [research-report](https://github.com/PerryLink/dsh-research-report) — verifiable report engine

**Interface & utilities**
[draw](https://github.com/PerryLink/dsh-draw) — image generation router · [talk](https://github.com/PerryLink/dsh-talk) — voice loop (STT/TTS, speak-to-interrupt) · [mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) — MCP status panel · [output-styles](https://github.com/PerryLink/dsh-output-styles) — runtime output-style switching · [fast](https://github.com/PerryLink/dsh-fast) — performance diagnostics · [local-ai](https://github.com/PerryLink/dsh-local-ai) — Ollama provider & routing · [score](https://github.com/PerryLink/dsh-score) — plugin quality scoring · [mask](https://github.com/PerryLink/dsh-mask) — secret masking · [translate](https://github.com/PerryLink/dsh-translate) — translation & JSON repair · [test-drive](https://github.com/PerryLink/dsh-test-drive) — install smoke-test driver · [personal-directive](https://github.com/liucaimao2026/dsh-personal-directive) — directive injector with top-bar toggle (framework edition, upstream: Minglink/dsh-infinite-gen-1) · [skill-pack-security](https://github.com/PerryLink/dsh-skill-pack-security) — 8-skill security pack (zh/en) + provider

**Companion** · [plugin-guide](https://github.com/PerryLink/dsh-plugin-guide) — plugin-dev knowledge base & CLI toolkit

## Quality bar (every repo)

- Five-language READMEs (en/zh/es/pt/hi), Apache-2.0
- CI matrix + monthly compat workflow: real profile install → dump-config → keyless smoke → uninstall
- `verify:self-contained` + artifact verification + readme-sync gates
- npm provenance publishing; Gitee mirrors auto-synced

---

**中文** · 33 个 DeepSeek Harness 开源插件，统一质量门禁（五语文档 / CI+compat / 自包含校验 / provenance 发布），全部通过 2026-08-27 全量体检并发布最新版本。
