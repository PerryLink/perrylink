# The PerryLink DSH plugin family — full index

> Generated 2026-11-04 from `dsh-plugins/family.json` (137 rows: 126 active / 8 frozen / 3 retired),
> `dsh-kit` and the PerryLink/Phocinae repositories. Groups overlap where a support repo is also a
> bundle; they are an index, not a partition.

The family has three layers: **standards and guides** (how to build), **developer toolchain** (how to
ship), and **runtime/domain plugins** (what users install). Phocinae is a separate decision-model line.

## 1. Three-level standards and checks

| Repo | What it is |
|---|---|
| [dsh-standards](https://github.com/PerryLink/dsh-standards) | ENTRY/FLOW conformance checker, level audit, clause execution |
| [dsh-plugin-spec](https://github.com/PerryLink/dsh-plugin-spec) | Rule text and clause IDs (the source the checker executes) |
| [dsh-certification](https://github.com/PerryLink/dsh-certification) | Community attestation registry, scoring model and badges |
| [dsh-clinic](https://github.com/PerryLink/dsh-clinic) | Install doctor, host-surface snapshot, recovery checks |
| [dsh-score](https://github.com/PerryLink/dsh-score) | Multi-dimensional plugin quality scoring |
| [dsh-plugin-ready](https://github.com/PerryLink/dsh-plugin-ready) | Static ENTRY preflight (`dsh-ready`) |
| [dsh-check-pack](https://github.com/PerryLink/dsh-check-pack) | One-command installer for the 53-checker compliance suite |

## 2. Three-level guides

| Repo | What it is |
|---|---|
| [dsh-plugin-guide](https://github.com/PerryLink/dsh-plugin-guide) | Three-layer guide: ENTRY checks, FLOW journeys, BOOST practices |
| [dsh-primer](https://github.com/PerryLink/dsh-primer) | Practical primer + legacy build skill/CLI |

## 3. Developer toolchain

| Repo | What it is |
|---|---|
| [dsh-plugin-dev](https://github.com/PerryLink/dsh-plugin-dev) | `dsh-dev` front door: new/check/test/submit/upgrade |
| [dsh-plugin-devtools](https://github.com/PerryLink/dsh-plugin-devtools) | Umbrella for start/ready/tools/dev |
| [dsh-plugin-start](https://www.npmjs.com/package/dsh-plugin-start) | `dsh-start new` minimal skeleton (npm; source repo retired) |
| [dsh-plugin-tools](https://github.com/PerryLink/dsh-plugin-tools) | `dsh-tools list/doctor/install` |
| [dsh-scaffold](https://github.com/PerryLink/dsh-scaffold) | Shared scaffold and contracts for the family |
| [dsh-codemod](https://github.com/PerryLink/dsh-codemod) | Version-corridor migration codemods |
| [dsh-test-drive](https://github.com/PerryLink/dsh-test-drive) | Isolated install-and-smoke test drives |
| [dsh-claude-move](https://github.com/PerryLink/dsh-claude-move) | Four-source migration wizard (Claude Code/Codex/OpenCode/Hermes) |

## 4. Runtime plugins (32 active mainline rows)

| Repo | What it is | Axis |
|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | undefined | workflow |
| [dsh-checkpoint-rewind](https://github.com/PerryLink/dsh-checkpoint-rewind) | undefined | workflow |
| [dsh-click](https://github.com/PerryLink/dsh-click) | undefined | interface |
| [dsh-composer-history](https://github.com/PerryLink/dsh-composer-history) | undefined | interface |
| [dsh-data-quality](https://github.com/PerryLink/dsh-data-quality) | undefined | developer-tools |
| [dsh-doublecheck](https://github.com/PerryLink/dsh-doublecheck) | undefined | workflow |
| [dsh-fast](https://github.com/PerryLink/dsh-fast) | undefined | observability |
| [dsh-fund-research](https://github.com/PerryLink/dsh-fund-research) | undefined | research |
| [dsh-industry-research](https://github.com/PerryLink/dsh-industry-research) | undefined | research |
| [dsh-laya](https://github.com/laya-family/dsh-laya) | undefined | integrations |
| [dsh-library](https://github.com/PerryLink/dsh-library) | undefined | content |
| [dsh-local-ai](https://github.com/PerryLink/dsh-local-ai) | undefined | integrations |
| [dsh-lsp-actions](https://github.com/PerryLink/dsh-lsp-actions) | undefined | developer-tools |
| [dsh-mask](https://github.com/PerryLink/dsh-mask) | undefined | security |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | undefined | developer-tools |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | undefined | workflow |
| [dsh-observe](https://github.com/PerryLink/dsh-observe) | undefined | observability |
| [dsh-output-styles](https://github.com/PerryLink/dsh-output-styles) | undefined | interface |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | undefined | security |
| [dsh-primer](https://github.com/PerryLink/dsh-primer) | undefined | developer-tools |
| [dsh-codemod](https://github.com/PerryLink/dsh-codemod) | undefined | workflow |
| [dsh-research-report](https://github.com/PerryLink/dsh-research-report) | undefined | research |
| [dsh-score](https://github.com/PerryLink/dsh-score) | undefined | developer-tools |
| [dsh-session-sync](https://github.com/PerryLink/dsh-session-sync) | undefined | workflow |
| [dsh-talk](https://github.com/PerryLink/dsh-talk) | undefined | content |
| [dsh-test-drive](https://github.com/PerryLink/dsh-test-drive) | undefined | workflow |
| [dsh-translate](https://github.com/PerryLink/dsh-translate) | undefined | content |
| [dsh-github-bot](https://github.com/PerryLink/dsh-github-bot) | undefined | workflow |
| [dsh-clinic](https://github.com/PerryLink/dsh-clinic) | undefined | developer-tools |
| [dsh-scaffold](https://github.com/PerryLink/dsh-scaffold) | undefined | developer-tools |
| [dsh-security-pack](https://github.com/PerryLink/dsh-security-pack) | undefined | security |
| [dsh-dida](https://github.com/PerryLink/dsh-dida) | undefined | integrations |

## 5. Compliance checkers (62 active rows)

| Repo | What it is | Axis |
|---|---|---|
| [dsh-customs-doc-check](https://github.com/PerryLink/dsh-customs-doc-check) | null | compliance |
| [dsh-demurrage-ledger](https://github.com/PerryLink/dsh-demurrage-ledger) | null | compliance |
| [dsh-export-ctl-check](https://github.com/PerryLink/dsh-export-ctl-check) | null | compliance |
| [dsh-forecast-penalty](https://github.com/PerryLink/dsh-forecast-penalty) | null | compliance |
| [dsh-hs-classify](https://github.com/PerryLink/dsh-hs-classify) | null | compliance |
| [dsh-lc-doc-check](https://github.com/PerryLink/dsh-lc-doc-check) | null | compliance |
| [dsh-origin-rvc-check](https://github.com/PerryLink/dsh-origin-rvc-check) | null | compliance |
| [dsh-railway-window](https://github.com/PerryLink/dsh-railway-window) | null | compliance |
| [dsh-fmea-table-check](https://github.com/PerryLink/dsh-fmea-table-check) | null | compliance |
| [dsh-ota-review-check](https://github.com/PerryLink/dsh-ota-review-check) | null | compliance |
| [dsh-pipeline-check](https://github.com/PerryLink/dsh-pipeline-check) | null | compliance |
| [dsh-ppap-check](https://github.com/PerryLink/dsh-ppap-check) | null | compliance |
| [dsh-repair-order-qc](https://github.com/PerryLink/dsh-repair-order-qc) | null | compliance |
| [dsh-review-reply-check](https://github.com/PerryLink/dsh-review-reply-check) | null | compliance |
| [dsh-spc-gbt-adapter](https://github.com/PerryLink/dsh-spc-gbt-adapter) | null | compliance |
| [dsh-warranty-calc](https://github.com/PerryLink/dsh-warranty-calc) | null | compliance |
| [dsh-aqua-input-check](https://github.com/PerryLink/dsh-aqua-input-check) | null | compliance |
| [dsh-drill-script-check](https://github.com/PerryLink/dsh-drill-script-check) | null | compliance |
| [dsh-emergency-plan](https://github.com/PerryLink/dsh-emergency-plan) | null | compliance |
| [dsh-hazchem-check](https://github.com/PerryLink/dsh-hazchem-check) | null | compliance |
| [dsh-hidden-risk-map](https://github.com/PerryLink/dsh-hidden-risk-map) | null | compliance |
| [dsh-power-loss-split](https://github.com/PerryLink/dsh-power-loss-split) | null | compliance |
| [dsh-power-ticket-check](https://github.com/PerryLink/dsh-power-ticket-check) | null | compliance |
| [dsh-bid-ca-precheck](https://github.com/PerryLink/dsh-bid-ca-precheck) | null | compliance |
| [dsh-bid-qual-check](https://github.com/PerryLink/dsh-bid-qual-check) | null | compliance |
| [dsh-contract-stance](https://github.com/PerryLink/dsh-contract-stance) | null | compliance |
| [dsh-protest-deadline](https://github.com/PerryLink/dsh-protest-deadline) | null | compliance |
| [dsh-rulefile-check](https://github.com/PerryLink/dsh-rulefile-check) | null | compliance |
| [dsh-tender-extract](https://github.com/PerryLink/dsh-tender-extract) | null | compliance |
| [dsh-tender-matrix](https://github.com/PerryLink/dsh-tender-matrix) | null | compliance |
| [dsh-eia-guide-check](https://github.com/PerryLink/dsh-eia-guide-check) | null | compliance |
| [dsh-guard-plan-qc](https://github.com/PerryLink/dsh-guard-plan-qc) | null | compliance |
| [dsh-hazplan-check](https://github.com/PerryLink/dsh-hazplan-check) | null | compliance |
| [dsh-permit-report-check](https://github.com/PerryLink/dsh-permit-report-check) | null | compliance |
| [dsh-safety-brief-check](https://github.com/PerryLink/dsh-safety-brief-check) | null | compliance |
| [dsh-site-log-check](https://github.com/PerryLink/dsh-site-log-check) | null | compliance |
| [dsh-soilwater-check](https://github.com/PerryLink/dsh-soilwater-check) | null | compliance |
| [dsh-essay-rubric-check](https://github.com/PerryLink/dsh-essay-rubric-check) | null | compliance |
| [dsh-learning-gap-check](https://github.com/PerryLink/dsh-learning-gap-check) | null | compliance |
| [dsh-nsfc-form-check](https://github.com/PerryLink/dsh-nsfc-form-check) | null | compliance |
| [dsh-paper-doc-adapter](https://github.com/PerryLink/dsh-paper-doc-adapter) | null | compliance |
| [dsh-policy-brief-draft](https://github.com/PerryLink/dsh-policy-brief-draft) | null | compliance |
| [dsh-archive-check](https://github.com/PerryLink/dsh-archive-check) | null | compliance |
| [dsh-gongwen-flow-check](https://github.com/PerryLink/dsh-gongwen-flow-check) | null | compliance |
| [dsh-gongwen-word-check](https://github.com/PerryLink/dsh-gongwen-word-check) | null | compliance |
| [dsh-evidence-check](https://github.com/PerryLink/dsh-evidence-check) | null | compliance |
| [dsh-lawcite-adapter](https://github.com/PerryLink/dsh-lawcite-adapter) | null | compliance |
| [dsh-pleading-draft](https://github.com/PerryLink/dsh-pleading-draft) | null | compliance |
| [dsh-icd-rule-check](https://github.com/PerryLink/dsh-icd-rule-check) | null | compliance |
| [dsh-medrec-qc](https://github.com/PerryLink/dsh-medrec-qc) | null | compliance |
| [dsh-nurse-record-check](https://github.com/PerryLink/dsh-nurse-record-check) | null | compliance |
| [dsh-soe-decision-check](https://github.com/PerryLink/dsh-soe-decision-check) | null | compliance |
| [dsh-sop-sync-check](https://github.com/PerryLink/dsh-sop-sync-check) | null | compliance |
| [dsh-bid-health-check](https://github.com/PerryLink/dsh-bid-health-check) | null | compliance |
| [dsh-canteen-retention-check](https://github.com/PerryLink/dsh-canteen-retention-check) | null | compliance |
| [dsh-construction-doc-check](https://github.com/PerryLink/dsh-construction-doc-check) | null | compliance |
| [dsh-excel-reconcile](https://github.com/PerryLink/dsh-excel-reconcile) | null | data |
| [dsh-invoice-ledger](https://github.com/PerryLink/dsh-invoice-ledger) | null | compliance |
| [dsh-payroll-audit](https://github.com/PerryLink/dsh-payroll-audit) | null | compliance |
| [dsh-safety-ledger-check](https://github.com/PerryLink/dsh-safety-ledger-check) | null | compliance |
| [dsh-table-ingest](https://github.com/PerryLink/dsh-table-ingest) | null | data |
| [dsh-tender-requirements](https://github.com/PerryLink/dsh-tender-requirements) | null | business-ops |

## 6. Domain operations (29 active rows)

| Repo | What it is | Axis |
|---|---|---|
| [dsh-einvoice](https://github.com/PerryLink/dsh-einvoice) | China e-invoice (file-level) | business-ops · dsh-finops-suite |
| [dsh-bankrec](https://github.com/PerryLink/dsh-bankrec) | Bank statement reconciliation | business-ops · dsh-finops-suite |
| [dsh-ap-three-way](https://github.com/PerryLink/dsh-ap-three-way) | AP three-way match | business-ops · dsh-finops-suite |
| [dsh-travel-recon](https://github.com/PerryLink/dsh-travel-recon) | Travel reconciliation & policy check | business-ops · dsh-finops-suite |
| [dsh-legal-intake](https://github.com/PerryLink/dsh-legal-intake) | Legal request intake | business-ops · dsh-contract-suite |
| [dsh-legal-clause](https://github.com/PerryLink/dsh-legal-clause) | Contract clause & playbook review | business-ops · dsh-contract-suite |
| [dsh-ghg](https://github.com/PerryLink/dsh-ghg) | Electricity GHG (Scope 2) | business-ops |
| [dsh-qms-capa](https://github.com/PerryLink/dsh-qms-capa) | QMS NCR, CAPA & 8D | business-ops |
| [dsh-hs-candidate](https://github.com/PerryLink/dsh-hs-candidate) | HS candidate precheck | business-ops |
| [dsh-freight-audit](https://github.com/PerryLink/dsh-freight-audit) | Freight bill audit | business-ops |
| [dsh-docx-redline](https://github.com/PerryLink/dsh-docx-redline) | DOCX inspect & text diff | content |
| [dsh-ifc-qto](https://github.com/PerryLink/dsh-ifc-qto) | IFC quantity takeoff | data |
| [dsh-policy-ledger](https://github.com/PerryLink/dsh-policy-ledger) | Install doctor | developer-tools |
| [dsh-pim-lint](https://github.com/PerryLink/dsh-pim-lint) | PIM catalog lint | data |
| [dsh-eval-pack](https://github.com/PerryLink/dsh-eval-pack) | Eval pack lint & grader | developer-tools |
| [dsh-finops-suite](https://github.com/PerryLink/dsh-finops-suite) | Finance ops suite | business-ops |
| [dsh-contract-suite](https://github.com/PerryLink/dsh-contract-suite) | Contract ops suite | business-ops |
| [dsh-provider-params](https://github.com/PerryLink/dsh-provider-params) | Provider parameter mapping and JSON repair | developer-tools |
| [dsh-pdf-table](https://github.com/PerryLink/dsh-pdf-table) | PDF table extraction (text layer) | data |
| [dsh-contract-renewal](https://github.com/PerryLink/dsh-contract-renewal) | Contract renewal tracker | business-ops |
| [dsh-rfq-compare](https://github.com/PerryLink/dsh-rfq-compare) | RFQ comparison | business-ops |
| [dsh-labor-contract](https://github.com/PerryLink/dsh-labor-contract) | Labor contract check | business-ops |
| [dsh-progress-payment](https://github.com/PerryLink/dsh-progress-payment) | Progress payment audit | business-ops |
| [dsh-ar-aging](https://github.com/PerryLink/dsh-ar-aging) | AR aging | business-ops |
| [dsh-import-customs-check](https://github.com/PerryLink/dsh-import-customs-check) | Import document check | business-ops |
| [dsh-ar-collection](https://github.com/PerryLink/dsh-ar-collection) | AR collection | business-ops |
| [dsh-settlement-docs](https://github.com/PerryLink/dsh-settlement-docs) | Settlement document completeness | business-ops |
| [dsh-attendance-check](https://github.com/PerryLink/dsh-attendance-check) | Attendance and overtime check | business-ops |
| [dsh-store-replenish](https://github.com/PerryLink/dsh-store-replenish) | Store replenishment | business-ops |

## 7. Phocinae (decision-model line)

| Repo | What it is |
|---|---|
| [dsh-phocinae](https://github.com/PerryLink/dsh-phocinae) | Phocinae decision bundle for DSH: `phocinae_ask` + approval gate |
| [phocinae-server](https://github.com/Phocinae/phocinae-server) | Local TypeSafe `/v1/systemone` inference server |
| [phocinae-guard](https://github.com/Phocinae/phocinae-guard) | Command approval gate for agent harnesses |
| [phocinae-mcp](https://github.com/Phocinae/phocinae-mcp) | MCP decide/classify/route/score/gate tools |
| [phocinae-cli](https://github.com/Phocinae/phocinae-cli) | Terminal decisions |
| [phocinae-js](https://github.com/Phocinae/phocinae-js) | TypeScript client |
| [phocinae-rulepack](https://github.com/Phocinae/phocinae-rulepack) | Versioned rule-pack engine |
| [phocinae-formulate](https://github.com/Phocinae/phocinae-formulate) | Formulation measurement harness |
| [phocinae-publish-gate](https://github.com/Phocinae/phocinae-publish-gate) | Pre-publication checks |
| [dsh-evidence](https://github.com/Phocinae/dsh-evidence) | Deterministic pre-claim gate |
| [dsh-batch-triage](https://github.com/Phocinae/dsh-batch-triage) | Deterministic-first ticket triage |
| [dsh-context-verdict](https://github.com/Phocinae/dsh-context-verdict) | Compaction-loss verdict |

## 8. Catalogs and install surfaces

| Repo | What it is |
|---|---|
| [dsh-kit](https://github.com/PerryLink/dsh-kit) | One-command installers and the mainline roster |
| [dsh-catalog](https://github.com/PerryLink/dsh-catalog) | Machine-readable npm catalog / DSH Desktop Market source |
| [dsh-family-catalog](https://github.com/PerryLink/dsh-family-catalog) | Standard catalog source for the family |
| [dsh-plugin-portal](https://github.com/PerryLink/dsh-plugin-portal) | Zero-dependency static portal with grouped cards |
| [dsh-plugins](https://github.com/PerryLink/dsh-plugins) | Family site, taxonomy, market and ROSTER.md |

## 9. Retired, frozen, moved

- **Retired (3):** dsh-background-agents, dsh-session-pin, dsh-team-rooms — the harness absorbed the capability.
- **Frozen (8):** dsh-autotier, dsh-budget, dsh-cert-mcp, dsh-claude-move, dsh-defend, dsh-draw, dsh-reach, dsh-community-bench.
- **Moved pointers:** dsh-checkers → dsh-check-pack; dsh-plugin-doctor → dsh-clinic; dsh-plugin-kit → dsh-scaffold; dsh-plugin-certification → dsh-certification; dsh-standard → dsh-plugin-spec; dsh-ticktick → dsh-dida; dsh-plugin-upgrade → dsh-codemod; dsh-github → dsh-github-bot; dsh-skill-pack-security → dsh-security-pack.

Source of truth for the runtime/domain rows: [ROSTER.md](https://github.com/PerryLink/dsh-plugins/blob/main/ROSTER.md).
