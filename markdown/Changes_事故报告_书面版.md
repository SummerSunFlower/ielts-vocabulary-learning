# 📐 Changes — 事故报告书面版（Postmortem / RCA）

> 基于《Check Your English Vocabulary for IELTS》第12-17页 · 适用：Incident Report / Root Cause Analysis 书面写作
> 适配角色：Application Support / SRE（书面报告写作）

---

## 📌 核心词汇框架

### 词类分类

| 词类 | 含义 | Postmortem 书面应用 |
| --- | --- | --- |
| **指标趋势描述** | 描述"变化方向 / 幅度 / 态势" | incident 期间错误率、延迟、流量、MTTR、SLO 的量化趋势（上升、下降、波动、峰值） |
| **系统状态演变** | 描述"状态 / 性质如何变化" | 根因演变、修复前后对比、架构替换、配置调整、服务恶化与恢复 |

---

## 📈 指标趋势描述词汇 — Incident 指标变化（Changes 1）

### 上升（Upward）

| 词汇 | 用法 | 示例 |
| --- | --- | --- |
| `increase` | v. 上升 | The error rate **increased** from 2% to 9% during the incident.<br>事故期间错误率从 2% 上升到 9%。 |
| `rise` | v. 上升 | P99 latency **rose** steadily throughout the degraded window.<br>P99 延迟在整个劣化窗口期内稳步上升。 |
| `go up` | v. 上升（书面亦可用） | Error volume **went up** sharply after the bad rollout.<br>坏发布后错误量急剧上升。 |
| `peak at` | 短语，达到峰值 | Error rate **peaked at** 12% during the incident window.<br>事故窗口期内错误率峰值达 12%。 |
| `reach a peak of` | 短语，达到…的峰值 | Traffic **reached a peak of** 50k requests per second at 14:00.<br>流量在 14:00 达到每秒 5 万请求的峰值。 |

### 下降（Downward）

| 词汇 | 用法 | 示例 |
| --- | --- | --- |
| `decrease` | v. 下降 | After rollback, the error rate **decreased** to baseline.<br>回滚后错误率下降至基线水平。 |
| `decline` | v. 下降 | Service availability **declined** to 99.2% during the outage.<br>中断期间服务可用性下降至 99.2%。 |
| `drop` | v. 骤降 | Throughput **dropped** by 40% when the cache failed.<br>缓存失效时吞吐量骤降 40%。 |
| `fall` | v. 下降 | The success rate **fell** below the SLO threshold.<br>成功率跌破了 SLO 阈值。 |
| `go down` | v. 下降 | Latency **went down** once the extra replicas were added.<br>增加副本后延迟下降。 |

### 波动与持平（Fluctuation & Stability）

| 词汇 | 用法 | 示例 |
| --- | --- | --- |
| `fluctuate` | v. 波动 | Queue depth **fluctuated** between 1k and 8k during the spike.<br>峰值期间队列深度在 1 千到 8 千之间波动。 |
| `remain constant` | 短语，保持恒定 | The CPU usage **remained constant** throughout the incident.<br>整个事故期间 CPU 使用率保持恒定。 |
| `remain steady` | 短语，保持平稳 | The recovery progress **remained steady** after the fix.<br>修复后恢复进度保持平稳。 |

### 程度副词（Degree Adverbs）

| 词汇 | 用法 | 示例 |
| --- | --- | --- |
| `dramatically` | adv. 剧烈地 | The error rate rose **dramatically** after the config push.<br>配置推送后错误率剧烈上升。 |
| `sharply` | adv. 急剧地 | Latency dropped **sharply** once we disabled the feature flag.<br>关闭功能开关后延迟急剧下降。 |
| `steadily` | adv. 稳定地 | The backlog cleared **steadily** over the next hour.<br>接下来一小时积压稳定地清空。 |
| `gradually` | adv. 逐渐地 | The system **gradually** recovered after the restart.<br>重启后系统逐渐恢复。 |
| `slightly` | adv. 略微地 | Availability improved **slightly** after the first mitigation.<br>第一次缓解后可用性略微改善。 |

