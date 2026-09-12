# Reason & Result — Postmortem / RCA 事故报告书面定制版
> 来源：Check Your English Vocabulary for IELTS（第98–99页）
> **定制场景**：Application Support — 事故报告书面写作（Postmortem / Root Cause Analysis）
> **配套版本**：口语/会议版见《Reason_Result_ApplicationSupport_定制版.md》
> **语体要求**：书面正式语体 —— 优先正式词（owing to / as a consequence / on the grounds that / ensued / subsequently / thereby）、适度被动语态（It was determined that...）、避免口语缩写（do not 而非 don't）

---

## 📌 核心词汇框架（15词全覆盖）

### 📐 词类分类

| 词类 | 词汇 | Postmortem 场景应用 |
|------|------|----------------|
| **原因类** | due to, owing to, on account of, the reason for, on the grounds that | 根因陈述、故障归因、决策依据说明 |
| **目的类** | in order to, so as not to, with the aim of | 纠正/预防措施的目的说明 |
| **结果类** | ensued, as a result, as a consequence, affect | Timeline、Impact Analysis 影响链描述 |
| **动机/后果类** | motive, effect, consequence | 决策动机分析、措施效果评估、后果定性 |

> 💡 **书面语提示**：Postmortem 文档中，原因类优先用 **owing to**（比 due to 更正式），结果类优先用 **as a consequence**（比 as a result 更正式），并搭配被动语态增强客观性。

---

## 🔄 书面 vs 口语 表达对照表（重点！）

写 Postmortem 时，把口语表达升级为书面正式表达：

| 口语表达 | 书面正式表达 | 例句 |
|----------|-------------|------|
| because of / due to | **owing to** | The outage was attributed **owing to**... → 正确用法：Service degraded **owing to** connection pool exhaustion. |
| so | **thereby** | The patch was applied, **thereby** restoring normal traffic flow. |
| we found out | **It was determined that... / Subsequent investigation revealed...** | **Subsequent investigation revealed** a memory leak in the payment module. |
| as a result | **as a consequence / consequently** | **As a consequence**, error rates climbed to 31%. |
| it happened because | **The reason for... was...** | **The reason for** the prolonged downtime was the absence of automated rollback triggers. |
| we chose X because | **X was adopted on the grounds that...** | The release was promoted **on the grounds that** all integration tests had passed. |
| it broke things | **X was affected / X ensued** | A cascading failure **ensued** when the connection pool was exhausted. |
| we did X to Y | **X was implemented in order to Y** | Canary deployment was adopted **in order to** limit the blast radius. |
| we wanted to avoid | **so as not to** | Deployments are frozen during peak hours **so as not to** disrupt revenue-critical flows. |
| our goal was | **with the aim of** | Pool-exhaustion alerts were configured **with the aim of** detecting leaks within five minutes. |
| why we did it | **The motive behind... was...** | **The motive behind** bypassing the staging soak test was schedule pressure. |
| it hit X users | **X users were affected** | Approximately 9,800 active customers **were affected**. |
| don't / can't / didn't | **do not / cannot / did not** | The tests **did not** cover the exception-handling path. |

> 💡 **被动语态三件套**（Postmortem 高频）：
> - **It was determined that**... （经确认……）
> - **The outage was attributed to**... （故障归因于……）
> - **Subsequent investigation revealed**... （后续调查发现……）

---

## 📝 核心词汇详解 + Postmortem 书面例句

### 🔵 原因类 — 根因陈述与归因

| 词汇 | 用法 | 正式度 |
|------|------|--------|
| **due to** | + 名词短语 | 中性，通用 |
| **owing to** | + 名词短语 | ★ 最正式，Postmortem 首选 |
| **on account of** | + 名词短语 | 正式，多用于补充说明 |
| **the reason for** | + 名词/动名词 | 用于显式回答"为什么" |
| **on the grounds that** | + 从句 | 用于书面陈述决策依据 |

**Postmortem 书面实例：**

> The initial latency spike was **due to** lock contention on the inventory table.
> （最初的延迟飙升是由于库存表上的锁竞争。）

