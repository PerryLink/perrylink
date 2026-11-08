# PerryLink DSH 插件家族 — 全索引

> 2026-11-08 逐仓对照 README 重写描述；行数与状态沿用 2026-11-04 的 `dsh-plugins/family.json` 快照
> （137 行：126 active / 8 frozen / 3 retired），其余行来自 `dsh-kit` 与 PerryLink/Phocinae 仓库。
> **2026-11-08 改名：** `dsh-translate` 自 0.3.0 起是整页翻译插件；原「厂商参数映射 + 确定性 JSON 修复」改名
> `dsh-param-repair`（1.0.1），`/translate` 命令、`fix_json` 工具与全部配置键不变。
> 覆盖：169 个活跃 + 11 个归档的自有 DSH 仓库，全部在下方有链接（137 行安装名册 + 19 个 catalog-only 科研插件，见 §10；另有 catalog-only 的整页翻译插件）。
> 分组按用途重叠——一个支持仓同时是 bundle 时会出现两次；这是索引，不是互斥分区。

家族分三层：**规范与指南**（怎么建）、**开发者工具链**（怎么发）、**运行时/领域插件**（用户装什么）；Phocinae 是独立的决策模型线。

**怎么读**：每条一句话——前半句说它读什么、产出什么，后半句说它与同类不同在哪（确定性、离线、版本化规则包、不改原件、默认拒绝之类）。事实描述以对应仓库的 README 为准；🧊 表示冻结：兼容更新停止，已装的继续用。

## 1. Three-level standards and checks

规范、判据与验收表面：先把「什么样算合格」写成可执行条款，再谈单个插件做得好不好。要给 DSH 投稿或验收插件，从这一组进。