### 趋势名词（Trend Nouns）

| 词汇 | 用法 | 示例 |
| --- | --- | --- |
| `upward trend` | n. 上升趋势 | There was an **upward trend** in latency before the alert fired.<br>告警触发前延迟呈上升趋势。 |
| `downward trend` | n. 下降趋势 | A **downward trend** in error rate confirmed the fix worked.<br>错误率的下降趋势证实了修复有效。 |

> **💡 Postmortem 提示：** 趋势词用于量化 incident 指标，是 RCA 时间线与 status 图表说明的标准用语。
>
> Error rate **peaked at** 12% and then **decreased** to baseline within 20 minutes of the rollback.<br>（错误率峰值达 12%，并在回滚后 20 分钟内下降至基线。）
>
> Throughout the degraded window, P99 latency showed a clear **upward trend** before it **dropped sharply** post-mitigation.<br>（在整个劣化窗口期内，P99 延迟在缓解措施后急剧下降之前呈现出明显的上升趋势。）

---

## 🔧 系统状态演变动词 — 根因与修复（Changes 2）

### Group 1

| 词汇 | 用法 | 示例 |
| --- | --- | --- |
| `adjust` | v. 调整 / 适应 | We **adjusted** the timeout to reduce retries.<br>我们调整了超时设置以减少重试。 |
| `alter` | v. 改变 | The patch **altered** the retry logic in the client.<br>该补丁改变了客户端的重试逻辑。 |
| `deteriorate` | v. 恶化 | Service stability **deteriorated** after the bad deploy.<br>坏部署后服务稳定性恶化。 |
| `exchange` | v. 交换 / 更换 | We **exchanged** the faulty node for a healthy one.<br>我们将故障节点更换为正常节点。 |
| `fade` | v. 逐渐消失 / 消退 | The alert storm **faded** once the loop was broken.<br>打破循环后告警风暴逐渐消退。 |
| `reduce` | v. 减少 | The fix **reduced** MTTR from 45 to 12 minutes.<br>该修复将 MTTR 从 45 分钟减少到 12 分钟。 |
| `renovate` | v. 翻新 / 更新 | We **renovated** the runbook to reflect the new architecture.<br>我们翻新了 runbook 以反映新架构。 |
| `swell` | v. 膨胀 / 增大 | The incident channel **swelled** with messages during the outage.<br>中断期间事件频道消息量骤增。 |
| `switch` | v. 切换 | We **switched** the traffic to the standby region.<br>我们将流量切换到备用区域。 |
| `switch to` | 短语，转换到 | We **switched to** the degraded mode to protect the core path.<br>我们切换到降级模式以保护核心路径。 |
| `vary` | v. 变化 / 不同 | Impact **varied** by customer segment and region.<br>影响因客户群和区域而不同。 |

### Group 2

| 词汇 | 用法 | 示例 |
| --- | --- | --- |
| `adapt` | v. 适应 / 改编 | The on-call **adapted** the runbook to the new topology.<br>值班团队将 runbook 改编适配了新拓扑。 |
| `cut` | v. 削减 | We **cut** the rollout to 5% to limit the blast radius.<br>我们将发布比例削减至 5% 以限制爆炸半径。 |
| `decline` | v. 下降 / 减少 | The failure rate **declined** after the hotfix.<br>热修复后故障率下降。 |
| `disappear` | v. 消失 | The intermittent errors **disappeared** after the restart.<br>重启后间歇性错误消失。 |
| `expand` | v. 扩张 / 扩容 | We **expanded** capacity to absorb the traffic surge.<br>我们扩容以吸收流量激增。 |
| `improve` | v. 改善 | Service stability **improved** once we rolled back.<br>回滚后服务稳定性改善。 |
| `promote` | v. 提升 / 晋升（此处：提升发布） | We **promoted** the fix from canary to full rollout.<br>我们将修复从金丝雀提升为全量发布。 |
| `relax` | v. 放松 / 放宽 | We **relaxed** the circuit breaker threshold post-incident.<br>事故后我们放宽了熔断阈值。 |
| `replace` | v. 替换 | We **replaced** the corrupt cache with a fresh instance.<br>我们用全新实例替换了损坏的缓存。 |
| `transform` | v. 彻底转型 / 改变 | The remediation **transformed** the fragile pipeline into a resilient one.<br>该修复将脆弱的流水线彻底转变为有韧性的流水线。 |