> The outage was attributed **owing to** an unclosed database connection in the exception-handling path. → 注意：be attributed to 是固定搭配；owing to 用于主动归因句，如：
> Service degradation **owing to** connection pool exhaustion was first observed at 13:45 UTC.
> （UTC 时间 13:45 首次观察到因连接池耗尽导致的服务降级。）

> Two scheduled batch jobs were suspended **on account of** elevated error rates.
> （由于错误率升高，两个定时批处理任务被暂停。）

> **The reason for** the prolonged downtime was the absence of automated rollback triggers.
> （停机时间过长的原因在于缺少自动回滚触发机制。）

> The release was promoted to production **on the grounds that** all integration tests had passed.
> （该版本之所以被推进到生产环境，理由是所有集成测试均已通过。）

---

### 🟡 目的类 — 纠正与预防措施说明

| 词汇 | 用法 | 书面提示 |
|------|------|----------|
| **in order to** | + 动词原形 | Corrective Actions 首选，比 to 更正式 |
| **so as not to** | + 动词原形 | 书面否定目的；口语多说 so that we don't |
| **with the aim of** | + 动名词 | 用于说明长期预防目标（Preventive Actions） |

**Postmortem 书面实例：**

> A canary deployment strategy has been adopted **in order to** limit the blast radius of future releases.
> （已采用金丝雀发布策略，以限制未来发布的故障波及范围。）

> Deployments are now frozen during peak trading hours **so as not to** disrupt revenue-critical flows.
> （现在高峰交易时段冻结部署，以免干扰对营收至关重要的业务流。）

> Connection-pool utilization alerts were configured **with the aim of** detecting leaks within five minutes.
> （已配置连接池利用率告警，目的是在五分钟内检测到连接泄漏。）

---

### 🟢 结果类 — 时间线与影响描述

| 词汇 | 用法 | Postmortem 位置 |
|------|------|----------------|
| **ensued** | 不及物动词，随之发生 | Timeline 中描述连锁反应 |
| **as a result** | 连接短语 | 描述行动后的直接结果 |
| **as a consequence** | 连接短语（更正式） | Impact Analysis 中描述业务后果 |
| **affect** | 及物动词，影响 | Impact Analysis 中陈述影响范围 |

**Postmortem 书面实例：**

> A cascading failure **ensued** when the connection pool was exhausted.
> （连接池耗尽后，级联故障随之发生。）

> The rollback was executed at 14:32 UTC, and **as a result**, error rates returned to baseline within eight minutes.
> （回滚于 UTC 14:32 执行，结果错误率在八分钟内回到基线水平。）

> **As a consequence**, the payment gateway began rejecting new sessions.
> （因此，支付网关开始拒绝新建会话。）

> The outage **affected** approximately 9,800 active customers across all regions.
> （此次故障影响了所有区域约 9,800 名活跃客户。）

---

### 🔴 动机/后果类 — 决策分析与后果定性

| 词汇 | 含义 | Postmortem 位置 |
|------|------|----------------|
| **motive** | n. 动机 | Root Cause / Lessons Learned 中分析决策动机 |
| **effect** | n. 效果 | 评估纠正措施的效果 |
| **consequence** | n. 后果 | Impact Analysis 中定性最严重后果 |

**Postmortem 书面实例：**

> **The motive behind** bypassing the staging soak test was schedule pressure from the Q2 roadmap.
> （跳过预发环境浸泡测试的动机，是 Q2 路线图带来的排期压力。）

> The rollback had an **immediate positive effect** on error rates and checkout latency.
> （回滚对错误率和结账延迟产生了立竿见影的积极效果。）

> The most serious **consequence** of the incident was the SLA breach on the checkout endpoint.
> （此次事故最严重的后果是结账接口的 SLA 违约。）

---

## 🎯 Postmortem 文档六大章节：书面句式框架

### 1️⃣ Executive Summary（故障概述）

```
现象 + 影响 + 根因 + 解决，四句成段
```

| 要素 | 句式模板 |
|------|----------|
| 现象 | On [date], [service] experienced [symptom] owing to... |
| 影响 | Approximately [N] users were affected... |
| 根因 | The outage was attributed to... / It was determined that... |
| 解决 | Service was restored following [action] at [time]. |