| 仓库 | 它做什么 · 关键差异 |
|---|---|
| [dsh-standards](https://github.com/PerryLink/dsh-standards) | 三层规范（ENTRY/FLOW/BOOST）的执行总入口：带一致性核查器、等级审计与规范原文；A–D 只是质量分档，不是认证或安全审计 |
| [dsh-plugin-spec](https://github.com/PerryLink/dsh-plugin-spec) | 以编号条款维护 DSH 插件规范原文，供核查器逐条执行；只维护规则文本与编号，不做认证、安全审计与收费评级 |
| [dsh-certification](https://github.com/PerryLink/dsh-certification) | 社区插件的公开规范、可机器校验的评分模型与带徽章的独立登记册；只做可复现的数据登记，不发布插件、不声称权威 |
| [dsh-clinic](https://github.com/PerryLink/dsh-clinic) | 一次运行对插件做四层检测：包结构静态检查、cordis 契约扫描、动态沙箱冒烟与集合站清单校验；零依赖，只用 Node 自带能力 |
| [dsh-score](https://github.com/PerryLink/dsh-score) | 对插件做五维质量评分（安装、维护、文档、安全、合规），产出风险卡与排行榜；只跑 gh 与 npm 取证，无证据就报 no-evidence |
| [dsh-plugin-ready](https://github.com/PerryLink/dsh-plugin-ready) | 不装包、不启宿主，只读包内容做 ENTRY 静态预检（元数据、入口、patch、engines、README/LICENSE）；静态通过不等于认证 |
| [dsh-check-pack](https://github.com/PerryLink/dsh-check-pack) | 用一条命令把 53 个合规核查器按锁定版本装进当前 profile；包本身只负责安装，不含核查逻辑、不碰数据 |

## 2. Three-level guides

把条款讲成人能走的路径：三层规范怎么落地、一次会话旅程怎么验收、性能实践怎么量。

| 仓库 | 它做什么 · 关键差异 |
|---|---|
| [dsh-plugin-guide](https://github.com/PerryLink/dsh-plugin-guide) | 三层讲 DSH 插件开发：ENTRY 检查、FLOW 旅程、BOOST 实践，配官方文档副本与版本矩阵；知识库注册成可加载的 agent 技能 |
| [dsh-primer](https://github.com/PerryLink/dsh-primer) | DSH 插件开发知识库：官方文档副本、版本矩阵、Cordis 入门与 20+ 踩坑，注册成按需加载的 agent 技能；另带 new/check/verify CLI |

## 3. Developer toolchain

从建仓到发布的一条命令行路径：脚手架、静态预检、安装与诊断、版本迁移、隔离试装。

| 仓库 | 它做什么 · 关键差异 |
|---|---|
| [dsh-plugin-dev](https://github.com/PerryLink/dsh-plugin-dev) | 把新建、检查、测试、提交、升级收成一个 dsh-dev 入口，按流程分发给家族里的各专用命令；包名与命令名分开以免重名 |
| [dsh-plugin-devtools](https://github.com/PerryLink/dsh-plugin-devtools) | 把 start、ready、tools、dev 四个小 CLI 收成一套命令家族，覆盖插件开发全程；本身不是运行时插件，也不做评分、排名与认证 |
| [dsh-plugin-start](https://github.com/PerryLink/dsh-plugin-start) | 给一个包名即写出符合当前规范的最小插件骨架，含 package.json 与 cordis.patch.yml；只生成文件，不装依赖、不启宿主、不发布 |
| [dsh-plugin-tools](https://github.com/PerryLink/dsh-plugin-tools) | 列出、诊断 DSH 开发工具并打印可直接执行的安装命令；它自己从不安装或更新，也不做包审计与评分 |
| [dsh-scaffold](https://github.com/PerryLink/dsh-scaffold) | 把 20+ 插件重复手写的 Provider seam、审批门与 sanitize/pricing/judge 抽成共享 TypeScript 包；零运行时依赖 |
| [dsh-codemod](https://github.com/PerryLink/dsh-codemod) | 读取目标仓库声明的 dsh 版本区间，套用对应走廊里有证据的迁移规则做只读扫描；不写被扫仓库、不联网、不起子进程 |
| [dsh-test-drive](https://github.com/PerryLink/dsh-test-drive) | 在一次性 profile 中安装插件、跑 headless 冒烟与可选能力断言，产出结构化矩阵后再卸载清理；隔离根只落在系统临时目录，绝不碰真实 ~/.dsh |
| [dsh-claude-move](https://github.com/PerryLink/dsh-claude-move) | 把 Claude Code、Codex、OpenCode 与 Hermes 的会话、记忆、技能和斜杠命令复制成可续聊的 DSH 会话；源文件只读、写入过审批门（🧊 已冻结） |

## 4. Runtime plugins

装进 DSH 后直接改变会话行为的插件：审批与权限、记忆与回滚、界面与输入、研究、可观测性、外部系统对接。

| 仓库 | 它做什么 · 关键差异 | 分类 |
|---|---|---|
| [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) | 在动作越过沙箱边界时由只读的第二模型审查证据并给出允许或拒绝及理由；白名单只含读类工具，任何异常路径默认按拒绝处理 | workflow |
| [dsh-checkpoint-rewind](https://github.com/PerryLink/dsh-checkpoint-rewind) | 把会话、工作区与配置三态一起存成检查点，用一条经批准的命令恢复其中任意一个；恢复只覆盖已捕获文件，检查点之后新建的文件原样保留 | workflow |
| [dsh-click](https://github.com/PerryLink/dsh-click) | 先观察屏幕再动手的跨平台桌面控制，每次点击都过审批并留审计；屏幕像素哈希变化或观察过期即拒绝，且不抢目标窗口前台焦点 | interface |
| [dsh-composer-history](https://github.com/PerryLink/dsh-composer-history) | 把终端式输入历史搬进 Web GUI 作曲器，光标在首行时按 ↑ 召回、按 Esc 还原草稿；纯 UI 行为，不产生会话事件也不发模型请求 | interface |
| [dsh-data-quality](https://github.com/PerryLink/dsh-data-quality) | 对 CSV/JSON 表格数据集做确定性梳理、声明式清洗与规则核查，逐规则留审计日志；不做 ML 异常检测、不做 PII 脱敏、不连数据库 | developer-tools |
| [dsh-doublecheck](https://github.com/PerryLink/dsh-doublecheck) | 在改动前拷问需求，用红绿测试证据与对抗式评审验收实现，最后给出可交付或需要返工的裁决；报告只记计数与裁决，不含文件内容 | workflow |
| [dsh-fast](https://github.com/PerryLink/dsh-fast) | 只读观测会话事件流，报出加载耗时、上下文注入体量与缓存命中率并给阈值驱动的优化建议；异步 O(1) 折叠，绝不在追加路径上执行 | observability |
| [dsh-fund-research](https://github.com/PerryLink/dsh-fund-research) | 按基金代码生成版本化 Markdown 研究报告，把每个关键数字映射到带哈希的快照路径与核查结论；数据源缺失时显式声明缺口，绝不编造数字 | research |
| [dsh-industry-research](https://github.com/PerryLink/dsh-industry-research) | 把产业链结构图、公开源时间线与公司速览卡汇成可核查报告，每个数字都带来源哈希回溯；v1 只读文本格式、不解析 PDF，不接交易也不预测价格 | research |
| [dsh-laya](https://github.com/laya-family/dsh-laya) | 把 Laya 的 noul、choice、score 三类类型化决策以一等 Cordis 服务和模型可见工具的形式接入 DeepSeek Harness | integrations |
| [dsh-library](https://github.com/PerryLink/dsh-library) | 把本地文档导入成知识库并做带引用标记的混合检索，让 agent 可自证引用；默认零模型下载零网络调用，打分是确定性哈希与词法数学 | content |
| [dsh-local-ai](https://github.com/PerryLink/dsh-local-ai) | 把 Ollama 注册成一等本地模型提供方，按任务类型或关键词分流、首个 token 前失败自动回退云端；走 HTTP API、零依赖、不捆绑模型文件 | integrations |
| [dsh-lsp-actions](https://github.com/PerryLink/dsh-lsp-actions) | 把真实语言服务器的诊断、格式化、补全、代码动作、符号与重命名做成八个 lsp_ 工具，并给出编辑器 action 协议面；每个动作都是开文件、发一个请求、关文件 | developer-tools |
| [dsh-mask](https://github.com/PerryLink/dsh-mask) | 在消息进模型前把电话、邮箱、身份证、银行卡与密钥换成占位符；恢复表只落在内存与受控存储域，审计只记替换处数与类型分布 | security |
| [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) | 在设置页可视化增删改 MCP 服务器并试调工具，未观测到的状态如实显示 unknown；只写走审批的 profile patch，写完对照 loader 复验 | developer-tools |
| [dsh-memento](https://github.com/PerryLink/dsh-memento) | 用本地 SQLite 提供有界、分层、带审批门且可审计的跨会话记忆，写满返回结构化错误；每条写路径都经服务内部审批，被拒的写也落审计行 | workflow |
| [dsh-observe](https://github.com/PerryLink/dsh-observe) | 把 turn、step、工具调用与生成导出成 OTLP 与 Langfuse 观测，按 provider/model 汇总 token 与美元成本；正文脱敏后入队，默认关闭 | observability |
| [dsh-output-styles](https://github.com/PerryLink/dsh-output-styles) | 用 /style 命令在运行时切换模型输出风格并按会话持久保存，内置 concise 等六种风格；只作用于主会话，子代理保留各自提示 | interface |
| [dsh-param-repair](https://github.com/PerryLink/dsh-param-repair) | 把 11 家厂商的请求参数互相映射，并把坏掉的 JSON 工具输出按固定策略修到能过 schema 校验；不联网、不编造值，修复过程不调用模型 | developer-tools |
| [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) | 在每次工具调用前用纯 YAML 规则表裁决 allow、deny、ask，命中和透传都写入会话日志；未命中严格交给下游，缺审批者时失败关闭 | security |
| [dsh-primer](https://github.com/PerryLink/dsh-primer) | DSH 插件开发知识库：官方文档副本、版本矩阵、Cordis 入门与 20+ 踩坑，注册成按需加载的 agent 技能；另带 new/check/verify CLI | developer-tools |
| [dsh-codemod](https://github.com/PerryLink/dsh-codemod) | 读取目标仓库声明的 dsh 版本区间，套用对应走廊里有证据的迁移规则做只读扫描；不写被扫仓库、不联网、不起子进程 | workflow |
| [dsh-research-report](https://github.com/PerryLink/dsh-research-report) | 把每条结论绑定到不可变证据快照，按字节核查其中数字与引文，再封存成哈希可重算的版本化报告；只做字面核对，不做语义理解 | research |
| [dsh-score](https://github.com/PerryLink/dsh-score) | 对插件做五维质量评分（安装、维护、文档、安全、合规），产出风险卡与排行榜；只跑 gh 与 npm 取证，无证据就报 no-evidence | developer-tools |
| [dsh-session-sync](https://github.com/PerryLink/dsh-session-sync) | 为会话存储建立专用 git 镜像，在多设备间同步会话；冲突时 append-only 三分支合并保留两边，绝不强推、reset 或删 fork 文件 | workflow |
| [dsh-talk](https://github.com/PerryLink/dsh-talk) | 按下麦克风说话，把回复朗读出来，说话即打断；语音事件只在宿主能承载时写入会话日志，审批播报不阻塞 | content |
| [dsh-test-drive](https://github.com/PerryLink/dsh-test-drive) | 在一次性 profile 中安装插件、跑 headless 冒烟与可选能力断言，产出结构化矩阵后再卸载清理；隔离根只落在系统临时目录，绝不碰真实 ~/.dsh | workflow |
| [dsh-translate](https://github.com/PerryLink/dsh-translate) | 遍历当前页面可见文字，用你当前会话的模型路由整页翻译，代码、路径、命令与专名先遮成占位符再还原；只改显示层，不写会话日志 | interface |
| [dsh-github-bot](https://github.com/PerryLink/dsh-github-bot) | 把 PR、审查、issue 与 CI 接进会话，让 agent 在审批后创建、审查、合并与检索 GitHub；写操作只走官方审批接缝，token 从不落日志 | workflow |
| [dsh-clinic](https://github.com/PerryLink/dsh-clinic) | 一次运行对插件做四层检测：包结构静态检查、cordis 契约扫描、动态沙箱冒烟与集合站清单校验；零依赖，只用 Node 自带能力 | developer-tools |
| [dsh-scaffold](https://github.com/PerryLink/dsh-scaffold) | 把 20+ 插件重复手写的 Provider seam、审批门与 sanitize/pricing/judge 抽成共享 TypeScript 包；零运行时依赖 | developer-tools |
| [dsh-security-pack](https://github.com/PerryLink/dsh-security-pack) | 把八套安全审计方法论做成 SKILL.md 技能，附零依赖的 plugin_vet 装前扫描器查许可证、SBOM 与 commit 锁定；不取代人工审计 | security |
| [dsh-dida](https://github.com/PerryLink/dsh-dida) | 把滴答清单的清单、任务与截止日期接到会话头部面板，另给 11 个 agent 工具；全部走官方滴答 MCP 端点，令牌每次请求重读 | integrations |

**`family.json` 之外的运行时条目：** [dsh-phone-inbox](https://github.com/PerryLink/dsh-phone-inbox)（微信桥接入站附件）、[dsh-laya](https://github.com/PerryLink/dsh-laya)（Laya 决策引擎；family 行指向 [laya-family/dsh-laya](https://github.com/laya-family/dsh-laya)）与 [dsh-translate](https://github.com/PerryLink/dsh-translate)（0.3.2 起的整页翻译，catalog-only；与 §10 科研套件同类，不计入 137 行）。

## 5. Compliance checkers

这一组核查器形态相同：交一份材料，按随包版本化规则逐条核，输出「哪行、哪栏、差什么」；差异在材料类型和规则包，不在流程。

| 仓库 | 它做什么 · 关键差异 | 分类 |
|---|---|---|
| [dsh-customs-doc-check](https://github.com/PerryLink/dsh-customs-doc-check) | 核对报关单证台账的十位商品编号、币制代码与单证编号重复，指出哪行哪栏差什么；只列能逐条指认的差异，不判申报是否属实 | compliance / trade |
| [dsh-demurrage-ledger](https://github.com/PerryLink/dsh-demurrage-ledger) | 核对滞箱费台账的免箱期起算、还箱日期、超期天数与金额算式是否自洽，逐箱指出哪一栏差什么；纯内存计算，不判费用该由谁承担 | compliance / trade |
| [dsh-export-ctl-check](https://github.com/PerryLink/dsh-export-ctl-check) | 核对出口管制物项台账的受控标注、许可证号与发证日期、最终用途是否闭环，逐行指出哪一栏缺什么；离线运行，不判物项是否受控 | compliance / trade |
| [dsh-forecast-penalty](https://github.com/PerryLink/dsh-forecast-penalty) | 核对预测准确率考核台账的定义式与考核费用算式是否与配置相符，逐期指出哪栏差什么；不判达标与否，也不决定费用该不该收 | compliance / trade |
| [dsh-hs-classify](https://github.com/PerryLink/dsh-hs-classify) | 核对商品归类台账里编号与章、品目、子目的前缀层级是否逐级自洽，指出哪行哪栏差什么；不查税则，也不判断商品该归入哪个编号 | compliance / trade |
| [dsh-lc-doc-check](https://github.com/PerryLink/dsh-lc-doc-check) | 核对信用证交单核对表的单据种类、提交情况与两项日期是否自洽，逐条指出哪栏缺什么；只做机械核对，不解读条款、不判不符点 | compliance / trade |
| [dsh-origin-rvc-check](https://github.com/PerryLink/dsh-origin-rvc-check) | 核对原产地判定台账的区域价值成分算式与协定口径，逐料件指出哪栏差什么；规则包不伪造引文，不下合规结论、不改原件 | compliance / trade |
| [dsh-railway-window](https://github.com/PerryLink/dsh-railway-window) | 核对铁路施工天窗台账的起止时间与天窗时长、批准时长是否自洽，逐条指出哪栏差什么；分类口径由本机构配置，不判施工是否违章 | compliance / trade |
| [dsh-fmea-table-check](https://github.com/PerryLink/dsh-fmea-table-check) | 核对 FMEA 分析表的评分可运算性、RPN 乘积与高风险措施的责任人期限，指出哪栏差什么；不改原表，不评判打分是否恰当 | compliance / quality |
| [dsh-ota-review-check](https://github.com/PerryLink/dsh-ota-review-check) | 核对在线点评回复台账的回复人与回复日期、未回复是否超出自填期限，逐条指出哪栏差什么；不判回复是否恰当、差评是否恶意 | compliance / quality |
| [dsh-pipeline-check](https://github.com/PerryLink/dsh-pipeline-check) | 核对项目文件链条台账的环节顺序、批复与签署日期先后、文件编号唯一性，指出哪栏差什么；不判项目合规，也不判支出是否超概算 | compliance / quality |
| [dsh-ppap-check](https://github.com/PerryLink/dsh-ppap-check) | 核对 PPAP 提交要素清单的提交记录、受控要素版本与零件号提交等级是否齐全，指出哪栏差什么；不判 PPAP 能否批准 | compliance / quality |
| [dsh-repair-order-qc](https://github.com/PerryLink/dsh-repair-order-qc) | 核对机动车维修工单的数量单价乘积、明细合计与结算总额算式，逐项指出哪栏差什么；7 条规则各带条款出处，不判收费是否合理 | compliance / quality |
| [dsh-review-reply-check](https://github.com/PerryLink/dsh-review-reply-check) | 核对审稿意见逐条回应表的回应覆盖与修改位置留痕，逐条指出哪栏缺什么；看不到稿件本身，不核对改动是否真的存在 | compliance / quality |
| [dsh-spc-gbt-adapter](https://github.com/PerryLink/dsh-spc-gbt-adapter) | 核对控制图台账的控制限、中心线与 Cp/Cpk 是否符合定义式与常数表，指出哪栏差什么；不判过程是否受控、能力是否充分 | compliance / quality |
| [dsh-warranty-calc](https://github.com/PerryLink/dsh-warranty-calc) | 核对质保索赔台账的质保期截止、质保里程与金额算式是否自洽，逐笔指出哪栏差什么；零依赖纯本地计算，不判索赔是否该受理 | compliance / quality |
| [dsh-aqua-input-check](https://github.com/PerryLink/dsh-aqua-input-check) | 核对水产养殖投入品记录的投入量、使用日期与休药期起捕关系，指出哪行哪栏差什么；不判水产品是否安全可食，不判用药是否恰当 | compliance / safety |
| [dsh-drill-script-check](https://github.com/PerryLink/dsh-drill-script-check) | 核对应急演练脚本的指挥人、响应级别、所需资源与各环节时长合计，逐环节指出哪栏差什么；响应分级不内置，须填本单位口径 | compliance / safety |
| [dsh-emergency-plan](https://github.com/PerryLink/dsh-emergency-plan) | 核对应急预案的章节树与正文，按声明的预案类型查要素缺失、只有标题没正文，并定位到页或行；不判内容写得好坏 | compliance / safety |
| [dsh-hazchem-check](https://github.com/PerryLink/dsh-hazchem-check) | 核对危险化学品台账的储存量与临界量关系、重大危险源判定是否自洽，逐种指出哪栏差什么；不判是否构成重大危险源、是否需备案 | compliance / safety |
| [dsh-hidden-risk-map](https://github.com/PerryLink/dsh-hidden-risk-map) | 按关键词把安全隐患台账映射到工贸企业重大事故隐患判定标准的候选条款，报出台账缺口；只供人工复核，不判是否构成重大隐患 | compliance / safety |
| [dsh-power-loss-split](https://github.com/PerryLink/dsh-power-loss-split) | 核对一条线路单周期线损材料中供电量、售电量、线损电量与线损率的除法与量平衡，每条命中带算式和容差；阈值由本机构配置 | compliance / safety |
| [dsh-power-ticket-check](https://github.com/PerryLink/dsh-power-ticket-check) | 核对电力工作票的必填栏目、签发许可终结时间顺序与角色分设是否成立，逐栏指出差什么；单票模式看不出同一人是否同时执行两票 | compliance / safety |
| [dsh-bid-ca-precheck](https://github.com/PerryLink/dsh-bid-ca-precheck) | 核对投标符合性响应台账的响应、结论取值与高风险条款证明材料，指出哪行哪栏差什么；不判投标是否有效、是否构成实质性偏离 | compliance / tender |
| [dsh-bid-qual-check](https://github.com/PerryLink/dsh-bid-qual-check) | 核对投标人资格条件核对表的要求内容、实际情况与证明材料是否三者闭环，逐条指出哪栏缺什么；不核验原件，也不认定资格 | compliance / tender |
| [dsh-contract-stance](https://github.com/PerryLink/dsh-contract-stance) | 核对合同条款立场台账的条款原文摘录、本方立场与必保条款退让底线，指出哪行哪栏差什么；不改原件，不判合同是否有效 | compliance / tender |
| [dsh-protest-deadline](https://github.com/PerryLink/dsh-protest-deadline) | 核对质疑与投诉台账的提出与答复日期先后、答复是否超出自填期限，逐条指出哪栏差什么；不判质疑是否在法定期限内提出 | compliance / tender |
| [dsh-rulefile-check](https://github.com/PerryLink/dsh-rulefile-check) | 核对规则库自身的编号唯一性、依据字段齐全、摘录长度与来源链接，逐条指出哪一条哪一栏差什么；它检查的是家族自定的引用纪律 | compliance / tender |
| [dsh-tender-extract](https://github.com/PerryLink/dsh-tender-extract) | 核对招标条款摘录表的出处、原文栏与提炼要求共同词、类别取值与序号唯一性，指出哪行哪栏差什么；只看摘录表，不能证明漏摘 | compliance / tender |
| [dsh-tender-matrix](https://github.com/PerryLink/dsh-tender-matrix) | 核对评标因素评分矩阵的单项上限、分值合计与评分依据，逐行指出哪行哪栏差什么；不判断评分是否恰当、谁应当中标 | compliance / tender |
| [dsh-eia-guide-check](https://github.com/PerryLink/dsh-eia-guide-check) | 核对环评导则适用性核对表的导则名称编号、状态取值与执行标准是否可追溯，指出哪栏差什么；不判评价等级与预测模型是否适用 | compliance / construction |
| [dsh-guard-plan-qc](https://github.com/PerryLink/dsh-guard-plan-qc) | 把一份劳保用品配置表逐行核对，按随包 6 条规则查品名规格是否填写、配置数量能否由配置人数推出；只列差异，不判防护是否适用 | compliance / construction |
| [dsh-hazplan-check](https://github.com/PerryLink/dsh-hazplan-check) | 把一份 HAZOP 分析表逐行核对，查必填栏目、引导词取值与每个偏差能否由旁边的工艺参数推出；核对核心是纯函数，不联网、不调模型 | compliance / construction |
| [dsh-permit-report-check](https://github.com/PerryLink/dsh-permit-report-check) | 把行政许可办理台账逐行核对，查受理日期是否不晚于决定日期、决定结果是否出自配置口径、办结记录有无许可证号；许可决定留给审批人 | compliance / construction |
| [dsh-safety-brief-check](https://github.com/PerryLink/dsh-safety-brief-check) | 把安全技术交底记录核一遍，查被交底人是否都在签字名单内、交底日期是否不晚于施工日期、工种是否覆盖实际参建；规则库解析失败即报错 | compliance / construction |
| [dsh-site-log-check](https://github.com/PerryLink/dsh-site-log-check) | 把一份监理资料导出核一遍，查服务期内哪几天没有日志、同一日是否重复出日志、声明的旁站是否都有记录；14 条规则各带条款出处 | compliance / construction |
| [dsh-soilwater-check](https://github.com/PerryLink/dsh-soilwater-check) | 把土壤与地下水监测台账逐行核对，查结果能否解析为数值、超标判定是否与台账自记限值相符；不自带限值，也不核对限值取自哪个标准 | compliance / construction |
| [dsh-essay-rubric-check](https://github.com/PerryLink/dsh-essay-rubric-check) | 把一份作文评分表逐项核对，查每项得分是否超出该项分值、各项合计是否等于量表总分、给分的项是否留下原文定位；只看评分表不看作答 | compliance / research |
| [dsh-learning-gap-check](https://github.com/PerryLink/dsh-learning-gap-check) | 把能力差距与培养计划台账逐行核对，查差距是否等于要求等级减现有等级、超阈值项是否写了培养措施与责任人期限；不判员工是否胜任 | compliance / research |
| [dsh-nsfc-form-check](https://github.com/PerryLink/dsh-nsfc-form-check) | 核对国自然申请书的正文行与文档属性，按本机构名单报出身份词出现在哪一行、四个属性各写了什么；不解析 .pdf，发现只作技术性观察 | compliance / research |
| [dsh-paper-doc-adapter](https://github.com/PerryLink/dsh-paper-doc-adapter) | 把试卷解析结果逐题核对，查各题分值合计是否等于表头总分、题型与难度是否落在配置范围内、题目标识是否唯一；只列结构差异 | compliance / research |
| [dsh-policy-brief-draft](https://github.com/PerryLink/dsh-policy-brief-draft) | 把政策专报要素核对表逐节核对，查每节是否有核心观点与出处、数据截止日期是否落在配置的新鲜度窗口内；不判观点是否正确 | compliance / research |
| [dsh-archive-check](https://github.com/PerryLink/dsh-archive-check) | 把归档登记表逐行核对，查著录栏目是否填写、档号是否唯一、件号是否连续、保管期限是否用本机构期限表的用词；不判合规、不改原件 | compliance / government |
| [dsh-gongwen-flow-check](https://github.com/PerryLink/dsh-gongwen-flow-check) | 把收文登记与办理环节台账逐行核对，查每个环节有无承办人、收发文日期是否先后成立、办结是否落在台账自记期限内；规则逐条引用条例原文 | compliance / government |
| [dsh-gongwen-word-check](https://github.com/PerryLink/dsh-gongwen-word-check) | 把公文台账逐份核对，查发文字号是否为机关代字〔年份〕序号、文种是否出自本机关取值清单、标题有无残留占位符；只查台账登记的文字 | compliance / government |
| [dsh-evidence-check](https://github.com/PerryLink/dsh-evidence-check) | 把证据清单逐份核对，查每份证据是否写明名称与待证事实、取得日期是否不晚于提交日期、证据编号是否唯一；不判真伪与能否采信 | compliance / legal |
| [dsh-lawcite-adapter](https://github.com/PerryLink/dsh-lawcite-adapter) | 把法条引用清单逐处核对，查是否写明法律名称与条号、条号是否写成规范中文形式、效力状态是否出自本机构取值；不核法条现行有效 | compliance / legal |
| [dsh-pleading-draft](https://github.com/PerryLink/dsh-pleading-draft) | 把起诉状要素核对表逐项核对，查每项诉请是否写明事实依据、证据与法律依据、写了金额的是否也写履行期限；不判诉请能否获支持 | compliance / legal |
| [dsh-icd-rule-check](https://github.com/PerryLink/dsh-icd-rule-check) | 把病案首页的编码记录逐份核对，查诊断是否符合 ICD-10 形式、手术操作是否符合 ICD-9-CM-3 形式、星号是否与剑号成对；不查编码目录 | compliance / medical |
| [dsh-medrec-qc](https://github.com/PerryLink/dsh-medrec-qc) | 把病案首页导出表逐行核对，查必填栏是否填写、入出院时间是否精确到分钟且不倒置、实际住院天数是否与日期一致；每条差异带条款出处 | compliance / medical |
| [dsh-nurse-record-check](https://github.com/PerryLink/dsh-nurse-record-check) | 核对一次住院的护理记录、医嘱与评估表导出，查抢救记录是否在结束后 6 小时内补记、临时医嘱有无执行时间与签名；规则库可整体替换 | compliance / medical |
| [dsh-soe-decision-check](https://github.com/PerryLink/dsh-soe-decision-check) | 把三重一大决策事项台账逐行核对，查每个议题有无决议结论、前置研究日期是否不晚于会议审议日期、已决议议题有无表决结果；缺的不补不猜 | compliance / governance |
| [dsh-sop-sync-check](https://github.com/PerryLink/dsh-sop-sync-check) | 把作业规程台账与其引用的 PFMEA、控制计划对齐，查所引版本是否与台账记录的现行版本一致、填了参数的是否也填公差；依据封顶 warn | compliance / governance |
| [dsh-bid-health-check](https://github.com/PerryLink/dsh-bid-health-check) | 把招标要求清单与一份投标 .docx 逐条比对，报出哪些要求有响应、哪些匹配偏弱、哪些定位不到；定位不到不等于没写，命中也不等于满足 | compliance / tender |
| [dsh-canteen-retention-check](https://github.com/PerryLink/dsh-canteen-retention-check) | 把食堂留样台账逐行核对，查四要素是否填写、留样量是否达 125 克、出柜是否满 48 小时；空白格只说台账没记录，不说没留样过 | compliance / safety |
| [dsh-construction-doc-check](https://github.com/PerryLink/dsh-construction-doc-check) | 扫一遍施工项目的资料目录，按相对路径与文件名查 12 类规定资料是否齐全，并报出同资料多版本与零字节文件；只读文件名不打开文件 | compliance / construction |
| [dsh-excel-reconcile](https://github.com/PerryLink/dsh-excel-reconcile) | 把两份表格按配置的主键对齐、逐字段比较，输出报告、JSON 与差异工作簿；金额用整数最小单位比较，主键重复时整键跳过 | data / data |
| [dsh-invoice-ledger](https://github.com/PerryLink/dsh-invoice-ledger) | 把发票台账逐行核对，查同一张发票有无重复入账、价税合计是否等于金额加税额、抬头是否本公司；发票号码全程按字符串保存 | compliance / finance |
| [dsh-payroll-audit](https://github.com/PerryLink/dsh-payroll-audit) | 给一张工资表逐行重算应缴与应发，再拿已公开的社保、公积金与个税参数比对基数上下限与累计预扣；参数未取到即列入未核验 | compliance / finance |
| [dsh-safety-ledger-check](https://github.com/PerryLink/dsh-safety-ledger-check) | 把施工安全教育与资格台账逐行核对，查岗前学时是否达 24 学时、培训记录四要素是否齐全、证书当日是否仍在有效期；不验证证书真伪 | compliance / construction |
| [dsh-table-ingest](https://github.com/PerryLink/dsh-table-ingest) | 把 .docx、.xlsx、.csv 等文件转成规则检查器可直接消费的表格 JSON，给出列名、行与置信度、预览；抽不出表时给候选与原因，不猜 | data / data |
| [dsh-tender-requirements](https://github.com/PerryLink/dsh-tender-requirements) | 读一份招标 .docx 的前附表与正文，抽出时间、保证金、投标文件组成与正副本份数，按三队列装进要求包；未检索到不等于文件里没有 | business-ops / tender |

## 6. Domain operations

领域运营：把财务、法务、贸易、HR、建筑、零售等一类单据做成可重复跑的本机流程，产出工作底稿而不是聊天结论。

| 仓库 | 它做什么 · 关键差异 | 分类 |
|---|---|---|
| [dsh-einvoice](https://github.com/PerryLink/dsh-einvoice) | 把本地 OFD/XML 电子发票解析成八字段台账，按主体与期间查重、归集并归档；不联网、不改原件，金额用整数分勾稽 | business-ops / finance |
| [dsh-bankrec](https://github.com/PerryLink/dsh-bankrec) | 把银行流水与总账按金额相同且日期相差不超三天逐笔勾对，导出 Bank / GL / Matches 三表 xlsx 底稿；不联网、不改原文件，不替你下审批结论 | business-ops / finance |
| [dsh-ap-three-way](https://github.com/PerryLink/dsh-ap-three-way) | 把发票行逐行对上采购单与收货单，按默认 1% 价格容差分出可过账与例外并导出两表 xlsx 底稿；只做本地匹配，不改任何单据 | business-ops / finance |
| [dsh-travel-recon](https://github.com/PerryLink/dsh-travel-recon) | 把差旅行程、发票、卡流水三份 CSV 按 trip_id 逐单匹配，列出重复报销、金额不符、缺发票与每日超限并导出 xlsx 台账；只读检查，不审批不打款 | business-ops / finance |
| [dsh-legal-intake](https://github.com/PerryLink/dsh-legal-intake) | 把 EML 法务需求邮件按 Message-ID 去重、归入六类需求类型，导出 Excel 台账；不连邮箱、不联网，也不出法律意见 | business-ops / legal |
| [dsh-legal-clause](https://github.com/PerryLink/dsh-legal-clause) | 把合同纯文本按行首编号切成条款树，对齐 12 项关键条款 playbook 并列出缺项与编号重号跳号；只做静态检查，不出法律意见 | business-ops / legal |
| [dsh-ghg](https://github.com/PerryLink/dsh-ghg) | 把全年电费台账（CSV 或文本型 PDF）按电网因子折成范围二 tCO2e 并逐行复算，导出底稿与部分 ESRS E1 包；不联网，不做正式鉴证 | business-ops / esg |
| [dsh-qms-capa](https://github.com/PerryLink/dsh-qms-capa) | 把 NCR 不良记录按五个字段去重入库、解析批次别名、评估库存与途中影响，再开 CAPA 或 8D；不连 MES，不替你判根因 | business-ops / quality |
| [dsh-hs-candidate](https://github.com/PerryLink/dsh-hs-candidate) | 把产品描述按公开关键词表给出 Top-3 HS 候选与 GIR 依据，并列出 12 项归类要素缺项；只做候选与结构检查，不做海关裁定 | business-ops / trade |
| [dsh-freight-audit](https://github.com/PerryLink/dsh-freight-audit) | 把运费账单逐票对上版本化费率卡，以分为单位算出多收少收并导出底稿与争议 CSV；不改原账单，不替代正式索赔 | business-ops / logistics |
| [dsh-docx-redline](https://github.com/PerryLink/dsh-docx-redline) | 把本地 .docx 的 OOXML 包按部件算 SHA-256 与 13 项结构计数，并对两版正文做段落级比对；不写修订痕迹、不改原件 | content / documents |
| [dsh-ifc-qto](https://github.com/PerryLink/dsh-ifc-qto) | 把本地 IFC 文本里的墙、板、门窗等构件与 IfcQuantity 工程量按计量类型汇总成 CSV；只做文本清点，不做几何核量 | data / construction |
| [dsh-policy-ledger](https://github.com/PerryLink/dsh-policy-ledger) | 安装第三方 DSH 包前从本地 npm tarball 抽出声明能力并折算 R0–R3 风险，安装失败时把日志归因到阶段与根因；只读诊断，不执行包内代码 | developer-tools / plugin-install |
| [dsh-pim-lint](https://github.com/PerryLink/dsh-pim-lint) | 把商品目录 CSV 逐行查重复 SKU、GTIN 校验位与价格精度，按 SKU、字段、错误码列成问题清单；只读不落盘，不做合规背书 | data / retail |
| [dsh-eval-pack](https://github.com/PerryLink/dsh-eval-pack) | 把评测包逐条按规范化 JSON 精确比对，给出通过率、失败项与无偏 pass@k；纯函数只读评分，不运行被测对象 | developer-tools / evaluation |
| [dsh-finops-suite](https://github.com/PerryLink/dsh-finops-suite) | 把电子发票、银行对账、三单匹配与差旅对账四个成员钉在同一组精确版本上装齐，装完核对是否 4/4 可解析；套件无工具面，不读单据 | business-ops / finance |
| [dsh-contract-suite](https://github.com/PerryLink/dsh-contract-suite) | 把合同需求收件与条款 playbook 审查两个成员钉在同一组精确版本上一起装，装完核对是否 2/2 可解析；套件无工具面，不审合同 | business-ops / legal |
| [dsh-provider-params](https://github.com/PerryLink/dsh-provider-params) | 把 11 家厂商的请求参数互相映射并列出被改名、丢弃与夹取项，再按固定策略修复坏 JSON；不联网、不编造值 | developer-tools / runtime |
| [dsh-pdf-table](https://github.com/PerryLink/dsh-pdf-table) | 把带文本层 PDF 的表格按坐标还原成行列并导出 RFC 4180 转义的 CSV；不做 OCR、不联网，原 PDF 只读 | data / document |
| [dsh-contract-renewal](https://github.com/PerryLink/dsh-contract-renewal) | 把合同编号、对方、起止日与续签窗口登记到本地，按 as_of 分出已过期、续签窗口与 N 天内到期三组并导出 CSV；只算日期，不解析正文、不发提醒 | business-ops / legal |
| [dsh-rfq-compare](https://github.com/PerryLink/dsh-rfq-compare) | 把多家供应商对同一批物料的报价按占位汇率折成 CNY，排出最低价、价差与交期并标出低于成本、超预算与已过期；不联网、不自动淘汰 | business-ops / procurement |
| [dsh-labor-contract](https://github.com/PerryLink/dsh-labor-contract) | 把劳动合同正文核对九项必备条款、试用期上限与试用期工资 80% 下限，并批量体检员工合同 CSV，导出带 sha256 的问题清单；不构成法律意见 | business-ops / hr |
| [dsh-progress-payment](https://github.com/PerryLink/dsh-progress-payment) | 把本期进度款申报按合同基准逐项核对量与单价，用整数分算出本期与累计金额及累计比例，导出审核底稿 CSV；不判变更签证与索赔 | business-ops / construction |
| [dsh-ar-aging](https://github.com/PerryLink/dsh-ar-aging) | 把应收明细 CSV 按开票日算账龄、按到期日算逾期，出固定五桶账龄表、客户汇总与 Top 逾期客户并导出 CSV；单币种，不做核销与坏账 | business-ops / finance |
| [dsh-import-customs-check](https://github.com/PerryLink/dsh-import-customs-check) | 把发票、装箱单、提单、报关单四份 JSON 的 9 个表头字段逐项对照，并列出报关单 12 项要素缺项；只核对表头，不做归类裁定 | business-ops / trade |
| [dsh-ar-collection](https://github.com/PerryLink/dsh-ar-collection) | 把应收明细按 7/15/30 天提醒阶梯排出客户催收优先级，生成中文催收函草稿与清单 CSV；只写本地草稿，不发送、不算利息 | business-ops / finance |
| [dsh-settlement-docs](https://github.com/PerryLink/dsh-settlement-docs) | 把资料清单与实际提交清单逐项对齐，列出缺件、份数不足、未签字盖章并算出齐套率，导出核对表 CSV；只看文件名与签章标记，不读内容 | business-ops / construction |
| [dsh-attendance-check](https://github.com/PerryLink/dsh-attendance-check) | 把打卡明细按 8 小时标准工时、单日 3 小时与月 36 小时加班上限逐日核对，输出超限、缺卡与休息不足并导出核对表 CSV；不算工资，周末行跳过 | business-ops / hr |
| [dsh-store-replenish](https://github.com/PerryLink/dsh-store-replenish) | 把门店-SKU 销售库存表按日均销量乘补货周期与安全天数再减库存与在途算出缺口，取整到起订量并出补货 CSV，标出滞销与缺货风险；不下采购单 | business-ops / retail |

## 7. Phocinae

Phocinae（斑海豹）是独立的一条决策线：百 M 级非生成式模型在本机做是/否、分类、路由与评分，不写作文、不调云 API。

| 仓库 | 它做什么 · 关键差异 |
|---|---|
| [dsh-phocinae](https://github.com/PerryLink/dsh-phocinae) | 把工具调用送进本机 150M 非生成式模型，按答案映射成 allow / ask / deny；只判断不生成，服务不可达时转人工 |
| [phocinae-server](https://github.com/Phocinae/phocinae-server) | 把决策模型用纯 torch 前向跑成本机 /v1/systemone 服务，一次请求回答 noul / choice / score；不做 chat 与 OpenAI 兼容 |
| [phocinae-guard](https://github.com/Phocinae/phocinae-guard) | 用单文件 guard.py 给每条 shell 命令出放行、拒绝或需人工确认的判定；纯标准库零依赖，L0 黑白名单在服务挂掉时仍生效 |
| [phocinae-mcp](https://github.com/Phocinae/phocinae-mcp) | 把 gate、classify、route、score 四项能力暴露成 MCP 工具，供只读 MCP 的编码代理直接调用；新旧两代协议并存 |
| [phocinae-cli](https://github.com/Phocinae/phocinae-cli) | 用一行终端命令对接本机 phocinae-server，执行 ping、decide 与 gate 判定；推理全在本机、不上云，结果以退出码返回 |
| [phocinae-js](https://github.com/Phocinae/phocinae-js) | 用一行 TypeScript 调用本机决策服务并拿回结构化答案；零运行时依赖、全类型化，内置与 guard 同源的 L0 离线门 |
| [phocinae-rulepack](https://github.com/Phocinae/phocinae-rulepack) | 读入台账、套用指定版本的规则包，只把差异项留给人工复核；模型调用为零、无第三方运行时依赖，判定只由规则包版本决定 |
| [phocinae-formulate](https://github.com/Phocinae/phocinae-formulate) | 把同一个判断用多种问法各跑一遍已标注命令集，量出破坏性命令召回与例行命令误拦；用数字决定该用哪种问法，而不是凭直觉 |
| [phocinae-publish-gate](https://github.com/Phocinae/phocinae-publish-gate) | 在媒体交付物发布前量出目标的一组事实并交给 phocinae-rulepack 引擎裁决；只测量、从不写入目标，也不自己下结论 |
| [dsh-evidence](https://github.com/Phocinae/dsh-evidence) | 把提交信息里「测试通过」这类主张与本次会话真实跑过的记录比对，指出对不上的地方；不调模型、不联网、不留台账，只拦自述比事实快半步的情形 |
| [dsh-batch-triage](https://github.com/Phocinae/dsh-batch-triage) | 先给每张工单跑确定性预筛，规则能定的直接归类、定不了的交人工而不是悄悄归为常规；模型档尚未接入，相关字段如实报 unavailable |
| [dsh-context-verdict](https://github.com/Phocinae/dsh-context-verdict) | 给出上下文压缩的丢失裁决，safe_to_compact 表示记录里没有未落盘的东西；digest 只做完整性检查，防的是意外而不是蓄意绕过 |

## 8. Catalogs and install surfaces

目录与安装面：哪份清单算权威、一条命令装哪套、站点和门户各自吃什么数据。

| 仓库 | 它做什么 · 关键差异 |
|---|---|
| [dsh-kit](https://github.com/PerryLink/dsh-kit) | 一条命令装好仍在维护的家族插件，冻结件保持可装；同时是主线名册，装哪些、什么状态以仓里的清单一处为准 |
| [dsh-catalog](https://github.com/PerryLink/dsh-catalog) | 旧入口：GitHub 现在 301 重定向到 dsh-family-catalog（同一仓、同一份产物），仅保留旧链接可达 |
| [dsh-family-catalog](https://github.com/PerryLink/dsh-family-catalog) | DSH Desktop Market 的标准目录源：从 npm registry 生成目录清单并逐条按公开 v1 契约校验，每条带中英名称与中文摘要 |
| [dsh-plugin-portal](https://github.com/PerryLink/dsh-plugin-portal) | 把插件清单渲染成一页分组卡片，显示仓库名、一句话简介、星数与徽章；零依赖静态页、无构建步骤，数据取自 repos.json |
| [dsh-plugins](https://github.com/PerryLink/dsh-plugins) | 家族站点的内容源：域插件分类（TAXONOMY.md）、市场清单（market/）与名册（ROSTER.md）都在这里；只收公开或合成样例 |

## 9. Frozen, moved and retired

冻结 = 停兼容更新但已装可用；迁移 = 旧仓只留指针；退役 = 宿主已原生提供同类能力。

### 冻结（8）

| 仓库 | 状态 |
|---|---|
| [dsh-autotier](https://github.com/PerryLink/dsh-autotier) | 🧊 冻结 — 按每个 turn 的确定性信号选强档或廉价档，只有低置信时才问裁判模型；弱档执行时拒绝破坏性命令并提示先升级，守卫出错则升级而非放行 |
| [dsh-budget](https://github.com/PerryLink/dsh-budget) | 🧊 冻结 — 把每次会话的预算、碳足迹与延迟算进一个面板，超限时在流上给出修正性错误而不编造模型输出；不改写请求，配置非法在挂载时即失败 |
| [dsh-cert-mcp](https://github.com/PerryLink/dsh-cert-mcp) | 🧊 冻结 — 以只读 MCP 服务暴露插件认证登记表：认证等级、快照日期与五维证据；零运行时依赖，走 stdio |
| [dsh-claude-move](https://github.com/PerryLink/dsh-claude-move) | 🧊 冻结 — 把 Claude Code、Codex、OpenCode 与 Hermes 的会话、记忆、技能和斜杠命令复制成可续聊的 DSH 会话；源文件只读、写入过审批门 |
| [dsh-community-bench](https://github.com/PerryLink/dsh-community-bench) | 🧊 冻结 — 开一个应用内 Community Bench 页签，展示 dsh-score 的公开证据层，读所有人同一份公开登记表；不做本地打分、不发遥测 |
| [dsh-defend](https://github.com/PerryLink/dsh-defend) | 🧊 冻结 — 在官方 seam 上为提示注入、越狱与密钥泄露给出 deny / ask / block 决策；规则裁决已知模式，其余交检测层，失败关闭 |
| [dsh-draw](https://github.com/PerryLink/dsh-draw) | 🧊 冻结 — 把静态图像生成收成一个工具、多个引擎的路由，按健康度回退并记账用量；凭据以 apiKeyRef 引用环境变量，配额在调用引擎前检查，耗尽时给完整尝试记录 |
| [dsh-reach](https://github.com/PerryLink/dsh-reach) | 🧊 冻结 — 把任意工作区的审批与提问卡推到微信、Telegram、飞书等 IM 通道，让人在聊天里直接答复；首位发送者成为 owner、白名单为空即拒绝所有人，默认失败关闭 |

### 迁移指针

| 仓库 | 现在 |
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
| [dsh-plugin-upgrade-015](https://github.com/PerryLink/dsh-plugin-upgrade-015) | [dsh-codemod](https://github.com/PerryLink/dsh-codemod)（该升级包已退役） |
| [dsh-plugin-upgrade-016](https://github.com/PerryLink/dsh-plugin-upgrade-016) | [dsh-codemod](https://github.com/PerryLink/dsh-codemod)（该升级包已退役） |

### 退役（3）

| 仓库 | 退役原因 |
|---|---|
| [dsh-background-agents](https://github.com/PerryLink/dsh-background-agents) | harness 已原生支持可续子代理 |
| [dsh-session-pin](https://github.com/PerryLink/dsh-session-pin) | harness 已原生支持会话置顶 |
| [dsh-team-rooms](https://github.com/PerryLink/dsh-team-rooms) | harness 已原生支持 Agent Teams |


## 10. Research suite (catalog-only, 19)

> 2026-11-08 发布的科研插件套件：已进 DSH Desktop Market catalog 与 `data/discovery.json`，但**未进** `dsh-kit/plugins.txt` 安装名册。它们不计入上文的 137 行；npm 名为 `@perrylink/dsh-claim-check` / `@perrylink/dsh-research-core` 的两个包使用 scope，其余为同名。

| 仓库 | 它做什么 · 关键差异 |
|---|---|
| [dsh-cite-verify](https://github.com/PerryLink/dsh-cite-verify) | 核验一条引用确实存在——并核验它的元数据是否正确。DOI / PMID / arXiv / BibTeX → 数据源自己的回答、逐字段核对、内容寻址的快照与 REP 证据记录。 |
| [dsh-claim-check](https://github.com/PerryLink/dsh-claim-check) | 来源原文是否真的支持这条断言？逐字节、确定性、可复算：逐字片段、数字、带标签的数值、否定与限定。转述按 insufficient 处理，绝不报“支持”。 |
| [dsh-dataset-card](https://github.com/PerryLink/dsh-dataset-card) | 发布数据集时附上一份 Datasheet——并在发布前搞清楚个人数据在哪里。对 CSV/TSV/JSON/JSONL 做画像，按列名与脱敏值模式标记疑似 PII，拒绝把原始行存为证据。 |
| [dsh-doc-anchor](https://github.com/PerryLink/dsh-doc-anchor) | 把 PDF / HTML / LaTeX / Markdown 文档变成可定位的证据。它不做阅读器、渲染或翻译——只提供坐标、不可变快照，以及一份任何人都能复核的证据记录。 |
| [dsh-dmp](https://github.com/PerryLink/dsh-dmp) | 一份说得清数据放在哪里、谁能动、资助结束后如何处置的数据管理计划。十节脚手架，每节带提示语；检查个人数据与开放共享、最短保存期、备份、仓库/许可证/DOI。 |
| [dsh-image-integrity](https://github.com/PerryLink/dsh-image-integrity) | 这张子图是不是被复用了——原地重复，还是从另一张图镜像粘贴过来？零依赖 PNG 解码、带 NCC 确认的均值阈值块指纹、重复/镜像区域报告与 SARIF。 |
| [dsh-irb](https://github.com/PerryLink/dsh-irb) | 赶在伦理委员会之前把申请材料准备好——并知道哪些核心陈述还缺着。18 项关键词清单、建议性风险等级与对应保障措施，可导出 Markdown + SARIF。 |
| [dsh-lit-watch](https://github.com/PerryLink/dsh-lit-watch) | 这次检索相比上次新增了什么——而且只报新增。保存带时间窗口的 Crossref 检索；用已见 DOI 库保证重复运行只返回真正新增的条目。 |
| [dsh-grant-cn](https://github.com/PerryLink/dsh-grant-cn) | 投稿/申报前：本子的检查清单是否齐、预算算术是否对、材料包是否真的打包了？面向中文基金申请书的 19 项结构/属性/声明检查、预算算术与材料包扫描。 |
| [dsh-manuscript-check](https://github.com/PerryLink/dsh-manuscript-check) | 投稿前：稿件是否完整、指南要求报告的内容是否都报告了、投稿包是否真的打齐了？关键词检查清单 + CONSORT/STROBE/PRISMA 起步条目覆盖 + 投稿目录扫描。 |
| [dsh-notebook-capture](https://github.com/PerryLink/dsh-notebook-capture) | 能在你机器上跑通的 notebook，还不等于可复现。不执行、只读取 .ipynb：内核、执行顺序、import、运行时安装、随机种子、绝对路径、输出状态与哈希。 |
| [dsh-meta-analysis](https://github.com/PerryLink/dsh-meta-analysis) | 把效应量合并起来——每一步算术都能逐行核对。效应量换算、固定效应与 DerSimonian–Laird 随机效应合并、Q / I² / τ²、森林图数据与轻量 Egger 检验。 |
| [dsh-response-letter](https://github.com/PerryLink/dsh-response-letter) | 每一条审稿意见都有回复——而且可以按编号核实。解析审稿意见（Reviewer/Referee/审稿人 标题行），检查回复信的缺失、过短、多余、重复，并导出覆盖表。 |
| [dsh-retraction-watch](https://github.com/PerryLink/dsh-retraction-watch) | 你引用的论文，后来有没有被撤稿或更正？Crossref 工作记录 + 已实测的 filter=updates:<doi> 查询、逐 DOI 状态、追加式时间线与 REP 证据。 |
| [dsh-repro-audit](https://github.com/PerryLink/dsh-repro-audit) | 别人能复现这项分析吗——以及从你记录至今，有没有东西发生漂移？有界只读扫描记录 commit、lockfile、环境、数据哈希、图表、seed 与运行命令。 |
| [dsh-source-cnki](https://github.com/PerryLink/dsh-source-cnki) | 中文文献记录：导入你自己的导出文件，按 GB/T 7714 引用，检查元数据——全程不抓取 CNKI。读取 RIS/EndNote 风格或带标签的文本导出，分配稳定记录 id。 |
| [dsh-sr-ledger](https://github.com/PerryLink/dsh-sr-ledger) | 经得起复核的系统综述账本：只追加、双人筛选、PRISMA 2020、审计可验。记录方案、每条筛选决策、冲突裁决与 RoB/GRADE 评估，再推导 PRISMA 流程。 |
| [dsh-statcheck](https://github.com/PerryLink/dsh-statcheck) | 重算稿件报告的统计数据——并把对不上的那些标出来。这是算术，不是指控：每条 finding 都给出报告的统计量、它实际蕴含的 p 值，以及精确字符位置。 |
| [dsh-research-core](https://github.com/PerryLink/dsh-research-core) | REP v1——DSH 科研插件家族的共享证据协议。一套协议、一个存储、一个校验器：每个科研插件说同一种证据语言，任何人 30 秒内可复算它声称的结论。 |

运行时/领域行的权威来源：[ROSTER.md](https://github.com/PerryLink/dsh-plugins/blob/main/ROSTER.md)。
