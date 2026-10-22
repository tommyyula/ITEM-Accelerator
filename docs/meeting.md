# AI Accelerator 的业务价值实现探讨

Item × ISS Biz Team × COO AI Team

> 面向联想各部门领导的完整阅读资料。会前用十页简版建立共同业务主线，会上用四十页详版展开案例与讨论，会后用本文件查阅完整内容。本文不是已发生会议的纪要；待确认事项不代表已形成的会议决策。


> **共同探讨如何将 ISS Biz Team 的业务知识、COO AI 团队的预测与优化能力，以及 Item 的业务应用与工程能力，转化为可复用、可治理、可持续演进的业务结果。**

---

## 0. 合作目标：合作不是一次产品交付，而是共同建设业务能力

### 本节大纲

- 面向联想各部门的真实业务场景，共同讨论业务结果、能力协同、治理责任与联合产品路径。
- 先讲合作，再讲产品：三方共同把已有业务知识、供应链 AI 能力和应用工程能力串成业务闭环。
- 共同目标自然合并为一条主线：减少重复建设、形成能力协同、通过能力复用触发新的业务创新，并在 ISS Biz Team 真实场景中验证后沉淀为可复制的联合产品。
- 明确会议结束时必须获得的四个确认。

### 0.1 合作主张与三方分工

> 我们今天不是来完成一次孤立的产品交付，也不是来展示一个孤立的平台，也不是来增加更多孤立的 Agent。我们希望和 ISS Biz Team一起，把已经拥有的业务知识、供应链算法和 AI 实践串起来，形成可以真正服务业务、可控上线、可持续复用的能力。
>
> Item 负责应用层、业务场景和产品化；COO AI 团队提供供应链、服务供应链、算法与企业级技术能力；ISS Biz Team 提供真实场景、业务 Owner 和价值验证。我们希望从一组 Hero Cases 开始，逐步沉淀为一套可复制的产品。

### 0.2 合作背景与共同目标

ISS Biz Team 已经有较强的 AI 实践基础和真实业务问题，是联合产品验证的最佳场景。COO AI 团队拥有供应链与服务供应链场景、预测与优化算法、企业级数据与技术资源，以及与 ISS Biz Team 相关的真实业务环境。Item 擅长业务场景理解、物流与供应链应用、SaaS 产品化和 Agent 应用落地。

因此，三方共同目标不是继续增加数量更多、彼此孤立的 Agent，而是从一组高价值 Hero Cases 出发，把分散的 Data、Compute、Model、Agent 和 Skill 串成端到端业务流程，并通过 ISS Biz Team 的业务验证将其沉淀为可治理、可复用、可复制的标准能力。

这条主线同时包含三个相互关联的业务结果：

1. **减少重复建设，降低成本。** 复用已有数据、算力、模型、Agent 和 Skill，避免不同团队重复开发相似能力。
2. **让已有能力形成协同。** 让数据、算力、Model、Agent 和 Skill 在统一业务语义下彼此连接，形成“1+1 大于 2”的业务价值。
3. **通过能力复用触发创新。** 把已经验证的能力组合到新的流程、服务和业务生态中，推动新的业务模式与联合产品。

### 0.3 今天要展示和讨论的内容

- 一套从 Ontology 到 Agent、从 Data 到 Model、再到 Action 的架构；
- 一组分别证明流程自动化、业务应用生成、复杂决策、知识沉淀和商业化潜力的案例；
- 两套面向不同用户角色的 Business Oriented Tools；
- Ontology Studio 如何成为知识、模型、Agent 和 Action 的共同起点；
- 一个从知识挖掘、能力基座准备、典型 Agent 共建，到训练、产品化和外部推广的合作计划。

### 0.4 会议结束必须获得的四个确认

1. **确定首批 Hero Cases 组合。** 建议将 BO / Customer Promise 作为优先候选，同时评估 CEC SOP、WMS 等场景的组合，明确各案例的业务问题、边界和价值指标。
2. **确定参与团队和业务 Owner。** 至少覆盖 CEC、eSVC、UKM、SSC / GPO、Global Logistics、Field Service 等相关团队中的实际责任人。
3. **确定能力准备清单。** 明确数据、知识、模型、Connector、Tools、Action、权限、安全、部署、日志和评估要求。
4. **确定联合推进方式。** 明确知识挖掘、Ontology 共建、Agent 共建、培训推广、产品化和下一决策门的责任矩阵。

会议不只是要获得“大家认可方向”，而是要让这四个确认可以在会后转化为 Owner、输入、产出和时间边界。

### 0.5 为什么现在需要合作

ISS Biz Team 已经有不少 Agent 和自动化实践，问题不是“有没有 AI”，而是 Agent 分散在不同团队和地区，业务流程之间存在断点，一线知识没有稳定沉淀为组织能力，复杂决策不能只依赖自然语言模型，组织层面的收益、采用率和复用情况也缺少统一衡量。

因此，下一阶段的重点应从“继续做更多 Agent”转向选择高价值场景、建立统一业务本体和数据上下文、连接预测与优化、用治理和门户把 Agent 串起来，并将成功实践产品化。


---

## 1. 总体架构：让业务、知识、模型和行动连成一条链

### 本节大纲

1. 业务人员有什么问题？
2. 系统需要知道什么？
3. 系统需要如何判断？
4. 系统可以执行什么？
5. 谁来构建、谁来审核、谁来使用？
6. 如何统计效果并持续优化？

业务链路从 CEC、eSVC、UKM、Field Service、SSC / GPO、Global Logistics、RMC / Pass 等业务上下文出发，经由 Ontology、Data、Model、Connector 和 Tools，最后进入 Agent、Business Interface 和 Action。