> **💡 Postmortem 提示：** 状态动词用于描述根因如何演变、修复如何改变系统，是 "Timeline" 与 "Remediation" 段的核心动词。
>
> Service stability **deteriorated** after the bad deploy, then **improved** once we rolled back and **replaced** the faulty component.<br>（坏部署后服务稳定性恶化，在我们回滚并替换故障组件后得以改善。）

---

## 🎯 场景一：RCA 时间线描述（Incident Timeline）

**流程：** Detection → Impact → Mitigation → Resolution

| 阶段 | 指标变化（趋势词） | 根因演变（状态动词） |
| --- | --- | --- |
| **Detection** | Error rate **rose** sharply and **peaked at** 12%. | Root cause **altered** from config drift to bad rollout. |
| **Impact** | Availability **declined** to 99.1%; latency **went up**. | Blast radius **expanded** across regions. |
| **Mitigation** | Error rate **decreased** after rollback. | We **switched** traffic to the standby region and **adjusted** the breaker. |
| **Resolution** | Metrics **remained steady**; a **downward trend** confirmed. | Root cause **replaced** by a stable configuration. |

> **完整示例（正式 Postmortem 摘要）：** During the Detection phase, the error rate **rose** sharply and **peaked at** 12% within ten minutes of the bad rollout, while the root cause **altered** from suspected config drift to a faulty deployment. In the Impact phase, availability **declined** to 99.1% and P99 latency **went up** by 300 ms as the blast radius **expanded** across two regions. For Mitigation, we **switched** user traffic to the standby region and **adjusted** the circuit breaker threshold, after which the error rate **decreased** to baseline. By Resolution, all metrics **remained steady** and a clear **downward trend** in incidents confirmed the root cause had been **replaced** by a stable configuration.

---

## 🎯 场景二：修复前后对比（Before / After）

**流程：** Faulty state → Remediation → Improved state

| 维度 | 修复前（Before） | 修复后（After） |
| --- | --- | --- |
| **架构** | Monolith with a single cache tier | Cache tier **replaced** with a replicated cluster |
| **流水线** | Fragile, single-region deploy | Pipeline **transformed** into a resilient, multi-region one |
| **MTTR** | 45 minutes | MTTR **reduced** to 12 minutes |
| **稳定性** | Stability **deteriorated** under load | Stability **improved** and remained steady |

> **完整示例：** Before remediation, the platform relied on a monolith with a single cache tier, and stability **deteriorated** under peak load. The remediation **replaced** the single cache tier with a replicated cluster and **transformed** the fragile deploy pipeline into a resilient, multi-region one. As a result, MTTR was **reduced** from 45 to 12 minutes, and service stability **improved** while remaining steady across subsequent load tests. The fragile topology was therefore **transformed** into a self-healing architecture.

---

## 💬 对话一：Postmortem 评审会 — SRE 向管理层口头汇报指标演变

> **SRE:** Thanks for the time. I'll walk through how the key metrics evolved during last night's incident.<br>（谢谢抽空。我来说明昨晚事故期间关键指标是如何演变的。）
>
> **Manager:** Go ahead. What did the error rate do?<br>（请讲。错误率是什么走势？）
>
> **SRE:** The error rate **peaked at** about 12% around 02:10, roughly twenty minutes after the bad rollout.<br>（错误率在 02:10 左右达到约 12% 的峰值，也就是坏发布后约二十分钟。）
>
> **Manager:** And during the window, was it stable at all?<br>（那在窗口期内，它有过稳定吗？）
>
> **SRE:** Between mitigations, the rate **remained steady** at around 4% while we investigated the root cause.<br>（在两次缓解之间，错误率在我们排查根因时保持在约 4% 的平稳状态。）
>
> **Manager:** How bad did it get before we acted?<br>（在我们采取行动前，情况有多糟？）
>
> **SRE:** Before rollback, service stability **deteriorated** sharply and availability dropped below our SLO.<br>（回滚前，服务稳定性急剧恶化，可用性跌破了我们的 SLO。）
>
> **Manager:** And now?<br>（那现在呢？）
>
> **SRE:** Once we rolled back and switched traffic, the system **recovered** and the error rate fell back to baseline within half an hour.<br>（一旦我们回滚并切换流量，系统就恢复了，错误率在半小时内回落到基线。）

