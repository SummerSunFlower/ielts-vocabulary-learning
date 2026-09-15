# 📐 Changes — Application Support 定制版

> 基于《Check Your English Vocabulary for IELTS》第12-17页 · 适用角色：Application Support Engineer

## 📌 核心词汇框架

### 词类分类

| 词类 | 含义 | Support 场景应用 |
| --- | --- | --- |
| **趋势描述类** | 描述数字、指标、数据随时间的变化方向 | 故障指标汇报、容量趋势、工单量 / 延迟 / 错误率走势 |
| **状态变化类** | 描述系统、服务、流程的状态或性质的改变 | 系统迁移、服务状态切换、工具替换、事件复盘 |

## 📈 趋势描述类词汇（Changes 1）

### 上升 / 下降 / 波动

| 词汇 | 用法 | 示例 |
| --- | --- | --- |
| `increase` | v. 上升 | The error rate `increased` after the deploy.<br>（部署后错误率上升了。） |
| `rise` | v. 上升 | Latency `rose` from 200ms to 800ms during peak hours.<br>（高峰时段延迟从 200ms 升到 800ms。） |
| `go up` | v. 上升（口语） | Ticket volume `went up` by 40% this week.<br>（本周工单量上升了 40%。） |
| `peak at` | v. 达到峰值 | CPU usage `peaked at` 95% at 14:00.<br>（CPU 使用率在 14:00 达到峰值 95%。） |
| `reach a peak of` | v. 达到…的峰值 | The queue length `reached a peak of` 12,000 messages.<br>（队列长度达到峰值 12,000 条消息。） |
| `decrease` | v. 下降 | Memory consumption `decreased` after the patch.<br>（打补丁后内存消耗下降了。） |
| `decline` | v. 下降 | The success rate `declined` over the weekend.<br>（成功率在周末下降了。） |
| `drop` | v. 下降（骤降） | Throughput `dropped` to 50 requests per second.<br>（吞吐量骤降到每秒 50 个请求。） |
| `fall` | v. 下降 | Availability `fell` below the 99.9% SLA target.<br>（可用性跌破了 99.9% 的 SLA 目标。） |
| `go down` | v. 下降（口语） | The false-positive alerts `went down` after tuning.<br>（误报在调优后减少了。） |
| `fluctuate` | v. 波动 | Response time `fluctuated` between 300ms and 1.2s.<br>（响应时间在 300ms 到 1.2 秒之间波动。） |
| `remain constant` | v. 保持恒定 | Disk I/O `remained constant` throughout the incident.<br>（整个故障期间磁盘 I/O 保持恒定。） |
| `remain steady` | v. 保持平稳 | The throughput `remained steady` at 2,000 rps.<br>（吞吐量保持在 2000 rps 平稳。） |

### 程度副词（修饰变化幅度）

| 词汇 | 用法 | 示例 |
| --- | --- | --- |
| `dramatically` | adv. 急剧地 | Errors rose `dramatically` after the bad release.<br>（糟糕的发布后错误急剧上升。） |
| `sharply` | adv. 急剧地 | Latency dropped `sharply` once we scaled out.<br>（扩容后延迟急剧下降。） |
| `steadily` | adv. 稳定地 | The backlog cleared `steadily` after the fix.<br>（修复后积压稳定地清空。） |
| `gradually` | adv. 逐渐地 | Performance improved `gradually` as the cache warmed up.<br>（随着缓存预热，性能逐渐改善。） |
| `slightly` | adv. 略微 | CPU dipped `slightly` after the config change.<br>（配置变更后 CPU 略微下降。） |

### 趋势名词

| 词汇 | 用法 | 示例 |
| --- | --- | --- |
| `upward trend` | n. 上升趋势 | There is an `upward trend` in ticket volume.<br>（工单量呈上升趋势。） |
| `downward trend` | n. 下降趋势 | We see a `downward trend` in MTTR this quarter.<br>（本季度 MTTR 呈下降趋势。） |

> **💡 Support 场景提示：** 这些词在 incident report、postmortem 和容量周报里高频出现，用于客观描述指标走向，避免主观措辞。
>
> The error rate `increased` `dramatically` after the deploy, then `peaked at` 8% before the rollback brought it back down.<br>（部署后错误率急剧上升，在回滚把它降下来之前达到峰值 8%。）

## 🔧 状态变化类动词（Changes 2）

### Group 1