### 1.1 推荐的架构叙述

不要一上来按产品名称讲，而是按业务问题拆解：

1. **业务人员有什么问题？**
2. **系统需要知道什么？**
3. **系统需要如何判断？**
4. **系统可以执行什么？**
5. **谁来构建、谁来审核、谁来使用？**
6. **如何统计效果并持续优化？**

### 1.2 六层架构

#### 第一层：Business Context

这里承载 ISS Biz Team 的组织、角色、业务流程和价值指标：

- CEC：客户电话和人工坐席；
- eSVC：网站、Chatbot、e-ticket、Email；
- UKM：诊断知识、Service Menu、换件建议；
- Field Service：现场服务和维修执行；
- SSC / GPO：服务供应链、Supply Planning、物料；
- Global Logistics：物流执行和运输节点；
- RMC / Pass：维修、订单和服务闭环。

#### 第二层：Ontology Studio

把业务场景中的对象、关系、规则和行动定义出来。例如 BO 场景至少需要理解：

- Customer；
- Order；
- Back Order；
- Part；
- Inventory；
- Substitute Part；
- Repair Case；
- Shipment；
- ETA；
- Service Promise；
- Priority；
- Action。

Ontology 的关键不是列出名词，而是定义这些对象如何相互影响，以及在什么条件下可以执行什么动作。

#### 第三层：Data Hub

Data Hub 负责把事实和上下文接入：

- CRM / Order 数据；
- 维修和 Field Service 数据；
- 物料、库存和供应链数据；
- 物流节点、运输状态和 ETA 数据；
- UKM / EKP / EKF 知识；
- SOP、PRD、邮件、会议记录和历史案例；
- 必要时包括代码库、音视频和其他多模态资料。

#### 第四层：Model Hub

Model Hub 负责提供适合业务场景的判断和计算能力。结合 COO AI 团队的供应链 AI 材料，可以将技术分为三类：

**场景建模：**

- 场景聚合建模；
- 时序数据结构化建模；
- 基于图网络的物流模型；
- 用户需求变化的时空模型；
- 产品或设备生命周期模型；
- 产能多变量干预模型；
- 物流网络拓扑模型。

**决策支持：**

- Le-TSFM 等时序预测基础模型；
- Router-based Hybrid Forecast；
- 全局性的结构化层级预测；
- 协同相关性自动分析；
- 基于信息或置信区间的预测解释；
- 需求预测、产能预测、销售预测、补货、物流 ETA 和故障诊断。

**优化决策：**

- Le-OPT 优化求解器；
- 混合强化学习的多目标优化；
- 多目标量级同构策略算法；
- 基于重心梯度的 3-D Bin Packing 算法；
- 知识增强的因果推理；
- 生产料件预留、APS、多工厂订单分配、备件计划、库存优化、网络路径和装箱优化。

对 ISS Biz Team 工作坊不需要逐项解释算法，而应说明：

> 大模型负责理解、协作和解释；时序模型负责预测；优化算法负责在约束条件下求解；Ontology 和规则负责限定可控范围；Agent 负责把这些能力编排成业务流程。

#### 第五层：Connector 与 Tools

- Connector 连接系统、数据和外部服务；
- Tools 封装 API、MCP、业务查询和业务 Action；
- 高风险动作需要权限、人工确认和日志；
- 低风险、重复性强的动作可以自动执行。

#### 第六层：Agent 与 Business Interface

- Agent Factory：构建、编排、测试、Qualification 和 Logging；
- ITEMGPT Runtime：业务人员使用、配置和运行；
- ISS Dashboard：面向人的入口和业务可视化；
- Marketplace：属于技术能力层，面向 Agent 提供能力发现、复用和治理。

---

---

## 2. 典型案例的推荐讲法

### 本节大纲

每个案例只承担一个主要证明任务：

- 港口拖柜：证明无头 Agent 可以真正跑流程；
- WMS Dynamic Form：证明业务人员可以快速构建应用；
- BO / Customer Promise：证明跨组织数据、预测、优化和 Action 可以形成 Hero Cases；
- BNP → Dynamic Form → PEI：证明从业务建模到复杂业务生态的扩展能力；
- Record & Reply → CEC SOP：证明一线经验可以沉淀为组织知识；
- eSVC Small Model：证明小模型、路由与 Token Saving 的价值；
- CEC + Genesys AI App：证明内部能力可以走向标准产品与外部商业化。


这些案例不应全部用相同的方式介绍。每个案例承担不同的证明任务。

### 2.1 港口拖柜：证明“无头 Agent 可以真正跑流程”

#### 业务故事

港口拖柜流程涉及打单、监控、派车、状态更新、收付款等多个环节。如果每一步都依赖人工，不仅成本高，也容易出现状态不同步和异常处理延迟。

#### Demo 展示

- 主 Agent 接收一个运输任务；
- 自动拆解为多个子 Agent；
- 子 Agent 分别处理订单、监控、派车、状态和结算；
- 状态变化触发后续动作；
- 异常进入人工确认；
- 所有过程可追踪、可回放。

#### 这个案例要证明什么

- 多 Agent 协作不是概念，而是可以承担完整流程；
- Agent 可以在后台运行，不必每一步都由人发起；
- 通过标准化 Tools 和 Connectors，可以把流程变成机器人化执行；
- 这与 ISS Biz Team 的服务供应链、Field Service、物流场景具有迁移关系。

可以补充 Units 场景中后台人员从 570 人减少到 320 人的经验，但正式 Demo 中应明确这是历史案例，不要把它直接承诺为ISS 项目结果。

---

### 2.2 WMS 动态表单：证明“业务人员可以快速做应用”