> On 12 March 2026, the checkout service experienced a complete outage lasting 47 minutes. Approximately 9,800 customers **were affected**, and an estimated $18,000 in revenue was lost. **It was determined that** the outage was attributable to a memory leak introduced by release v2.14.0. Service was restored following an emergency rollback executed at 14:32 UTC.
> （2026年3月12日，结账服务经历了持续47分钟的完全停机。约9,800名客户受到影响，预计损失营收1.8万美元。经确认，故障归因于 v2.14.0 版本引入的内存泄漏。服务在 UTC 14:32 执行紧急回滚后恢复。）

### 2️⃣ Timeline（时间线，因果词串联）

| 时间点 | 书面句式 |
|--------|----------|
| 起因 | At [time], [trigger event] occurred **owing to**... |
| 连锁 | **Consequently**, [event B] **ensued**... |
| 扩大 | **As a consequence**, [impact] **affected**... |
| 止损 | [Action] was taken **in order to**... |
| 恢复 | **As a result**, [metric] returned to baseline. |

> - 13:38 UTC — Release v2.14.0 was promoted to production **on the grounds that** all integration tests had passed.（v2.14.0 版本因所有集成测试通过而被推进至生产环境。）
> - 13:45 UTC — Latency alarms fired; service degradation **owing to** rising heap usage was first observed.（延迟告警触发；首次观察到因堆内存上升导致的服务降级。）
> - 13:52 UTC — Connection pool exhaustion **ensued**, and a cascading failure spread to the order service.（连接池耗尽随之发生，级联故障蔓延至订单服务。）
> - 14:02 UTC — Two batch jobs were suspended **on account of** elevated error rates.（因错误率升高，两个批处理任务被暂停。）
> - 14:32 UTC — An emergency rollback was executed **in order to** restore service availability.（为恢复服务可用性，执行了紧急回滚。）
> - 14:40 UTC — **As a result**, error rates returned to baseline and the incident was closed.（结果错误率回到基线，事故关闭。）

### 3️⃣ Impact Analysis（影响分析）

| 维度 | 书面句式 |
|------|----------|
| 用户 | The outage affected [N] active users... |
| 收入 | An estimated [amount] in revenue was lost as a consequence of... |
| SLA | The incident resulted in an SLA breach of [duration]... |
| 关联服务 | Downstream services were affected on account of... |

> The outage **affected** approximately 9,800 active customers, of whom 12.4% experienced failed checkout attempts. **As a consequence**, an estimated $18,000 in revenue was lost. The incident **resulted in an SLA breach** of 47 minutes against the 99.95% availability target. Downstream reporting services **were affected on account of** suspended batch jobs.
> （此次故障影响了约9,800名活跃客户，其中12.4%结账失败。因此预计损失营收1.8万美元。事故导致结账接口违反99.95%可用性目标，SLA 违约47分钟。下游报表服务因批处理任务暂停而受影响。）

### 4️⃣ Root Cause Analysis（根因分析 — 5 Whys）

| 要素 | 书面句式 |
|------|----------|
| 现象确认 | It was determined that... |
| 深挖 | Subsequent investigation revealed... |
| 归因 | The root cause was determined to be..., owing to... |
| 决策动机 | The motive behind [decision] was... |

> **It was determined that** the immediate trigger was connection pool exhaustion. **Subsequent investigation revealed** that connections were never released in the exception-handling path **owing to** a missing `finally` block. **The root cause was determined to be** a code defect introduced in v2.14.0, compounded by insufficient test coverage **on the grounds that** the exception path had not been exercised. **The motive behind** deferring the additional test work was schedule pressure.
> （经确认，直接触发因素是连接池耗尽。后续调查发现，异常处理路径中因缺少 `finally` 块导致连接从未释放。根本原因确认为 v2.14.0 引入的代码缺陷，且由于异常路径未被测试覆盖，问题进一步放大。推迟补充测试工作的动机是排期压力。）

### 5️⃣ Corrective & Preventive Actions（纠正与预防措施）

| 类型 | 书面句式 |
|------|----------|
| 纠正（已完成） | [Action] was implemented **in order to**... |
| 预防（进行中） | [Action] is being rolled out **with the aim of**... |
| 流程约束 | [Rule] has been introduced **so as not to**... |