| 词汇 | 用法 | 示例 |
| --- | --- | --- |
| `adjust` | v. 调整 / 适应 | We `adjusted` the timeout to 30 seconds.<br>（我们把超时调整为 30 秒。） |
| `alter` | v. 改变 | The deploy `altered` the routing rules.<br>（部署改变了路由规则。） |
| `deteriorate` | v. 恶化 | Service health `deteriorated` after the traffic spike.<br>（流量激增后服务健康度恶化。） |
| `exchange` | v. 交换 | We `exchanged` the faulty node for a healthy one.<br>（我们用健康节点替换了故障节点。） |
| `fade` | v. 逐渐消失 / 褪色 | The cached session `faded` after the TTL expired.<br>（缓存会话在 TTL 到期后逐渐消失。） |
| `reduce` | v. 减少 | We `reduced` the retry count to cut load.<br>（我们减少了重试次数以降低负载。） |
| `renovate` | v. 翻新 | The team `renovated` the legacy logging pipeline.<br>（团队翻新了旧的日志管道。） |
| `swell` | v. 膨胀 / 增大 | The error log `swelled` to 2 GB overnight.<br>（错误日志一夜之间膨胀到 2 GB。） |
| `switch` | v. 转换（switch to） | We `switched` to the standby database.<br>（我们切换到了备用数据库。） |
| `vary` | v. 变化 / 不同 | Response times `vary` by region.<br>（响应时间因地区而异。） |

### Group 2

| 词汇 | 用法 | 示例 |
| --- | --- | --- |
| `adapt` | v. 适应 / 改编 | The runbook was `adapted` for the new stack.<br>（操作手册为新架构做了改编。） |
| `cut` | v. 削减 | We `cut` the batch size to relieve pressure.<br>（我们削减了批处理大小以缓解压力。） |
| `decline` | v. 下降 / 拒绝 | The vendor `declined` the rollback request.<br>（供应商拒绝了回滚请求。） |
| `disappear` | v. 消失 | The intermittent timeout `disappeared` after the fix.<br>（间歇性超时在修复后消失了。） |
| `expand` | v. 扩张 | We `expanded` capacity ahead of the campaign.<br>（活动前我们扩张了容量。） |
| `improve` | v. 改善 | Observability `improved` after adding tracing.<br>（增加追踪后，可观测性改善了。） |
| `promote` | v. 提升 / 晋升 | She was `promoted` to on-call lead.<br>（她被晋升为值班负责人。） |
| `relax` | v. 放松 | We `relaxed` the rate limit during maintenance.<br>（维护期间我们放宽了限流。） |
| `replace` | v. 替换 | The legacy system was `replaced` by microservices.<br>（旧系统被微服务架构取代了。） |
| `transform` | v. 彻底转型 / 改变 | The incident process was `transformed` by automation.<br>（事件流程被自动化彻底改变了。） |

> **💡 Support 场景提示：** 这组动词用于迁移通知、状态变更、事件复盘，描述"系统从 A 状态变成 B 状态"。
>
> The legacy platform was `replaced` by the new microservices architecture, and the on-call burden `improved` `gradually` over the next two sprints.<br>（旧平台被新微服务架构取代，随后两个迭代里值班负担逐渐改善。）

## 🎯 场景一：故障指标汇报（Metric Reporting）

**流程：** 现状 → 趋势描述 → 根因 → 影响 → 修复后对比

| 步骤 | 模板 | 示例 |
| --- | --- | --- |
| **现状** | Current status: X is showing... | Current status: the checkout API is showing elevated error rates. |
| **趋势描述** | The error rate increased / dropped... | The error rate `increased` `dramatically` and `peaked at` 9%. |
| **根因** | Root cause: X altered / deteriorated... | Root cause: a config change `altered` the connection pool size. |
| **影响** | This affected Y, ticket volume went up... | This `affected` checkout, and ticket volume `went up` by 60%. |
| **修复后对比** | After the fix, X dropped sharply... | After the rollback, the error rate `dropped` `sharply` to baseline. |

> **完整示例：** Current status: the payments service is showing elevated latency. The p99 latency `rose` from 300ms to 1.4s and `peaked at` 1.4s at 13:00, then `fluctuated` for 20 minutes. Root cause: a bad deploy `altered` the caching layer and service health `deteriorated`. This `affected` the retail client's checkout, and ticket volume `went up` by 60%. After we `switched` to the previous build, latency `dropped` `sharply` and remained steady at 300ms. We `reduced` the retry count to prevent a retry storm.

## 🎯 场景二：系统迁移 / 工具切换通报（Migration & Tool Switch）

**流程：** 背景 → 变更动作 → 过渡状态 → 预期收益 → 回滚预案

| 步骤 | 模板 | 示例 |
| --- | --- | --- |
| **背景** | We are migrating X to Y... | We are migrating the alerting stack from Nagios to Prometheus. |
| **变更动作** | The legacy system was replaced by... | The legacy platform was `replaced` by the new microservices architecture. |
| **过渡状态** | We switched to / adapted the runbook... | We `switched` to the standby cluster and `adapted` the runbook. |
| **预期收益** | Observability improved / MTTR went down... | Observability `improved` and MTTR `went down` by 30%. |
| **回滚预案** | If it fails, we will exchange / revert... | If it fails, we will `exchange` the new node for the old one. |

> **完整示例：** We are migrating our monitoring from the legacy tool to a new observability suite. Over the weekend the old dashboard was `replaced` by the new one, and the on-call runbook was `adapted` for the new queries. During cutover we `switched` traffic to the standby region so the main region could be `renovated`. Capacity was `expanded` ahead of the retail client's campaign, and alert noise `reduced` after we `relaxed` two noisy rules. If the new stack misbehaves, we will `exchange` it back to the previous version within 15 minutes.