#### 业务故事

仓储业务经常需要临时表单、异常登记、任务确认、状态采集和现场页面。如果每次都等传统开发，业务响应会很慢。

#### Demo 展示

用户可以用自然语言提出需求，例如：

> 我需要一个用于仓库异常处理的动态表单，能够记录订单、料件、位置、异常类型、照片和处理建议，并在确认后更新状态。

系统生成：

- 动态表单；
- 页面字段；
- 校验逻辑；
- 相关业务流程；
- 后续 Action；
- 与 WMS 或其他系统的连接。

#### 这个案例要证明什么

- ITEMGPT Runtime 可以服务 Citizen Business User；
- 业务人员不需要从零写代码；
- 应用生成不是最终目的，标准化、可复用和可治理才是重点；
- 表单和页面可以与 Ontology、Tools 和企业系统连接。

---

### 2.3 BO 项目：重点 Hero Cases 之一

这是整场 Demo 最重要的业务案例，建议占总 Demo 时间的 25%–35%。

#### 业务痛点

BO 不是一个孤立的订单状态问题，它会涉及：

- 客户是否得到明确承诺；
- CEC 是否能回答客户；
- eSVC 是否能在网站、Chatbot、e-ticket、Email 上提供一致信息；
- Field Service 是否有维修资源；
- UKM 是否提供正确诊断和换件建议；
- GPO 是否有物料和计划；
- Global Logistics 是否能按节点完成运输；
- RMC / Pass 是否完成维修和关闭。

#### 推荐 Demo 场景

选择一个存在缺料或延迟风险的订单：

1. CEC 或 eSVC 收到客户询问；
2. Agent 读取订单、维修、库存、物流和知识信息；
3. Ontology 将不同系统中的字段转换为统一业务概念；
4. Model Hub 预测 ETA 或风险；
5. 优化模型比较料件替换、订单优先级、库存和运输方案；
6. Agent 用业务语言解释原因和推荐方案；
7. 对低风险动作自动执行，对高风险动作请求人工确认；
8. 更新状态并把结果反馈给 CEC、eSVC、Field Service 和客户。

#### BO 不是“聊天机器人”

需要明确强调：

> BO Agent 的价值不在于回答“订单在哪里”，而在于把分散在不同组织和系统中的信息、规则和决策串起来，帮助组织回答“为什么延迟、什么时候可以完成、下一步应该怎么做”。

#### 需要展示的指标

建议显示指标框架，而不是提前承诺数字：

- BO 查询响应时间；
- 重复来电和重复查询量；
- 人工跨团队确认次数；
- ETA / Customer Promise 准确率；
- Order Close 周期；
- 料件替换建议采纳率；
- Action 自动执行率；
- 客户满意度和 NPS。

#### 必须正面回应的风险

Susan 或相关团队可能关注：

- 加约束后模型是否过于僵硬；
- 不加约束时准确性和可控性是否不足；
- 规模化后质量能否保持；
- BO 项目是否只是在减少人头，而没有真正提升客户体验。

建议回应：

- 不同风险等级采用不同自治级别；
- 把预测、优化、规则和大模型分工；
- 高风险 Action 保留人工审批；
- 通过沙盒、版本、测试集和日志验证质量；
- 以 Customer Promise、流程透明度和跨团队协作为核心价值，而不是只看减员。

---

### 2.4 BNP → 动态表单 → PEI：证明“从模型到应用再到复杂业务生态”

由于 BNP 和 PEI 是内部项目名称，正式材料中建议保留内部缩写，并在首次出现时由业务负责人补充全称和背景。

#### 推荐叙事

1. 先从 BNP 的业务对象、流程和规则开始；
2. 通过 Ontology Studio 建立业务模型；
3. 由 Agent Factory 生成或配置业务能力；
4. 通过 ITEMGPT Runtime 生成动态表单和业务页面；
5. 将同一套能力扩展到 PEI 的伙伴、采购或生态流程；
6. 展示从知识到应用、从单点场景到业务网络的扩展能力。

#### 这个案例要证明什么

- Item 不只是搭一个聊天入口；
- 业务建模可以直接转化为可运行的表单和流程；
- 复杂业务可以先拆成可治理的业务对象和 Action；
- 一个场景的建模成果可以迁移到相关项目。

---

### 2.5 Record & Reply → CEC SOP：证明“把一线经验变成组织知识”

#### 业务故事

CEC 坐席每天会产生大量对话和处理经验，但如果只留在个人或一次性对话里，组织无法持续复用。

#### 推荐 Demo 展示

- 录入或导入一段客服交互；
- Record & Reply 提取问题、上下文、处理动作和结果；
- 系统识别是否符合现有 SOP；
- 对缺失或不一致的步骤进行标记；
- 生成结构化 SOP 草稿或知识更新建议；
- 由业务 Owner 审核后进入 UKM / Ontology / Skill；
- 下一次由 CEC Agent 或 Genesys Agent 调用。

#### 这个案例要证明什么

- AI 能把隐性知识转成显性知识；
- 知识不是一次生成，而是“记录—审核—发布—使用—反馈—优化”的闭环；
- Record & Reply 可以与 CEC SOP、UKM 和 Genesys 连接；
- 这正是 Ontology Studio 的输入来源之一。

---

### 2.6 eSVC 小模型：可作为补充案例，不宜单独抢主线

准备清单中有“eSVC small model 情绪？”的方向。这里建议在正式材料中先确认两个问题：

- 该小模型的目标是情绪识别、意图识别、路由，还是其他能力；
- 它是在 eSVC 前端做辅助判断，还是作为 CEC / Genesys Agent 的一个能力组件。