> - A canary deployment strategy has been adopted **in order to** limit the blast radius of future releases.（已采用金丝雀发布策略，以限制未来发布的故障波及范围。）
> - Connection-pool utilization alerts were configured **with the aim of** detecting leaks within five minutes.（已配置连接池利用率告警，目的是五分钟内发现连接泄漏。）
> - Deployments are frozen during peak trading hours **so as not to** disrupt revenue-critical flows.（高峰交易时段冻结部署，以免影响营收关键业务流。）
> - Exception-path unit tests are now mandatory **on the grounds that** untested error handling caused this incident.（异常路径单元测试现已成为强制要求，理由是未经测试的异常处理引发了本次事故。）

### 6️⃣ Lessons Learned（经验教训）

> **What went well:** The rollback procedure had an immediate positive **effect** on service health and was completed within eight minutes.
> （做得好的：回滚流程对服务健康产生了立竿见影的积极效果，八分钟内完成。）
>
> **What went wrong:** The most serious **consequence** was the SLA breach; the **reason for** the extended impact was the absence of automated rollback triggers.
> （做得不好的：最严重的后果是 SLA 违约；影响扩大的原因在于缺少自动回滚触发机制。）
>
> **Where we got lucky:** The incident occurred outside the APAC peak window, **so as not to**... → 正确书面表达：The timing limited the number of **affected** users; had it coincided with APAC peak hours, the impact would have been significantly greater.
> （时机上比较幸运：事故未与 APAC 高峰重叠，否则受影响用户将显著增加。）

---

## 📄 完整 Postmortem 短文示例（覆盖全部15个核心词）

**Incident Postmortem: Checkout Service Outage — 12 March 2026**

> On 12 March 2026, the checkout service experienced a complete outage lasting 47 minutes, during which approximately 9,800 active customers **(1) were affected**. Release v2.14.0 had been promoted to production **(2) on the grounds that** all integration tests had passed, although the exception-handling path **(3) was not** covered by the test suite. Forty minutes later, connection pool exhaustion **(4) ensued owing to** a memory leak caused by connections that were never released. **(5) As a consequence**, the payment gateway began rejecting new sessions, and a cascading failure spread to the order service. **(6) The reason for** the prolonged downtime was the absence of automated rollback triggers; two batch jobs were additionally suspended **(7) on account of** elevated error rates. An emergency rollback was executed at 14:32 UTC **(8) in order to** restore service availability, and it had an **(9) immediate positive effect** on error rates, which returned to baseline within eight minutes. **(10) As a result**, the incident was formally closed at 14:40 UTC. **(11) It was determined that** the root cause was a code defect introduced by v2.14.0, and subsequent investigation revealed that heap usage had been rising for days **(12) due to** the same leak. **(13) The motive behind** skipping the staging soak test was schedule pressure from the Q2 roadmap. The most serious **(14) consequence** of the incident was an SLA breach of 47 minutes. Going forward, canary deployments have been adopted **(15) with the aim of** limiting the blast radius, and deployments are frozen during peak hours **(15b) so as not to** disrupt revenue-critical flows.

**中文翻译：**

> 2026年3月12日，结账服务经历了持续47分钟的完全停机，期间约9,800名活跃客户受到影响。v2.14.0 版本之所以被推进到生产环境，理由是所有集成测试均已通过，尽管测试套件并未覆盖异常处理路径。四十分钟后，因从未释放的连接引发内存泄漏，连接池耗尽随之发生。因此，支付网关开始拒绝新建会话，级联故障蔓延至订单服务。停机时间过长的原因在于缺少自动回滚触发机制；此外，因错误率升高，两个批处理任务被暂停。为恢复服务可用性，UTC 14:32 执行了紧急回滚，回滚对错误率产生了立竿见影的积极效果，八分钟内即回到基线。结果，事故于 UTC 14:40 正式关闭。经确认，根本原因是 v2.14.0 引入的代码缺陷；后续调查还发现，数日以来堆内存一直因同一泄漏而持续上升。跳过预发环境浸泡测试的动机是 Q2 路线图带来的排期压力。此次事故最严重的后果是47分钟的 SLA 违约。今后已采用金丝雀发布以限制故障波及范围，并在高峰时段冻结部署以免干扰营收关键业务流。