---

## 💬 对话二：跨部门书面报告评审（Written Review）

> **Reviewer:** I've read the draft RCA. Can you clarify the remediation section?<br>（我读了 RCA 草稿。能说明一下修复这一段吗？）
>
> **Author:** Certainly. We first **switched** the serving path from the legacy gateway to the new proxy.<br>（当然。我们首先把服务路径从旧网关切换到了新代理。）
>
> **Reviewer:** And the corrupt cache?<br>（那损坏的缓存呢？）
>
> **Author:** We **replaced** the corrupt cache with a fresh, replicated instance to stop the data loss.<br>（我们用全新的、带复制的实例替换了损坏的缓存，以阻止数据丢失。）
>
> **Reviewer:** Did the runbook help, or did you change it?<br>（runbook 帮上忙了吗，还是你们改了它？）
>
> **Author:** We **adapted** the runbook to the new topology so on-call could follow it next time.<br>（我们把 runbook 改编适配了新拓扑，这样下次值班团队就能照着执行。）
>
> **Reviewer:** Good. And the bigger picture?<br>（很好。那更宏观的层面呢？）
>
> **Author:** The remediation **transformed** our fragile single-region setup into a resilient, multi-region platform.<br>（这次修复把我们脆弱的单区域架构彻底转型成了有韧性的多区域平台。）

---

## 📊 Postmortem 速查表

### 指标趋势（Metrics）

| 想表达 | 正式书面表达 |
| --- | --- |
| **错误率飙升到顶点** | The error rate rose sharply and peaked at 12% during the incident window. |
| **延迟持续上升** | P99 latency showed an upward trend and rose steadily before mitigation. |
| **可用性下降** | Availability declined to 99.1%, falling below the SLO threshold. |
| **回滚后指标恢复** | After rollback, the error rate decreased to baseline and remained steady. |
| **流量激增** | Inbound traffic went up and reached a peak of 50k RPS at 14:00. |

### 状态演变（State Changes）

| 想表达 | 正式书面表达 |
| --- | --- |
| **稳定性恶化** | Service stability deteriorated after the bad deploy, then improved after rollback. |
| **替换故障组件** | We replaced the corrupt cache with a fresh, replicated instance. |
| **架构彻底转型** | The remediation transformed the fragile pipeline into a resilient one. |
| **削减发布范围** | We cut the rollout to 5% to limit the blast radius during remediation. |
| **缩短恢复时间** | The fix reduced MTTR from 45 to 12 minutes and expanded capacity for surges. |

---

## 🚀 实战练习（Postmortem 语境）

### 练习一：趋势词填空

> **Timeline:** The error rate __________ sharply right after the bad rollout and __________ at 12% within ten minutes. After we rolled back, it __________ to baseline and then __________ steady for the rest of the window. A clear __________ in incidents confirmed the fix.

### 练习二：状态动词填空

> **Remediation:** Service stability __________ after the faulty deploy, so we __________ the corrupt cache with a fresh instance and __________ traffic to the standby region. These steps __________ our fragile setup and __________ MTTR from 45 to 12 minutes.

### 练习三：场景写作

> **任务：** 用至少 4 个趋势词（如 peaked at / decreased / remained steady / upward trend）和 3 个状态动词（如 deteriorated / replaced / transformed），写一段 3–4 句的正式 Postmortem 摘要。