如果确认是情绪或意图相关，可以把它放在 eSVC 案例中，作为：

- 轻量模型承担高频、低成本判断；
- 将请求路由到正确的知识、Agent 或人工队列；
- 通过模型分层降低 Token 消耗；
- 避免所有简单任务都调用大模型。

这个案例适合用来引出 Token Saving、垂直小模型和 Model Hub，不建议单独作为主 Hero Cases。

---

### 2.7 CEC + Genesys AI App：证明“从内部能力到商业化”

#### 推荐叙事

CEC 的成熟能力可以被封装成基于 Genesys 的 AI App：

- 连接客户请求、订单、服务、知识和 SOP；
- 自动检索和解释信息；
- 生成标准回复；
- 推荐下一步处理动作；
- 在权限和审批规则下执行任务；
- 将过程记录、结果和人工修正反馈回知识体系。

#### Agent 无头化

“无头化”不是取消人，而是让重复性和后台性工作由 Agent 自动运行：

- 坐席需要时调用；
- 后台自动监控和补充信息；
- 异常时升级给人；
- 最终由人和 Agent 共同完成 Customer Promise。

#### 商业化引申

这可以进一步引出：

- CSAS Genesys AI App；
- Genesys Marketplace；
- 将 ISS Biz Team 验证过的服务能力包装为标准产品；
- 从内部项目走向联想服务产品和外部客户。

---

---

## 3. 能力底座与 COO AI 团队供应链 AI 的差异化表达

### 本节大纲

- Data Hub 不是更多数据源，而是统一的业务上下文；
- Model Hub 不是模型仓库，而是 Hybrid AI 的服务化协同；
- Connector 与 Tools 让 Agent 从“能理解”走向“能调用、能执行、可审计”；
- Dashboard 面向人呈现收益，Marketplace 面向 Agent 提供能力发现与复用；
- 差异化在于业务 Action、垂直知识、预测优化协同和全生命周期治理；
- 按 Hollis 框架从 Open 走向 Transform、Engineer，并采用阶段性 Agent 治理。


### 3.1 不要把 Data Hub 讲成“更多数据源”

Data Hub 的价值是形成统一上下文：

- 同一个订单在 CEC、物流、维修和物料团队中有一致的业务定义；
- 同一个客户承诺能够被多个 Agent 访问和更新；
- 同一个知识对象能够在 UKM、SOP、Agent 和 Action 中复用。

### 3.2 不要把 Model Hub 讲成“模型仓库”

Model Hub 的价值是让不同类型的模型在同一个业务流程中协同：

- 时序模型负责预测；
- 优化模型负责权衡约束；
- 诊断模型负责归因；
- 小模型负责高频分类和路由；
- 大模型负责理解、解释和多 Agent 协作；
- 规则和 Ontology 负责边界和可控性。

### 3.3 Hybrid AI 是双方合作的技术共识

COO AI 团队供应链 AI 材料中展示的三层结构，可以在 Demo 中简化为：

**数据与知识驱动的场景建模 → 决策支持 → 优化决策**

Item 的价值是在这三层之上增加：

- 业务用户入口；
- Agent 编排；
- 动态表单；
- Action 执行；
- 业务流程串联；
- 结果反馈和治理。

因此，双方的结合不是“Item 接一个联想模型”，而是：

> **COO AI 团队提供预测与优化的决策能力，Item 将其嵌入业务本体、Agent 流程和最终用户体验，ISS Biz Team 提供真实场景和闭环验证。**

---

### 3.4 ISS Biz Team 智能门户：面向人的 Dashboard，面向 Agent 的 Marketplace

这是需要重点讲清楚的概念。

#### Dashboard 面向人

Dashboard 应该帮助业务和管理层回答：

- 哪些 Agent 已上线？
- 哪些团队在使用？
- 采用率如何？
- 哪些流程得到改善？
- 哪些应用带来了 Customer Experience 或效率收益？
- 哪些能力可以复制到其他区域？

它是组织级 AI 价值的可视化入口。

#### Marketplace 面向 Agent

Marketplace 不应只是“人去找工具的商城”，而应是 Agent 自动发现和复用能力的目录：

- Agent；
- Skill；
- MCP Server；
- Tools；
- Models；
- Ontology 和领域能力。

Agent Factory 或 Master Agent 可以根据任务自动找到合适能力，并按权限调用。

#### Dashboard、Marketplace、Factory 与 Runtime 的关系

- Dashboard 让人看到组织发生了什么；
- Marketplace 让 Agent 找到可以复用什么；
- Agent Factory 让专业人员建设和治理什么；
- ITEMGPT Runtime 让业务人员使用和配置什么。

---

---

## 4. 两套 Business Oriented Tools 的详细定位

### 本节大纲

- ITEMGPT Runtime：让 Citizen Business User 用起来、配置起来；
- Agent Factory：让 DT、FDE、Senior User 和 Developer 建起来、评起来、管起来；
- 两者共享 Ontology、Data Hub、Model Hub、Connector、Tools 和治理规范；
- 通过 Skill-based JEV Harness 过渡，再演进到 ISS Skill-based Model。


### 4.1 ITEMGPT Runtime：给最终业务用户

#### 目标用户

- Citizen Business User；
- CEC / eSVC 等一线人员；
- 仓库和现场业务人员；
- 需要使用而不是开发 AI 的人员。

#### 核心体验

用户不需要理解 Prompt、MCP 或复杂模型，只需要表达业务目标：

- “帮我生成一个 WMS 异常处理表单”；
- “帮我查这个 BO 的原因和预计完成时间”；
- “把这段 CEC 记录整理成 SOP 草稿”；
- “请按当前库存和订单优先级给出料件替换建议”。

#### Standardization