## 💬 对话一：Slack / 会议中向 Dev 通报指标异常并请求协助

> **Support:** Hey, I'm seeing the error rate on the checkout API `increase` `dramatically` in the last 10 minutes. Can you take a look?<br>（Support：嘿，我看到结账 API 的错误率在过去 10 分钟急剧上升，能帮忙看下吗？）
>
> **Dev:** On it. What's the number now?<br>（Dev：在处理。现在到多少了？）
>
> **Support:** It `peaked at` about 9%, and the latency also `rose` from 300ms to over a second. Service health is starting to `deteriorate`.<br>（Support：峰值约 9%，延迟也从 300ms 升到一秒多，服务健康度开始恶化。）
>
> **Dev:** Looks like the last deploy `altered` the connection pool config. I'll roll it back.<br>（Dev：看起来上次部署改了连接池配置，我回滚一下。）
>
> **Support:** Good. Meanwhile I'll `switch` to the standby database to protect the main one. Ticket volume is already `going up`.<br>（Support：好，同时我切到备用库保护主库，工单量已经在涨了。）
>
> **Dev:** Rolled back. Did the error rate `drop`?<br>（Dev：已回滚，错误率降了吗？）
>
> **Support:** Yes, it `dropped` `sharply` and is `remaining steady` now. To avoid a retry storm I `reduced` the retry count on the client side. Thanks for the quick fix.<br>（Support：降了，急剧下降，现在平稳。为避免重试风暴我把客户端重试次数调小了，多谢快速修复。）

## 💬 对话二：跨团队 incident 复盘会议（Postmortem）

> **Support Lead:** Let's review the payments incident. First, the p99 latency `peaked at` 1.8s and the error rate stayed high for 25 minutes.<br>（Support Lead：我们复盘下支付故障。首先 p99 延迟峰值到 1.8 秒，错误率高企了 25 分钟。）
>
> **SRE:** Right. During that window the CPU usage `fluctuated`, but the queue length `remained steady`, so it wasn't a throughput issue.<br>（SRE：对，那段时间 CPU 有波动，但队列长度保持平稳，所以不是吞吐问题。）
>
> **Dev:** The root cause was a cache bug. After the fix, latency `went down` and the success rate `improved` `gradually` over the next hour.<br>（Dev：根因是缓存 bug。修复后延迟下降，成功率在接下来一小时逐渐改善。）
>
> **Support Lead:** Good. Longer term, the legacy cache was `replaced` by a distributed one, which `transformed` our incident handling. Our MTTR `went down` by 35% this quarter, a clear `downward trend`.<br>（Support Lead：很好。长期看，旧缓存被分布式缓存取代，彻底改变了我们的事件处理。本季度 MTTR 下降 35%，呈明显下降趋势。）
>
> **PM:** And we `expanded` the on-call coverage, so the alert noise `reduced` and page volume `declined`. Nice work, team.<br>（PM：我们还扩大了值班覆盖，告警噪音减少、呼叫量下降。干得好，团队。）

## 📊 Support 场景速查表

### 趋势汇报（Incident / Postmortem / 容量周报）

| 想表达 | 常用表达 |
| --- | --- |
| **指标骤升** | The error rate increased dramatically and peaked at X%. |
| **指标回落** | Latency dropped sharply and remained steady at Yms. |
| **波动 / 持平** | CPU fluctuated, but throughput remained constant. |
| **工单 / 负载变化** | Ticket volume went up by 40% this week. |
| **趋势判断** | There is an upward / downward trend in MTTR. |

### 状态变更（迁移 / 切换 / 事件复盘）

| 想表达 | 常用表达 |
| --- | --- |
| **系统被替换** | The legacy system was replaced by the new architecture. |
| **切换 / 适配** | We switched to the standby node and adapted the runbook. |
| **状态恶化 / 改善** | Health deteriorated, then improved gradually after the fix. |
| **削减 / 扩张** | We cut the batch size and expanded capacity ahead of the campaign. |
| **彻底改变** | Automation transformed our incident process. |

## 🚀 实战练习（Support 场景）

### 练习一：指标汇报填空

> **Incident Update:** The checkout API error rate __________ from 1% to 9% and __________ 9% at 13:00. Service health __________ after the traffic spike, so we __________ to the standby database. After the rollback, latency __________ and the success rate __________ over the next hour.

### 练习二：迁移通报填空

> **Migration Note:** The legacy monitor was __________ by the new stack, and the runbook was __________ for the new queries. We __________ traffic to the standby region while the main one was __________. Capacity was __________ ahead of the campaign, and alert noise __________. If it fails, we will __________ it back within 15 minutes.

### 练习三：复盘填空

> **Postmortem:** p99 latency __________ 1.8s, and the queue length __________ during that window. After the fix, MTTR __________ by 35% this quarter — a clear __________ in our response time.