> ✅ **15词核对清单**：were affected (1) / on the grounds that (2) / was not（书面缩写规避）(3) / ensued + owing to (4) / as a consequence (5) / the reason for (6) / on account of (7) / in order to (8) / effect (9) / as a result (10) / It was determined that（被动语态）(11) / due to (12) / motive (13) / consequence (14) / with the aim of + so as not to (15)

---

## 🔗 RCA 5 Whys 因果链示例

**问题：为什么结账服务在3月12日宕机47分钟？**

| 层级 | Why | 书面回答 |
|------|-----|----------|
| Why 1 | Why did the checkout service fail? | Service failed **owing to** connection pool exhaustion.（因连接池耗尽而失败。） |
| Why 2 | Why was the connection pool exhausted? | Connections were never released **due to** a memory leak in the exception path.（因异常路径内存泄漏，连接从未释放。） |
| Why 3 | Why were connections never released? | The code path lacked a `finally` block, **as a consequence of** which connections leaked on every timeout.（代码路径缺少 finally 块，因此每次超时都泄漏连接。） |
| Why 4 | Why was this not detected before release? | The exception path **was not** tested, **on the grounds that** it was considered low-priority coverage.（异常路径未被测试，理由是它被视为低优先级覆盖项。） |
| Why 5 | Why was it considered low-priority? | **The motive** was schedule pressure; **consequently**, test coverage for error handling **was deprioritized**.（动机是排期压力，因此异常处理测试被降级。） |

> **根因结论（书面）**：The root cause was determined to be a code defect compounded by process gaps. Corrective actions were therefore prioritized **with the aim of** addressing both the technical defect and the underlying decision-making culture.
> （根因确认为代码缺陷叠加流程缺口。因此纠正措施优先针对技术缺陷与底层决策文化两方面。）

---

## 📊 书面句式速查表（按 Postmortem 章节分组）

### Executive Summary 常用句式

| 想表达 | 书面表达 |
|--------|----------|
| 发生了什么 | On [date], [service] experienced [symptom]... |
| 归因 | The outage was attributed to... / It was determined that... |
| 影响人数 | Approximately [N] users were affected... |
| 已恢复 | Service was restored following [action] at [time]. |

### Timeline 常用句式

| 想表达 | 书面表达 |
|--------|----------|
| 由于（起因） | ...owing to... / ...due to... |
| 随之发生 | ...ensued... / Consequently, ... |
| 因此 | As a consequence, ... |
| 为了止损 | [Action] was taken in order to... |
| 恢复正常 | As a result, [metric] returned to baseline. |

### Impact Analysis 常用句式

| 想表达 | 书面表达 |
|--------|----------|
| 影响了 | ...affected [N] users / [N] users were affected |
| 收入损失 | An estimated [amount] was lost as a consequence of... |
| SLA 违约 | The incident resulted in an SLA breach of [duration] |
| 连带影响 | Downstream services were affected on account of... |

### Root Cause Analysis 常用句式

| 想表达 | 书面表达 |
|--------|----------|
| 经确认 | It was determined that... |
| 后续调查发现 | Subsequent investigation revealed... |
| 决策理由 | [Decision] was made on the grounds that... |
| 决策动机 | The motive behind [decision] was... |
| 原因是 | The reason for [outcome] was... |

### Corrective & Preventive Actions 常用句式

| 想表达 | 书面表达 |
|--------|----------|
| 为了（纠正） | ...was implemented in order to... |
| 目的是（预防） | ...with the aim of + 动名词 |
| 以免（约束） | ...so as not to + 动词原形 |
| 理由是 | ...on the grounds that + 从句 |

### Lessons Learned 常用句式

| 想表达 | 书面表达 |
|--------|----------|
| 效果好 | [Action] had a positive effect on... |
| 后果严重 | The most serious consequence was... |
| 应当避免 | [Practice] should be avoided so as not to [risk] |

---

## 🚀 实战练习（Postmortem 文本填空）

### 练习一：Executive Summary 挖空

填入适当词汇（owing to / were affected / It was determined that / attributed / as a consequence）：

> On 12 March, the checkout service experienced a 47-minute outage. Approximately 9,800 customers __________. The outage was __________ to a memory leak in the payment module. __________, the incident resulted in an estimated $18,000 revenue loss. __________ the root cause was a missing `finally` block, and the connection leak persisted __________ the lack of pool-utilization monitoring.