ITEMGPT Runtime 不应鼓励无限制的个人定制，而要通过：

- 标准模板；
- 标准字段；
- 标准 Action；
- 标准业务术语；
- 标准权限；
- 标准输出格式；
- 标准质量检查。

让 Citizen User 的创新能够进入可治理的组织流程。

#### Robotics / 无头化

运行时不仅是聊天入口，还可以把高频任务变成后台自动执行：

- 状态监控；
- 资料整理；
- 任务派发；
- 标准通知；
- 数据同步；
- 异常提醒。

#### Token Saving

- 简单分类和路由由小模型完成；
- 稳定流程使用规则和模板；
- 只有复杂判断才调用大模型；
- 领域知识通过 Ontology 和压缩上下文加载；
- 重复任务使用缓存和可复用 Agent。

---

### 4.2 Agent Factory：给专业共建者和治理者

#### 目标用户

- DT：业务数字化、流程和数据负责人；
- FDE：负责现场交付和领域知识落地；
- Senior User：具备业务判断能力和场景经验的高级用户；
- Developer：负责工具、连接器、部署和工程实现。

#### 核心能力

- 从场景描述生成 Agent 草案；
- 将多个子 Agent 组合为 Group Agent；
- 接入 Ontology、Data、Model、Skill、MCP 和 Tools；
- 配置权限、上下文和 Action；
- 在沙盒环境测试；
- 进行标准化 Qualification；
- 管理版本和发布；
- 记录内部调用、Token、错误和人工介入；
- 评估准确率、响应时间、成本和业务收益。

#### Qualification 的建议维度

一个 Agent 不应因为“能跑起来”就直接发布，至少应通过：

- 业务场景覆盖测试；
- 关键规则测试；
- 异常和数据缺失测试；
- 权限和安全测试；
- Action 风险测试；
- 响应时间测试；
- 成本 / Token 测试；
- 人工接管测试；
- 版本和日志完整性测试。

---

---

## 5. Ontology Studio：从知识挖掘开始的第一环

### 本节大纲

Ontology Studio 是整个闭环的第一环：它把事实、事理和行动组织成统一业务语义，使 Data、Model、Agent、Dynamic Form 和 Action 不再依赖个人 Prompt 或孤立经验。


### 5.1 为什么是第一环

如果没有 Ontology：

- Data Hub 只是数据连接；
- Model Hub 只是模型集合；
- Agent 只能依赖 Prompt 理解业务；
- Dynamic Form 只能生成页面，无法理解业务含义；
- Action 可能缺乏规则和边界。

Ontology Studio 的作用是把业务知识、数据和行动组织成统一的业务语义。

### 5.2 共建工作方式

建议采用五类角色共同参与：

- **业务 Owner**：说明目标、流程、例外和价值指标；
- **DT / Senior User**：梳理数据、流程和系统关系；
- **FDE**：补充真实现场知识和服务规则；
- **Item**：负责方法、工具、Agent 化和产品化；
- **IT / Security**：确认系统、权限和生产要求。

### 5.3 以 BO 为例的 Ontology 共建步骤

1. 描述 BO 的业务目标和客户承诺；
2. 列出订单、料件、库存、维修、物流、客户和服务对象；
3. 定义对象关系和状态变化；
4. 梳理优先级、替换、库存和运输规则；
5. 定义哪些动作可以自动执行；
6. 定义哪些动作必须人工确认；
7. 接入 UKM、订单、库存、物流和维修数据；
8. 在沙盒中用真实但脱敏的数据测试；
9. 将 Agent 使用中的错误和缺失反馈给 Ontology Owner；
10. 经过版本管理后发布到正式运行环境。

---

---

## 6. 合作计划：从知识挖掘走向联合产品

### 本节大纲

六个合作问题在这里收敛：

- 哪些已有 Agent、Model、Skill、Connector 和数据能力可以直接复用？
- 哪些能力适合标准接口接入，哪些需要进入 Accelerator 的统一治理与服务化环境？
- 第一阶段是否采用 Skill-based JEV Harness？
- 目标状态是否演进为 ISS Skill-based Model？
- ISS-LRM、通用 LLM、预测模型、优化模型与小模型如何路由和计费？
- 哪些业务场景真正体现“减少低水平重复”和“触发高水平创新”？

随后通过七个阶段把这些问题转成联合交付：知识挖掘、能力基座准备、Agent 共建、Training、优化深耕、产品沉淀、外部推广。


### 6.1 与 ISS AI Accelerator 的能力对齐（放在合作计划中讨论）

在 COO AI 团队 Hollis 提出的 Accelerator 理论框架下，ISS AI Accelerator 应被定位为 Item 业务应用之下的企业级赋能与治理底座。双方不应被表述为两个竞争平台，而应明确协作边界：Item 面向业务场景、用户体验、Agent 编排、动态表单和产品化；Accelerator 面向可复用能力、企业数据、异构算力、模型服务、部署认证和运行治理。

| Accelerator 能力域 | 对 Item × ISS Biz Team AI 合作的支撑 | 会议中应如何表达 |
|---|---|---|
| 数据分级互联 | LUDP、数仓、数据湖、DaaS、数据血缘、业务语义和知识接入 | 为 Data Hub 提供可信、可治理、可追溯的数据上下文 |
| 算力共享 | GPU as a Service、配额队列、MIG / 分时混部、资源利用率优化 | 为模型、Agent 和批量任务提供可控的算力服务 |
| 模型复用 | MaaS 模型目录、统一模型网关、LoRA、ISS 专域 LRM | Model Hub 不重复造模型，根据任务选择小模型、LRM、LLM、预测和优化模型 |
| 部署与认证 | K8S、多租户隔离、统一登录、EA / BIA 认证、共享环境 | 让 Demo 能够从沙盒走向可认证、可运行的企业环境 |
| 智能体服务化 | 沙箱、Runtime 托管、Agent Marketplace、编排、A2A 互通 | 让 Skill 和 Agent 可登记、发现、复用、观测和治理 |

