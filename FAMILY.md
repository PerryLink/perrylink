# The PerryLink DSH plugin family — full index

> Generated 2026-11-04 from `dsh-plugins/family.json` (137 rows: 126 active / 8 frozen / 3 retired),
> `dsh-kit` and the PerryLink/Phocinae repositories. **Coverage: all 149 active and 11 archived own DSH
> repositories are linked below.**
> Groups overlap where a support repo is also a bundle; they are an index, not a partition.

The family has three layers: **standards and guides** (how to build), **developer toolchain** (how to
ship), and **runtime/domain plugins** (what users install). Phocinae is a separate decision-model line.

## ## 1. Three-level standards and checks

| Repo | What it is |
|---|---|
| [dsh-standards](https://github.com/PerryLink/dsh-standards) | ENTRY/FLOW conformance checker, level audit, clause execution |
| [dsh-plugin-spec](https://github.com/PerryLink/dsh-plugin-spec) | Rule text and clause IDs (the source the checker executes) |
| [dsh-certification](https://github.com/PerryLink/dsh-certification) | Community attestation registry, scoring model and badges |
| [dsh-clinic](https://github.com/PerryLink/dsh-clinic) | Install doctor, host-surface snapshot, recovery checks |
| [dsh-score](https://github.com/PerryLink/dsh-score) | Multi-dimensional plugin quality scoring |
| [dsh-plugin-ready](https://github.com/PerryLink/dsh-plugin-ready) | Static ENTRY preflight (`dsh-ready`) |
| [dsh-check-pack](https://github.com/PerryLink/dsh-check-pack) | One-command installer for the 53-checker compliance suite |

## ## 2. Three-level guides

| Repo | What it is |
|---|---|
| [dsh-plugin-guide](https://github.com/PerryLink/dsh-plugin-guide) | Three-layer guide: ENTRY checks, FLOW journeys, BOOST practices |
| [dsh-primer](https://github.com/PerryLink/dsh-primer) | Practical primer + legacy build skill/CLI |

## ## 3. Developer toolchain

| Repo | What it is |
|---|---|
| [dsh-plugin-dev](https://github.com/PerryLink/dsh-plugin-dev) | `dsh-dev` front door: new/check/test/submit/upgrade |
| [dsh-plugin-devtools](https://github.com/PerryLink/dsh-plugin-devtools) | Umbrella for start/ready/tools/dev |
| [dsh-plugin-start](https://github.com/PerryLink/dsh-plugin-start) | `dsh-start new` minimal skeleton |
| [dsh-plugin-tools](https://github.com/PerryLink/dsh-plugin-tools) | `dsh-tools list/doctor/install` |
| [dsh-scaffold](https://github.com/PerryLink/dsh-scaffold) | Shared scaffold and contracts for the family |
| [dsh-codemod](https://github.com/PerryLink/dsh-codemod) | Version-corridor migration codemods |
| [dsh-test-drive](https://github.com/PerryLink/dsh-test-drive) | Isolated install-and-smoke test drives |
| [dsh-claude-move](https://github.com/PerryLink/dsh-claude-move) | Four-source migration wizard (Claude Code/Codex/OpenCode/Hermes) |

## 4. Runtime plugins (32 active mainline rows)

| Repo | What it is | Axis |
|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | 敏感操作复核 | workflow |
| [dsh-checkpoint-rewind](https://github.com/PerryLink/dsh-checkpoint-rewind) | 快照一键回滚 | workflow |
| [dsh-click](https://github.com/PerryLink/dsh-click) | 桌面点击操作 | interface |
| [dsh-composer-history](https://github.com/PerryLink/dsh-composer-history) | 输入历史回溯 | interface |
| [dsh-data-quality](https://github.com/PerryLink/dsh-data-quality) | 数据质量核验 | developer-tools |
| [dsh-doublecheck](https://github.com/PerryLink/dsh-doublecheck) | 交付质量把关 | workflow |
| [dsh-fast](https://github.com/PerryLink/dsh-fast) | 性能瓶颈诊断 | observability |
| [dsh-fund-research](https://github.com/PerryLink/dsh-fund-research) | 基金研究报告 | research |
| [dsh-industry-research](https://github.com/PerryLink/dsh-industry-research) | 行业公司研究 | research |
| [dsh-laya](https://github.com/laya-family/dsh-laya) | 结构化决策支持 | integrations |
| [dsh-library](https://github.com/PerryLink/dsh-library) | 本地资料库检索 | content |
| [dsh-local-ai](https://github.com/PerryLink/dsh-local-ai) | 本地模型接入 | integrations |
| [dsh-lsp-actions](https://github.com/PerryLink/dsh-lsp-actions) | 代码诊断与补全 | developer-tools |
| [dsh-mask](https://github.com/PerryLink/dsh-mask) | 个人信息脱敏 | security |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | 外部工具管理 | developer-tools |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | 跨会话记忆 | workflow |
| [dsh-observe](https://github.com/PerryLink/dsh-observe) | 链路追踪导出 | observability |
| [dsh-output-styles](https://github.com/PerryLink/dsh-output-styles) | 回复风格切换 | interface |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | 权限规则配置 | security |
| [dsh-primer](https://github.com/PerryLink/dsh-primer) | 扩展开发指南 | developer-tools |
| [dsh-codemod](https://github.com/PerryLink/dsh-codemod) | 版本升级迁移 | workflow |
| [dsh-research-report](https://github.com/PerryLink/dsh-research-report) | 可溯源研究报告 | research |
| [dsh-score](https://github.com/PerryLink/dsh-score) | 五维质量评分 | developer-tools |
| [dsh-session-sync](https://github.com/PerryLink/dsh-session-sync) | 会话跨设备同步 | workflow |
| [dsh-talk](https://github.com/PerryLink/dsh-talk) | 语音对话交互 | content |
| [dsh-test-drive](https://github.com/PerryLink/dsh-test-drive) | 隔离试装核验 | workflow |
| [dsh-translate](https://github.com/PerryLink/dsh-translate) | 文本翻译校对 | content |
| [dsh-github-bot](https://github.com/PerryLink/dsh-github-bot) | 代码评审对接 | workflow |
| [dsh-clinic](https://github.com/PerryLink/dsh-clinic) | 包结构冒烟检查 | developer-tools |
| [dsh-scaffold](https://github.com/PerryLink/dsh-scaffold) | 公共组件工具箱 | developer-tools |
| [dsh-security-pack](https://github.com/PerryLink/dsh-security-pack) | 安全技能包供给 | security |
| [dsh-dida](https://github.com/PerryLink/dsh-dida) | 滴答清单对接 | integrations |

**Runtime extras outside `family.json`:** [dsh-phone-inbox](https://github.com/PerryLink/dsh-phone-inbox) (WeChat-bridge inbound attachments) and [dsh-laya](https://github.com/PerryLink/dsh-laya) (Laya decision engine; the canonical family row points at [laya-family/dsh-laya](https://github.com/laya-family/dsh-laya)).

## 5. Compliance checkers (62 active rows)

| Repo | What it is | Axis |
|---|---|---|
| [dsh-customs-doc-check](https://github.com/PerryLink/dsh-customs-doc-check) | 报关单证比对 | compliance / trade |
| [dsh-demurrage-ledger](https://github.com/PerryLink/dsh-demurrage-ledger) | 滞箱费台账核验 | compliance / trade |
| [dsh-export-ctl-check](https://github.com/PerryLink/dsh-export-ctl-check) | 出口管制物项筛查 | compliance / trade |
| [dsh-forecast-penalty](https://github.com/PerryLink/dsh-forecast-penalty) | 预测考核费用测算 | compliance / trade |
| [dsh-hs-classify](https://github.com/PerryLink/dsh-hs-classify) | 商品归类层级校验 | compliance / trade |
| [dsh-lc-doc-check](https://github.com/PerryLink/dsh-lc-doc-check) | 信用证不符点筛查 | compliance / trade |
| [dsh-origin-rvc-check](https://github.com/PerryLink/dsh-origin-rvc-check) | 原产地成分核算 | compliance / trade |
| [dsh-railway-window](https://github.com/PerryLink/dsh-railway-window) | 铁路天窗台账复核 | compliance / trade |
| [dsh-fmea-table-check](https://github.com/PerryLink/dsh-fmea-table-check) | 失效分析表核对 | compliance / quality |
| [dsh-ota-review-check](https://github.com/PerryLink/dsh-ota-review-check) | 点评回复时效检查 | compliance / quality |
| [dsh-pipeline-check](https://github.com/PerryLink/dsh-pipeline-check) | 项目文件链条联查 | compliance / quality |
| [dsh-ppap-check](https://github.com/PerryLink/dsh-ppap-check) | 生产件批准放行 | compliance / quality |
| [dsh-repair-order-qc](https://github.com/PerryLink/dsh-repair-order-qc) | 维修结算单核算 | compliance / quality |
| [dsh-review-reply-check](https://github.com/PerryLink/dsh-review-reply-check) | 审稿回应逐条对照 | compliance / quality |
| [dsh-spc-gbt-adapter](https://github.com/PerryLink/dsh-spc-gbt-adapter) | 过程能力指数计算 | compliance / quality |
| [dsh-warranty-calc](https://github.com/PerryLink/dsh-warranty-calc) | 质保索赔金额核算 | compliance / quality |
| [dsh-aqua-input-check](https://github.com/PerryLink/dsh-aqua-input-check) | 水产投入品核查 | compliance / safety |
| [dsh-drill-script-check](https://github.com/PerryLink/dsh-drill-script-check) | 演练脚本要素清点 | compliance / safety |
| [dsh-emergency-plan](https://github.com/PerryLink/dsh-emergency-plan) | 应急预案要素审查 | compliance / safety |
| [dsh-hazchem-check](https://github.com/PerryLink/dsh-hazchem-check) | 危化品临界量辨识 | compliance / safety |
| [dsh-hidden-risk-map](https://github.com/PerryLink/dsh-hidden-risk-map) | 重大隐患判定映射 | compliance / safety |
| [dsh-power-loss-split](https://github.com/PerryLink/dsh-power-loss-split) | 线损电量拆分 | compliance / safety |
| [dsh-power-ticket-check](https://github.com/PerryLink/dsh-power-ticket-check) | 电力工作票核查 | compliance / safety |
| [dsh-bid-ca-precheck](https://github.com/PerryLink/dsh-bid-ca-precheck) | 投标符合性预检 | compliance / tender |
| [dsh-bid-qual-check](https://github.com/PerryLink/dsh-bid-qual-check) | 投标资格条件审查 | compliance / tender |
| [dsh-contract-stance](https://github.com/PerryLink/dsh-contract-stance) | 合同立场台账梳理 | compliance / tender |
| [dsh-protest-deadline](https://github.com/PerryLink/dsh-protest-deadline) | 质疑投诉期限测算 | compliance / tender |
| [dsh-rulefile-check](https://github.com/PerryLink/dsh-rulefile-check) | 规则库自检 | compliance / tender |
| [dsh-tender-extract](https://github.com/PerryLink/dsh-tender-extract) | 招标条款逐字摘录 | compliance / tender |
| [dsh-tender-matrix](https://github.com/PerryLink/dsh-tender-matrix) | 评标评分矩阵校验 | compliance / tender |
| [dsh-eia-guide-check](https://github.com/PerryLink/dsh-eia-guide-check) | 环评导则适用判定 | compliance / construction |
| [dsh-guard-plan-qc](https://github.com/PerryLink/dsh-guard-plan-qc) | 劳保用品配置核对 | compliance / construction |
| [dsh-hazplan-check](https://github.com/PerryLink/dsh-hazplan-check) | 偏差分析表复核 | compliance / construction |
| [dsh-permit-report-check](https://github.com/PerryLink/dsh-permit-report-check) | 行政许可材料核查 | compliance / construction |
| [dsh-safety-brief-check](https://github.com/PerryLink/dsh-safety-brief-check) | 安全交底签字闭环 | compliance / construction |
| [dsh-site-log-check](https://github.com/PerryLink/dsh-site-log-check) | 监理日志连续检查 | compliance / construction |
| [dsh-soilwater-check](https://github.com/PerryLink/dsh-soilwater-check) | 土壤地下水核验 | compliance / construction |
| [dsh-essay-rubric-check](https://github.com/PerryLink/dsh-essay-rubric-check) | 作文量表评分复核 | compliance / research |
| [dsh-learning-gap-check](https://github.com/PerryLink/dsh-learning-gap-check) | 能力差距培养评估 | compliance / research |
| [dsh-nsfc-form-check](https://github.com/PerryLink/dsh-nsfc-form-check) | 国自然形式审查 | compliance / research |
| [dsh-paper-doc-adapter](https://github.com/PerryLink/dsh-paper-doc-adapter) | 试卷结构解析校核 | compliance / research |
| [dsh-policy-brief-draft](https://github.com/PerryLink/dsh-policy-brief-draft) | 政策专报要素审定 | compliance / research |
| [dsh-archive-check](https://github.com/PerryLink/dsh-archive-check) | 档案归档查验 | compliance / government |
| [dsh-gongwen-flow-check](https://github.com/PerryLink/dsh-gongwen-flow-check) | 公文流转时限检查 | compliance / government |
| [dsh-gongwen-word-check](https://github.com/PerryLink/dsh-gongwen-word-check) | 公文格式要素校对 | compliance / government |
| [dsh-evidence-check](https://github.com/PerryLink/dsh-evidence-check) | 证据清单齐备核验 | compliance / legal |
| [dsh-lawcite-adapter](https://github.com/PerryLink/dsh-lawcite-adapter) | 法条引用校对 | compliance / legal |
| [dsh-pleading-draft](https://github.com/PerryLink/dsh-pleading-draft) | 起诉状要素核对 | compliance / legal |
| [dsh-icd-rule-check](https://github.com/PerryLink/dsh-icd-rule-check) | 疾病编码规则核对 | compliance / medical |
| [dsh-medrec-qc](https://github.com/PerryLink/dsh-medrec-qc) | 病案首页质控 | compliance / medical |
| [dsh-nurse-record-check](https://github.com/PerryLink/dsh-nurse-record-check) | 护理记录核对 | compliance / medical |
| [dsh-soe-decision-check](https://github.com/PerryLink/dsh-soe-decision-check) | 国企决策合规检查 | compliance / governance |
| [dsh-sop-sync-check](https://github.com/PerryLink/dsh-sop-sync-check) | 作业规程同步检查 | compliance / governance |
| [dsh-bid-health-check](https://github.com/PerryLink/dsh-bid-health-check) | 投标响应覆盖检查 | compliance / tender |
| [dsh-canteen-retention-check](https://github.com/PerryLink/dsh-canteen-retention-check) | 食堂留样台账核对 | compliance / safety |
| [dsh-construction-doc-check](https://github.com/PerryLink/dsh-construction-doc-check) | 施工资料齐套检查 | compliance / construction |
| [dsh-excel-reconcile](https://github.com/PerryLink/dsh-excel-reconcile) | 双表对账查差异 | data / data |
| [dsh-invoice-ledger](https://github.com/PerryLink/dsh-invoice-ledger) | 发票台账核验 | compliance / finance |
| [dsh-payroll-audit](https://github.com/PerryLink/dsh-payroll-audit) | 工资核算复核 | compliance / finance |
| [dsh-safety-ledger-check](https://github.com/PerryLink/dsh-safety-ledger-check) | 安全资质台账核对 | compliance / construction |
| [dsh-table-ingest](https://github.com/PerryLink/dsh-table-ingest) | 表格数据提取 | data / data |
| [dsh-tender-requirements](https://github.com/PerryLink/dsh-tender-requirements) | 招标文件要点提取 | business-ops / tender |

## 6. Domain operations (29 active rows)

| Repo | What it is | Axis |
|---|---|---|
| [dsh-einvoice](https://github.com/PerryLink/dsh-einvoice) | China e-invoice (file-level) | business-ops / finance |
| [dsh-bankrec](https://github.com/PerryLink/dsh-bankrec) | Bank statement reconciliation | business-ops / finance |
| [dsh-ap-three-way](https://github.com/PerryLink/dsh-ap-three-way) | AP three-way match | business-ops / finance |
| [dsh-travel-recon](https://github.com/PerryLink/dsh-travel-recon) | Travel reconciliation & policy check | business-ops / finance |
| [dsh-legal-intake](https://github.com/PerryLink/dsh-legal-intake) | Legal request intake | business-ops / legal |
| [dsh-legal-clause](https://github.com/PerryLink/dsh-legal-clause) | Contract clause & playbook review | business-ops / legal |
| [dsh-ghg](https://github.com/PerryLink/dsh-ghg) | Electricity GHG (Scope 2) | business-ops / esg |
| [dsh-qms-capa](https://github.com/PerryLink/dsh-qms-capa) | QMS NCR, CAPA & 8D | business-ops / quality |
| [dsh-hs-candidate](https://github.com/PerryLink/dsh-hs-candidate) | HS candidate precheck | business-ops / trade |
| [dsh-freight-audit](https://github.com/PerryLink/dsh-freight-audit) | Freight bill audit | business-ops / logistics |
| [dsh-docx-redline](https://github.com/PerryLink/dsh-docx-redline) | DOCX inspect & text diff | content / documents |
| [dsh-ifc-qto](https://github.com/PerryLink/dsh-ifc-qto) | IFC quantity takeoff | data / construction |
| [dsh-policy-ledger](https://github.com/PerryLink/dsh-policy-ledger) | Install doctor | developer-tools / plugin-install |
| [dsh-pim-lint](https://github.com/PerryLink/dsh-pim-lint) | PIM catalog lint | data / retail |
| [dsh-eval-pack](https://github.com/PerryLink/dsh-eval-pack) | Eval pack lint & grader | developer-tools / evaluation |
| [dsh-finops-suite](https://github.com/PerryLink/dsh-finops-suite) | Finance ops suite | business-ops / finance |
| [dsh-contract-suite](https://github.com/PerryLink/dsh-contract-suite) | Contract ops suite | business-ops / legal |
| [dsh-provider-params](https://github.com/PerryLink/dsh-provider-params) | Provider parameter mapping and JSON repair | developer-tools / runtime |
| [dsh-pdf-table](https://github.com/PerryLink/dsh-pdf-table) | PDF table extraction (text layer) | data / document |
| [dsh-contract-renewal](https://github.com/PerryLink/dsh-contract-renewal) | Contract renewal tracker | business-ops / legal |
| [dsh-rfq-compare](https://github.com/PerryLink/dsh-rfq-compare) | RFQ comparison | business-ops / procurement |
| [dsh-labor-contract](https://github.com/PerryLink/dsh-labor-contract) | Labor contract check | business-ops / hr |
| [dsh-progress-payment](https://github.com/PerryLink/dsh-progress-payment) | Progress payment audit | business-ops / construction |
| [dsh-ar-aging](https://github.com/PerryLink/dsh-ar-aging) | AR aging | business-ops / finance |
| [dsh-import-customs-check](https://github.com/PerryLink/dsh-import-customs-check) | Import document check | business-ops / trade |
| [dsh-ar-collection](https://github.com/PerryLink/dsh-ar-collection) | AR collection | business-ops / finance |
| [dsh-settlement-docs](https://github.com/PerryLink/dsh-settlement-docs) | Settlement document completeness | business-ops / construction |
| [dsh-attendance-check](https://github.com/PerryLink/dsh-attendance-check) | Attendance and overtime check | business-ops / hr |
| [dsh-store-replenish](https://github.com/PerryLink/dsh-store-replenish) | Store replenishment | business-ops / retail |

## ## 7. Phocinae (decision-model line)

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

## ## 8. Catalogs and install surfaces

| Repo | What it is |
|---|---|
| [dsh-kit](https://github.com/PerryLink/dsh-kit) | One-command installers and the mainline roster |
| [dsh-catalog](https://github.com/PerryLink/dsh-catalog) | Machine-readable npm catalog / DSH Desktop Market source |
| [dsh-family-catalog](https://github.com/PerryLink/dsh-family-catalog) | Standard catalog source for the family |
| [dsh-plugin-portal](https://github.com/PerryLink/dsh-plugin-portal) | Zero-dependency static portal with grouped cards |
| [dsh-plugins](https://github.com/PerryLink/dsh-plugins) | Family site, taxonomy, market and ROSTER.md |

## 9. Frozen, moved and retired

### Frozen (8)

| Repo | Status |
|---|---|
| [dsh-autotier](https://github.com/PerryLink/dsh-autotier) | 🧊 frozen — compatibility updates stopped; existing installs keep working |
| [dsh-budget](https://github.com/PerryLink/dsh-budget) | 🧊 frozen — compatibility updates stopped; existing installs keep working |
| [dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) | 🧊 frozen — compatibility updates stopped; existing installs keep working |
| [dsh-claude-move](https://github.com/PerryLink/dsh-claude-move) | 🧊 frozen — compatibility updates stopped; existing installs keep working |
| [dsh-community-bench](https://github.com/PerryLink/dsh-community-bench) | 🧊 frozen — compatibility updates stopped; existing installs keep working |
| [dsh-defend](https://github.com/PerryLink/dsh-defend) | 🧊 frozen — compatibility updates stopped; existing installs keep working |
| [dsh-draw](https://github.com/PerryLink/dsh-draw) | 🧊 frozen — compatibility updates stopped; existing installs keep working |
| [dsh-reach](https://github.com/PerryLink/dsh-reach) | 🧊 frozen — compatibility updates stopped; existing installs keep working |

### Moved pointers

| Repo | Now |
|---|---|
| [dsh-checkers](https://github.com/PerryLink/dsh-checkers) | [dsh-check-pack](https://github.com/PerryLink/dsh-check-pack) |
| [dsh-plugin-doctor](https://github.com/PerryLink/dsh-plugin-doctor) | [dsh-clinic](https://github.com/PerryLink/dsh-clinic) |
| [dsh-plugin-kit](https://github.com/PerryLink/dsh-plugin-kit) | [dsh-scaffold](https://github.com/PerryLink/dsh-scaffold) |
| [dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification) | [dsh-certification](https://github.com/PerryLink/dsh-certification) |
| [dsh-standard](https://github.com/PerryLink/dsh-standard) | [dsh-plugin-spec](https://github.com/PerryLink/dsh-plugin-spec) |
| [dsh-github](https://github.com/PerryLink/dsh-github) | [dsh-github-bot](https://github.com/PerryLink/dsh-github-bot) |
| [dsh-skill-pack-security](https://github.com/PerryLink/dsh-skill-pack-security) | [dsh-security-pack](https://github.com/PerryLink/dsh-security-pack) |
| [dsh-ticktick](https://github.com/PerryLink/dsh-ticktick) | [dsh-dida](https://github.com/PerryLink/dsh-dida) |
| [dsh-plugin-upgrade](https://github.com/PerryLink/dsh-plugin-upgrade) | [dsh-codemod](https://github.com/PerryLink/dsh-codemod) |
| [dsh-plugin-upgrade-015](https://github.com/PerryLink/dsh-plugin-upgrade-015) | [dsh-codemod (retired)](https://github.com/PerryLink/dsh-codemod (retired)) |
| [dsh-plugin-upgrade-016](https://github.com/PerryLink/dsh-plugin-upgrade-016) | [dsh-codemod (retired)](https://github.com/PerryLink/dsh-codemod (retired)) |

### Retired (3)

| Repo | Why |
|---|---|
| [dsh-background-agents](https://github.com/PerryLink/dsh-background-agents) | harness ships native continuable subagents |
| [dsh-session-pin](https://github.com/PerryLink/dsh-session-pin) | harness ships session pinning |
| [dsh-team-rooms](https://github.com/PerryLink/dsh-team-rooms) | harness ships Agent Teams |


Source of truth for the runtime/domain rows: [ROSTER.md](https://github.com/PerryLink/dsh-plugins/blob/main/ROSTER.md).