### 练习二：Timeline + Actions 挖空

填入适当词汇（ensued / in order to / on the grounds that / so as not to / as a result / with the aim of）：

> Release v2.14.0 was promoted to production __________ all integration tests had passed. Twenty minutes later, connection pool exhaustion __________, and a cascading failure spread to the order service. An emergency rollback was executed __________ restore availability. __________, error rates returned to baseline within eight minutes. Canary deployments have since been adopted __________ limiting the blast radius, and peak-hour deployment freezes were introduced __________ disrupt revenue-critical flows.

### 练习三：RCA + Lessons 挖空

填入适当词汇（the reason for / motive / consequence / on account of / affect / effect / subsequently）：

> __________ the extended downtime was the absence of automated rollback triggers. Two batch jobs were suspended __________ elevated error rates, which continued to __________ reporting services for two hours. The __________ behind skipping the soak test was schedule pressure. __________ investigation revealed the same defect existed in staging logs, but the alerts had been silenced. The most serious __________ was the SLA breach; fortunately, the rollback had an immediate positive __________ on service health.

**参考答案：**
- 练习一：were affected / attributed / As a consequence / It was determined that / owing to
- 练习二：on the grounds that / ensued / in order to / As a result / with the aim of / so as not to
- 练习三：The reason for / on account of / affect / motive / Subsequent / consequence / effect

---

## 💡 书面写作注意事项

| 原则 | 说明 | 示例 |
|------|------|------|
| **正式词优先** | owing to > due to；as a consequence > so | Service degraded **owing to** pool exhaustion. |
| **被动语态适度** | 客观归因用被动，主动补救用主动 | The outage **was attributed to**... / We executed the rollback... |
| **避免缩写** | do not / cannot / did not | The tests **did not** cover the exception path. |
| **thereby 连接结果** | 比口语 so 正式 | The patch was applied, **thereby** restoring traffic flow. |
| **量化一切** | 人数、时长、金额、百分比 | **affected** 9,800 users; **47-minute** outage; **$18,000** loss |

### 常见错误

| ❌ 避免 | ✅ 推荐 |
|--------|--------|
| The outage was attributed owing to a memory leak. | The outage was attributed **to** a memory leak.（be attributed to 固定搭配） |
| Owing to we lacked monitoring, ... | **Owing to** the lack of monitoring, ...（owing to + 名词短语） |
| We rolled back cause it broke things. | The release was rolled back **on the grounds that** it caused transaction failures. |
| As a result of the rollback, so errors dropped. | The rollback was executed, and **as a result**, error rates dropped. |

---

## 📚 相关词汇延伸（书面写作增强）

| 领域 | 相关词汇（本书其他章节） | Postmortem 应用 |
|------|------------------------|----------|
| **Changes** | deploy, roll back, roll out, migrate | Release v2.14.0 was rolled back at 14:32 UTC. |
| **Success & failure** | mitigate, resolve, restore, breach | SLA was breached for 47 minutes. |
| **Time** | subsequently, prior to, following | **Subsequent** investigation revealed... |
| **Objection & complaint** | acknowledge, justify, justify a decision | The decision was justified **on the grounds that**... |

---

## 🎯 场景索引

| 需求 | 查看章节 |
|------|----------|
| 15个核心词总览 | 核心词汇框架 |
| 口语→书面升级表达 | 书面 vs 口语 对照表 |
| Executive Summary 写法 | 六大章节 1️⃣ |
| Timeline 因果串联 | 六大章节 2️⃣ |
| Impact Analysis 量化 | 六大章节 3️⃣ |
| 5 Whys 因果链 | RCA 5 Whys 示例 |
| 完整范文（含翻译） | 完整 Postmortem 短文示例 |
| 分章节句式速查 | 书面句式速查表 |
| 填空自测 | 实战练习（附答案） |

---

*定制日期：2026-09-12*
*适配角色：Application Support Engineer（L2-L3, Softtek — lululemon）*
*重点场景：Postmortem / RCA 事故报告书面写作*
*配套版本：口语/会议版《Reason_Result_ApplicationSupport_定制版.md》*