Marketplace 在本架构中属于技术能力层，负责 Agent、Skill、Model、Tool、Connector 和 Ontology 能力的登记、发现、复用、评估与治理；Dashboard 则属于业务交互层，面向管理者和业务人员呈现采用率、收益和运行状态。

Accelerator 的五横两纵架构可简化为：基础设施与模型服务、数据与知识、模型能力、智能体服务、业务交互生态五个横向能力层，加上运营治理和运行观测两类纵向能力。


### 6.2 阶段一：知识挖掘

目标是先理解业务，而不是马上开发 Agent。

工作内容：

- 访谈 CEC、eSVC、UKM、SSC/GPO、Global Logistics、Field Service 等团队；
- 识别现有 Agent、SOP、知识库和流程断点；
- 梳理 BO、CEC SOP、Genesys、WMS、BNP、PEI 等场景；
- 建立场景价值、复杂度、数据可得性和复用潜力评分。

产出：

- Business Knowledge Map；
- Process Breakpoint Map；
- Hero Cases 优先级；
- 初版 Ontology 范围。

### 6.3 阶段二：能力基座准备

工作内容：

- 数据源和系统接口；
- UKM / EKP / EKF 知识接入；
- Data Hub 与数据治理；
- 共享算力和 GPU 配额；
- Model Hub、ISS-LRM、通用 LLM、小模型、预测与优化模型；
- Connector、Tools、Skill 和 Action；
- 部署、认证、权限、日志、审计和安全边界。

产出：

- Capability Inventory；
- Data / Model / Connector / Tool Catalog；
- 安全和上线要求；
- POC 环境。

### 6.4 阶段三：典型 Agent 共建

建议优先级：

1. BO / Customer Promise Agent；
2. CEC Record & Reply / SOP Agent；
3. Genesys CEC Agent；
4. WMS Dynamic Form Agent；
5. 港口拖柜 Headless Agent；
6. BNP / PEI 业务建模和动态表单 Agent。

先做少量高价值场景，避免一开始扩展到 20–30 个 POC 而没有统一方法。

### 6.5 阶段四：Training 和普及

#### 业务用户训练

- 如何使用 ITEMGPT Runtime；
- 如何表达业务需求；
- 如何使用标准 Agent 和动态表单；
- 如何反馈错误和改进建议；
- 哪些 Action 需要人工确认。

#### DT / FDE / Senior User 训练

- 如何使用 Ontology Studio；
- 如何构建和配置 Agent Factory；
- 如何连接 Data、Model、Skill、MCP 和 Tools；
- 如何进行 Qualification、沙盒测试和发布；
- 如何维护业务知识和版本。

### 6.6 阶段五：优化与垂直深耕

重点方向：

- 上下文压缩；
- Ontology 完善；
- 领域小模型；
- Hybrid AI；
- 预测与优化模型；
- 多 Agent 协作；
- 动态沙盒和规模化部署；
- Token 和调用成本；
- 准确性、响应时间和人工介入率。

垂直深耕优先考虑：

- 服务供应链；
- 售后诊断；
- BO 与 Customer Promise；
- 库存和料件替换；
- 物流 ETA；
- Supply / Demand Planning；
- Dynamic Sourcing 与 Tariff。

### 6.7 阶段六：沉淀产品

把成功案例从项目形态转成产品形态：

- 标准 Ontology；
- 标准数据模型；
- 标准 Agent；
- 标准动态表单；
- 标准 Connectors 和 Tools；
- 标准治理、测试和部署流程；
- 标准 Dashboard 指标。

建议形成以下产品包：

1. **ISS Service Intelligence Solution**；
2. **Back Order / Customer Promise Solution**；
3. **CEC / Genesys AI Solution**；
4. **Service Supply Chain Decision Solution**；
5. **WMS / Warehouse Business Tooling Solution**。

### 6.8 阶段七：外部推广

在内部验证后，探索：

- Genesys Marketplace；
- 联想服务业务和其他区域；
- 外部供应链和物流客户；
- Item SaaS 产品化；
- 联想品牌、场景与 Item 应用能力联合推广。

外部推广前需要先明确：

- 产品和 IP 归属；
- 数据和模型使用边界；
- 联合销售和交付方式；
- 商业收益分配；
- 版本、售后和运营责任。

---

### 6.9 Item 自有业务价值案例

为了让合作叙事同时具备“联想/ISS Biz Team 业务价值”和“Item 产品价值”两条证据链，建议补充一个 Item 已经验证过的效率或人力价值案例。该案例不应简单表达为“减员”，而应展示：

- 重复性后台工作被自动化；
- 人工处理量、人工介入时间或单位案件成本下降；
- 同等团队规模可以支持更多业务量；
- 人员从事务性操作转向异常处理和高价值决策；
- 通过标准 Skill、Agent、Connector 和治理机制，将一次性项目能力沉淀为可复制产品。

如果使用历史案例中的人员数量变化或效率数据，正式 Demo 中必须注明数据的业务背景、时间范围和口径，不应直接将历史结果承诺为 ISS Biz Team 项目结果。

### 6.10 “编辑部”事项

会议笔记中出现“编辑部”字样，但目前尚无法判断其具体团队、项目或业务含义。确认全称、业务场景和是否进入 Demo 前，不纳入正式议程。

---

### 6.11 模型路由、成本治理与内部结算议题

