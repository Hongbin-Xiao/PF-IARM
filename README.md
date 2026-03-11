# PF-IARM:Intelligent Agent Requirements Modeling Based on Problem Frames

[![License](https://img.shields.io/badge/license-Academic-blue.svg)]()
[![Paper](https://img.shields.io/badge/paper-Published-green.svg)]()
[![Framework](https://img.shields.io/badge/framework-PF--AIRM-orange.svg)]()

## 📋 Overview

**PF-IARM** (Problem Frames based Agent Intelligent Requirements Modeling) is a systematic requirements engineering methodology specifically designed for intelligent agent systems in industrial applications. This method innovatively integrates Jackson's Problem Frames theory with the intelligent agent paradigm to address the limitations of traditional requirements engineering approaches in capturing agent characteristics such as autonomy, adaptability, and uncertainty.


**Problem Framews Meta Model**
<img width="10498" height="4750" alt="problemframes" src="https://github.com/user-attachments/assets/6467145e-6408-44eb-8ed7-975b6ff1f783" />




**PF-IARM Meta Model**

<img width="9956" height="5017" alt="pF4Agent" src="https://github.com/user-attachments/assets/ab2b4c35-7a18-48bc-a42a-f9bb8d96b75a" />


## 🎯 Key Features

- **Extended Meta-Model**: Incorporates intelligent agent domain, environment domain, knowledge domain, and goal domain
- **Four Core Problem Patterns**:
  - Perception-Decision-Execution (PDE) Pattern
 ![四种模式_01](https://github.com/user-attachments/assets/0be80675-f831-467a-babd-f0fbe15440d2)


  - Knowledge Acquisition and Learning Pattern
    ![四种模式_01(1)](https://github.com/user-attachments/assets/651aa824-caf5-47c5-94eb-5806a4a148e2)

  - Goal-Oriented Behavior Pattern
 
    ![四种模式_01(2)](https://github.com/user-attachments/assets/ec7e5fe3-7ac8-4541-84ad-9cea515185b3)

  - Multi-Agent Collaboration Pattern
 
  ![四种模式_01(3)](https://github.com/user-attachments/assets/2339303d-213e-4a11-809b-1a00b68cf9e9)


- **Graphical Modeling Platform**: Visual requirements modeling tool with standardized notation system
- **Industrial Pattern Library**: Reusable problem patterns for common industrial scenarios

## 🏗️ Architecture
![面向问题的智能Agent需求建模方法-图(1)_01(1)](https://github.com/user-attachments/assets/d6c6fdfc-9f15-41b7-80d8-96fba1677bd1)


## 🔬 Methodology

### 1. Requirements Elicitation and Analysis
- Stakeholder interviews
- Scenario analysis
- Goal decomposition
- Constraint identification

### 2. Problem Decomposition and Framework Selection
- Functional/goal-based decomposition
- Pattern matching from library
- Framework composition strategy

### 3. Problem Context Modeling
- Domain identification and description
- Phenomenon and interface definition
- Requirements specification

### 4. Requirements Specification Generation
- Formal specification extraction
- Completeness and consistency validation
- Stakeholder confirmation
- Iterative refinement

## 📊 Formal Definitions

### Intelligent Agent Domain
\[A = (C, K, G, L, F)\]
- \(C\): Capability set
- \(K\): Knowledge base
- \(G\): Goal set
- \(L\): Learning mechanism
- \(F\): Function set

### Environment Domain
\[E = (S, O, D)\]
- \(S\): State space
- \(O: S \rightarrow P\): Observability function
- \(D: S \times A \rightarrow S\): Dynamics function

### Knowledge Domain
\[K = (T, R, U, V)\]
- \(T\): Knowledge type
- \(R\): Relations
- \(U: K \rightarrow [0,1]\): Uncertainty measure
- \(V: K \rightarrow \{true, false, unknown\}\): Verification mechanism

### Goal Domain
\[G = (P, C, E)\]
- \(P: G \rightarrow \mathbb{R}\): Priority function
- \(C\): Constraint set
- \(E: S \rightarrow [0,1]\): Evaluation function

## 🎨 Graphical Notation

| Element | Type | Representation |
|---------|------|----------------|
| Intelligent Agent | Domain T3 | Orange rectangle with agent icon |
| Environment | Domain T3 | Blue rectangle |
| Knowledge | Domain T3 | Green rectangle |
| Goal | Domain T3 | Purple rectangle |
| Machine | Domain T1 | White rectangle |
| Interface | Relationship | Solid line connection |
| Phenomenon | Relationship | Labeled connection (Domain!{Phenomenon}) |

## 💡 Case Study: Intelligent Customer Service Agent

The methodology was validated through a comprehensive case study of an e-commerce intelligent customer service system, demonstrating:

- **Query Understanding & Response**: PDE pattern for natural language processing
- **Knowledge Learning & Update**: Dynamic knowledge base management
- **Transaction Processing**: Goal-oriented automated operations
- **Human Handoff Decision**: Multi-agent collaboration for complex queries
- **Service Quality Optimization**: Continuous improvement through feedback

## 📈 Evaluation Results

### Comparison with Existing Methods

| Method | Agent Domain | Environment | Knowledge | Goal | Uncertainty | Temporal |
|--------|--------------|-------------|-----------|------|-------------|----------|
| PF-CPS | ❌ | ✅ | ❌ | ❌ | ❌ | ❌ |
| PF-HCPS | ❌ | ✅ | ❌ | ❌ | ❌ | ❌ |
| PF-STPA | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |
| **PF-IARM** | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |

### Key Improvements
- ✅ Enhanced expressiveness for agent characteristics
- ✅ Systematic requirements analysis process
- ✅ Reduced transformation cycle from requirements to design
- ✅ Improved requirement completeness and accuracy

![00e98020cf3ddfd1e4dca83be3f218cc](https://github.com/user-attachments/assets/6eb7b3a8-c3dd-4c1f-95e3-3f4e68badcad)




## Complete case study
**Step1需求获取与初步分析：**智能客服Agent是电子商务平台的自动化客户服务系统，承担自动化客户服务的任务。系统需实现对客户关于产品信息、订单状态及售后服务等多类查询的理解与响应，支持基于自然语言的交互。系统应具备对常见问题模式的识别和学习能力，以提高回答的准确性和覆盖范围。针对简单交易操作，如订单查询、退换货申请等，系统需实现自动化处理，减少人工介入。在复杂问题场景下，系统能够准确识别无法自动处理的请求，并实现向人工客服的无缝转接，确保服务的连续性和问题的有效解决。系统同时需要收集客户反馈信息，结合交互数据进行分析，支持服务质量的持续改进。该系统涉及多层次的物理与信息环境，包括用户交互终端、后台服务系统、数据库及人工客服接口。系统设计需要明确各环境之间的边界与交互关系，构建完整的问题模型，确保需求的准确表达。

**Step2问题分解与框架选择：**智能客服Agent系统作为面向电子商务平台的自动客户服务系统，功能复杂且涉及多维度业务场景。为确保需求建模的针对性和可操作性，首先对整体问题进行分解，明确系统所需解决的核心子问题。结合系统实际业务需求及用户交互特点，将整体问题划分为以下五个子问题：
客户查询理解与响应。该子问题聚焦于系统如何准确理解用户的自然语言输入，包括产品信息、订单状态及售后服务等查询，并基于知识库和规则给出合理响应。
知识学习与更新。针对智能客服系统的持续优化需求，设计知识库的动态更新机制及模型版本管理策略，以支持系统对新问题的学习和回答质量的提升。
交易操作处理。涉及订单查询、退换货申请等简单交易操作的自动化处理，确保系统能安全、高效地执行相关业务流程。
人工转接决策。针对复杂或异常问题，系统需判断是否转接人工客服，并实现转接的上下文传递及权限审计，保障服务的连续性与合规性。
服务质量优化。通过设定KPI指标、监控服务表现及客户反馈，持续优化系统性能与用户体验。

**Step3问题上下文建模：**针对Step2中的五个子问题，依据PF-IARM方法选择适配的典型问题框架进行建模，明确各子问题的核心要素、输入输出及环境约束，具体如下：

子问题1：客户查询理解与响应如图5所示。采用感知-决策-执行(PDE)模式进行建模。
自主性体现：IntelligentAgent域通过自主决策机制，无需人工干预即可理解用户意图并生成响应。Agent根据感知到的用户消息和上下文，自主查询知识库并决策回复策略，体现了Agent的自主性。
学习能力体现：通过Knowledge域与IntelligentAgent域之间的“查询”和“更新”现象，Agent能够从交互日志中学习新的FAQ模式，动态更新知识库。当遇到未知问题时，系统记录问题并触发知识更新流程，体现了学习能力。
不确定性处理：用户消息现象标注了ProbabilityDistribution属性，表示意图识别的置信度。当置信度低于设定阈值(如0.7)时，Agent会触发澄清对话或转接人工客服，确保服务质量。
系统通过感知用户输入的消息及上下文信息，结合FAQ、商品信息及政策规则进行检索与匹配，决策相应的回复内容，并通过渠道接口返回给用户。该框架明确了输入(用户消息、上下文)、处理逻辑(理解与匹配)、输出(响应消息)及合规约束(隐私与合规限制)。

<img width="1890" height="755" alt="图5客户查询理解与响应" src="https://github.com/user-attachments/assets/73c38d3d-9a4d-4c8e-add2-9d234ba8d799" />
图5 客户查询理解与响应问题框架实例图

子问题2：知识学习与更新如图6所示。应用知识获取与学习模式，侧重知识库、模型仓库及版本管理的设计。
学习能力体现：Knowledge域通过数据治理和版本策略实现知识的持续演化。Agent从交互数据、外部知识源中提取新知识，经过验证后写入知识库，并通过版本管理支持知识回滚，体现了系统的学习和自适应能力。
知识不确定性管理：Knowledge域的不确定性度量U:K→[0,1]为每条知识标注可信度，验证机制V:K→{true, false, unknown}支持知识的真值判断，确保知识质量。
系统通过数据治理、版本策略及外部数据补充，实现知识的持续写入、模型的迭代更新和版本回滚，保证知识与模型的时效性和准确性。日志与监控系统提供反馈支持，促进知识质量提升。

<img width="1844" height="684" alt="图6知识学习与更新" src="https://github.com/user-attachments/assets/00451552-c06b-4900-a207-1cba428f3502" />
图6 知识学习与更新问题框架实例图




子问题3：交易操作处理如图7所示，采用目标导向行为模式，聚焦动作序列设计与异常处理。
目标驱动特性：Goal域定义了交易操作的目标(如“成功完成退货申请”)及其约束条件。Agent根据目标优先级和当前环境状态，动态规划动作序列，体现了目标导向行为。
自主决策与异常处理：IntelligentAgent域包含权限校验、异常判别和替代方案选择的决策逻辑。当遇到异常情况(如库存不足)时，Agent自主选择替代方案(如推荐类似商品)，无需人工介入。
系统根据用户身份、订单信息及授权状态，调用订单、物流、支付等后端系统API，执行交易操作。设计包含权限校验，确保交易安全与流程合规，同时关注处理效率与用户等待体验。

<img width="1865" height="601" alt="图7交易操作处理" src="https://github.com/user-attachments/assets/f9cd3f17-578b-4ed2-bd44-5d91e3a795f5" />
图7 交易操作处理问题框架实例图





子问题4：人工转接决策如图8所示，采用多Agent协作模式。
多Agent协作特性：该框架涉及智能客服Agent与人工客服Agent的协作。通过定义转接协议、上下文传递规范和权限审计机制，确保两个Agent之间的无缝协作。
动态决策机制：IntelligentAgent域根据问题复杂度、队列状态和客户满意度等多维度信息，动态决策是否转接人工。决策过程考虑了不确定性因素，如人工客服的可用性。
基于多Agent协作模式，系统需要判断是否将请求升级至人工客服。该框架涵盖转接时的上下文协议、客户满意度及升级成功率等指标，同时考虑隐私遮蔽和权限审计，保障转接过程的安全与合规。系统通过查询队列和坐席状态，实现转接受理和结果反馈。

<img width="1808" height="551" alt="图8人工转接决策" src="https://github.com/user-attachments/assets/60ad21c4-ccd0-4283-b01f-c0d6a48b774b" />
图8 人工转接决策问题框架实例图






子问题5：服务质量优化问题如图9所示，采用知识获取与学习模式进行建模，结合KPI目标与阈值设定，监控系统的响应准确率、一次解决率（FCR）及响应时延等关键指标。
持续优化能力：通过KPI目标域和度量体系，系统持续监控服务质量指标(如响应准确率、一次解决率)。当指标低于阈值时，触发策略库更新和流程优化，体现了系统的自我改进能力。
反馈驱动学习：客户反馈通过反馈表单收集，经过分析后驱动知识库和策略库的更新，形成“监控-反馈-优化”的闭环，体现了持续学习特性。
通过度量体系设计、报警规则及反馈表单，持续采集运营数据，驱动策略库和流程手册的动态更新，实现服务质量的闭环优化。

<img width="1640" height="551" alt="图9服务质量优化" src="https://github.com/user-attachments/assets/013471d5-6ec4-444f-893d-d2decf891c93" />
图9 服务质量优化问题框架实例图








**Step4需求规约生成与验证：**

功能需求规约详细描述了智能客服Agent系统应实现的核心业务功能及其行为逻辑。系统应支持多渠道的自然语言输入，具备精准的语义理解能力，能够结合FAQ、商品信息和政策规则，快速准确地响应用户查询。知识库的动态管理及模型版本控制机制是系统实现持续学习与优化的基础，确保知识体系的时效性和稳定性。交易操作处理方面，系统需自动执行订单查询、退换货申请等业务，具备完善的权限校验和异常处理机制，保障交易流程的安全与一致性。针对复杂问题，系统应智能判断并支持顺畅的人工客服转接，确保上下文信息完整传递，提升客户服务体验。同时，系统需持续采集运营数据，动态监控和优化服务质量，确保功能实现的有效性和用户满意度。


质量需求规约聚焦于系统的非功能性属性，明确了性能、可靠性、安全性和可维护性等方面的具体要求。系统必须保证高响应性能，达到预定的查询准确率和首次响应时间标准，确保用户交互的流畅性和效率。系统架构应具备高可用性和故障自动恢复能力，保障服务的连续性和数据完整性。在安全性方面，系统需严格遵循隐私保护法规，实施数据脱敏和访问权限审计，防范信息泄露和非法访问。可维护性方面，系统设计应模块化，支持知识库和模型的灵活更新，便于快速定位问题和迭代升级，从而保障系统长期稳定运行。


学习需求规约明确系统的智能化目标，强调知识获取、更新和优化机制。系统应整合多源知识数据，包括FAQ、用户交互日志及外部数据，构建全面且动态更新的知识库。通过基于反馈的在线学习机制，系统能够自动识别知识盲区，触发知识更新和模型训练，实现智能水平的持续提升。此外，系统应通过个性化交互引导和推荐，帮助用户快速获得所需信息和操作技能，提升用户满意度和使用效果，体现系统的教育和辅助功能。


接口需求规约详细规范了系统与外部组件及平台的交互方式，确保数据交换的兼容性和通信的安全性。系统接口需明确API调用方式、输入输出参数格式及调用频率限制，支持RESTful或RPC等主流通信协议。数据格式统一采用标准化的JSON或XML，保证跨平台的数据解析一致性。接口设计包含完善的异常捕获和错误反馈机制，定义明确的错误码和重试策略，以提升系统的健壮性和容错能力。同时，接口通信必须支持身份认证、权限控制和数据加密，防范非法访问和数据泄漏风险，保障系统间安全可靠地协同工作。
