Accelerator 材料中出现 ISS 专域 LRM、统一模型网关和模型复用能力。Demo 中不需要立即给出完整技术定价方案，但应把以下问题列为合作设计议题：

- 哪些任务使用通用 LLM，哪些任务使用 ISS-LRM、领域小模型、预测模型或优化模型？
- ISS-LRM 的能力边界、部署位置、数据使用范围和质量指标是什么？
- Model Hub 以调用次数、Token、GPU 时间、模型服务实例还是业务能力包进行成本核算？
- ISS-LRM 与通用 LLM 的定价/内部结算如何设计，是否需要按业务线、区域、模型等级或 Skill 计费？
- Skill、Agent、Model 和算力的成本是否能够回流到 Dashboard，形成 Adoption、质量和单位业务价值指标？

建议在会议中先使用“模型路由与成本治理”表述，不在信息未确认前承诺具体价格。

---

## 7. 会议结束确认与下一步

### 7.1 推进方向

**From Hero Cases to Joint Product**

#### 短期、中期与长期

**短期：**

- 将 BO / Customer Promise 作为首批 Hero Cases 的优先候选，并同时确认其他案例的组合与顺序；
- 完成知识挖掘、数据与接口梳理；
- 共建 Ontology 和首批 Agent。

**中期：**

- 扩展到 CEC SOP、Genesys、WMS、物流和供应链决策；
- 建立 ITEMGPT Runtime 与 Agent Factory 的使用和治理体系；
- 形成 ISS Dashboard 与 Marketplace 的组织级入口。

**长期：**

- 沉淀服务供应链和供应链智能化产品；
- 在联想其他区域和业务线复制；
- 通过 Genesys Marketplace 等渠道探索外部推广。

#### 结束语

> 我们不是要做一个更大的通用 AI 平台，而是要把 ISS Biz Team 已经拥有的业务知识、COO AI 团队的供应链算法能力和 Item 的应用工程能力，结合成一套真正能解决业务问题、能够持续治理、可以被复制和商业化的垂直智能解决方案。

---

---

### 7.2 正式会议前准备项

以下事项建议在正式 ISS Biz Team Demo 前确认，避免在会议中出现名称或状态不一致：

1. BNP 的准确业务全称和 PEI 的具体范围；
2. eSVC small model 的准确目标，是情绪、意图、路由还是其他能力；
3. CSAS Genesys AI App 的当前成熟度和可演示范围；
4. BO POC 当前已有结果、问题和可公开指标；
5. UKM / EKP / EKF 当前可提供的接口和知识范围；
6. 哪些 Action 可以在 Demo 中真实执行，哪些只能模拟；
7. 港口拖柜和 WMS 案例的数据是否需要脱敏或改用演示数据；
8. COO AI 团队供应链 AI 技术材料中模型名称和算法名称的最终英文写法；
9. ISS Biz Team 业务价值工作坊预计时长以及技术人员和业务领导的比例；
10. 首批 Hero Cases 的业务 Owner、技术 Owner 和后续 POC 决策人。

---

---

### 7.3 会议后共同确认的决策项

以下事项是本次 Accelerator 讨论后需要补齐的决策，不建议在尚未确认前写成对外承诺：

1. “Skill-based JEV Harness” 的正式名称、JEV 含义和第一阶段交付边界；
2. “ISS Skill-based Model” 的目标架构、Skill Owner、目录和治理规则；
3. ISS-LRM 的正式名称、能力范围、部署方式以及与通用 LLM 的路由关系；
4. ISS-LRM、LLM、GPU、Agent 和 Skill 的定价或内部成本分摊方式；
5. Data Hub、Connector、Tools 中由 DT、COO、ISS Biz Team AI 和 Item 分别负责的具体内容；
6. Record & Reply 的“不存视频”要求和 Edge server 的部署、绑定、数据留存边界；
7. Hollis Phase I & II 的阶段目标、时间范围、交付物和决策门；
8. “编辑部”具体指哪个团队或场景，是否进入 Demo；
9. Item 自有“业务价值/人力效率”案例的可公开数据、口径和历史背景。

---

---

# 结论

这版 Demo 的结构与演示顺序保持一致：先由 Steven 建立合作目标和四个会议确认，再用总体架构解释为什么能做；用案例证明能力覆盖，以 BO / Customer Promise 作为业务价值高潮；随后解释能力底座、差异化、两套 Business Oriented Tools 和 Ontology Studio；最后把 Accelerator 对齐、模型路由、成本治理和七阶段合作计划收敛为联合产品路线。

其中最重要的主线是：

**业务价值与知识挖掘 → Open 探索 → Transform 场景化 → Engineer 工程化 → Skill-based JEV Harness → ISS Skill-based Model → Data / Compute / Model / Agent / Skill 复用 → Agent Factory / ITEMGPT Runtime → ISS Dashboard / Marketplace → 反馈优化 → 标准产品与推广**


---

---

# 附录 A：会前、会上、会后的阅读关系
三份材料使用相同的 MD0–MD7 章节号。会前简版用于快速了解业务主线；会上详版用于观看案例、讨论边界与收敛决定；会后本文保留完整论证与待确认事项。HTML 顶部可切换版本，左侧“查看同章详版 / 返回同章简版”保持所选章节。

## 十页会前简版与四十页详版映射
- 简版第01页｜MD §0.1–0.2｜业务价值实现探讨：会前阅读总览｜对应详版第1页。
- 简版第02页｜MD §0.1–0.5｜合作不是一次产品交付｜对应详版第3–6页。
- 简版第03页｜MD §1.1–1.2｜从业务知识到可执行行动｜对应详版第7–10页。
- 简版第04页｜MD §2.1–2.7｜七个案例与 Hero Cases 组合｜对应详版第11–21页。
- 简版第05页｜MD §3.1–3.4｜统一上下文与能力复用｜对应详版第22–25页。
- 简版第06页｜MD §4.1–4.2｜两套业务工具与角色分工｜对应详版第26–29页。
- 简版第07页｜MD §5.1–5.3｜Ontology Studio 与知识共建｜对应详版第30–32页。
- 简版第08页｜MD §6.1–6.11｜从能力共建走向联合产品｜对应详版第33–37页。
- 简版第09页｜MD §7.1–7.3｜从 Hero Cases 到联合产品｜对应详版第38–40页。
- 简版第10页｜MD §0–7 / 结论｜会前、会上、会后三份材料联动｜对应详版第1–40页。

## 四十页详版内容索引
- 详版第01页｜MD §0.1–0.2｜AI Accelerator 的业务价值实现探讨。
- 详版第02页｜MD §0.3–0.4｜从部门业务场景走向可复用的业务能力。
- 详版第03页｜MD §0.1–0.5｜0. 合作不是一次产品交付。
- 详版第04页｜MD §0.1–0.2｜0.1–0.2 三方如何共同承担结果。
- 详版第05页｜MD §0.2 / 0.5｜0.2 / 0.5 为什么现在需要合作。
- 详版第06页｜MD §0.4｜0.4 今天必须获得的四类确认。
- 详版第07页｜MD §1.1–1.2｜1. 让业务、知识、模型和行动连成一条链。
- 详版第08页｜MD §1.2 第二–三层｜1.2 从系统字段到统一业务上下文。
- 详版第09页｜MD §1.2 第四层｜1.2 判断能力必须分工。
- 详版第10页｜MD §1.2 第五–六层｜1.2 从能理解到能执行、可审计。
- 详版第11页｜MD §2.1–2.7｜2. 七个案例，各证明一件事。
- 详版第12页｜MD §2.1｜2.1 港口拖柜：无头 Agent 跑完整流程。
- 详版第13页｜MD §2.2｜2.2 WMS Dynamic Form：业务人员快速做应用。
- 详版第14页｜MD §2.3｜2.3 BO / Customer Promise：重点 Hero Cases 之一。
- 详版第15页｜MD §2.3 推荐 Demo 场景｜2.3 把 BO 的八步闭环逐步走通。
- 详版第16页｜MD §2.3 指标与风险｜2.3 指标不是承诺；治理不是把模型锁死。
- 详版第17页｜MD §2.4｜2.4 BNP → Dynamic Form → PEI。
- 详版第18页｜MD §2.5｜2.5 Record & Reply → CEC SOP。
- 详版第19页｜MD §2.6｜2.6 eSVC Small Model：高频判断与成本分层。
- 详版第20页｜MD §2.7｜2.7 CEC + Genesys AI App：内部能力走向产品。
- 详版第21页｜MD §2 / 6.4｜2. 为首批 Hero Cases 做组合选择。
- 详版第22页｜MD §3.1–3.4｜3. 能力底座：不堆数据，不堆模型。
- 详版第23页｜MD §3.1–3.3｜3.1–3.3 COO AI × Item × ISS Biz Team 的协同。
- 详版第24页｜MD §3.4｜3.4 面向人的 Dashboard；面向 Agent 的 Marketplace。
- 详版第25页｜MD §3 本节大纲 / 6.1 / 7.3｜3. 从 Open 到 Transform，再到 Engineer。
- 详版第26页｜MD §4.1–4.2｜4. 两套 Business Oriented Tools，共用同一底座。
- 详版第27页｜MD §4.1｜4.1 ITEMGPT Runtime：目标表达、标准化、后台执行。
- 详版第28页｜MD §4.2｜4.2 Agent Factory：草案到可治理发布。
- 详版第29页｜MD §4.2 Qualification｜4.2 能跑起来，不等于可以上线。
- 详版第30页｜MD §5.1–5.3｜5. Ontology Studio：知识挖掘的第一环。
- 详版第31页｜MD §5.3｜5.3 用 BO 的对象、关系、规则和 Action 建模。
- 详版第32页｜MD §5.2–5.3｜5.2–5.3 现场共建一张可执行业务模型。
- 详版第33页｜MD §6.1–6.11｜6. 合作计划：复用底座，形成联合产品。
- 详版第34页｜MD §6.1｜6.1 Accelerator 提供什么，Item 不重复建设什么。
- 详版第35页｜MD §6.2–6.5｜6.2–6.5 先理解业务，再共建、训练。
- 详版第36页｜MD §6.6–6.8 / 6.9｜6.6–6.8 深耕、沉淀产品，再探索外部推广。
- 详版第37页｜MD §6.9–6.11 / 7.3｜6.11 模型路由与成本治理，先列决策再谈价格。
- 详版第38页｜MD §7.1｜7. From Hero Cases to Joint Product。
- 详版第39页｜MD §7.2–7.3｜7.2–7.3 准备项与待决策项不能混为承诺。
- 详版第40页｜MD §7.1 / 结论｜合作不是一次产品交付；让业务能力持续演进。

# 附录 B：会议决定的补录原则
待会议结束后，按实际共同确认的内容记录首批 Hero Cases 范围、业务 Owner、技术 Owner、能力准备清单、责任、输入、产出、时间边界及下一决策门。当前文件未替参会者填写未知结论；未确认事项继续保留“待确认”。

# 附录 C：Demo 视频资料
七个案例分别在详版第12、13、14、17、18、19、20页预留视频。当前视频未提供；不把待接入素材、模拟Action或历史案例包装为已完成验证的结果。
