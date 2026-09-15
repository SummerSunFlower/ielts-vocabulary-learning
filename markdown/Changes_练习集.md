# Changes 练习集（Chapter 3）

基于《Check Your English Vocabulary for IELTS》第12-17页。描述变化与趋势，5 大业务场景通用。

## 练习类型
- 词汇填空（基础巩固）
- 句子改写（口语 → 精确/正式）
- 情境对话（模拟真实工作）
- 错误改正（常见错误）
- 翻译练习（中译英）

## 练习一：词汇填空

### 1.1 趋势描述词（Changes 1）
1. After the fix, error rate **dropped** from 8% to 1.2% within an hour.
2. API latency **rose** steadily from 90ms to 140ms during the traffic surge.
3. Traffic **peaked at** 14:00 and then started to taper off.
4. CPU utilization **fluctuated** between 40% and 70% throughout the night.
5. Uptime **remained steady** at 99.95% for the whole quarter.
6. The number of open incidents **reached a peak of** 47 during the outage.
7. Once caching was enabled, database load **dropped** dramatically.
8. Daily active users **remained constant** despite the marketing pause.

### 1.2 程度副词
1. Response time improved **dramatically** after the DB upgrade.
2. The queue length grew **steadily** as the batch job stalled.
3. Memory usage crept up **gradually** before the OOM kill.
4. Throughput dropped **sharply** when the rate limiter kicked in.
5. The metric moved only **slightly** between 09:00 and 10:00.

### 1.3 状态变化动词（Changes 2）
1. We **switched** to a different monitoring tool.
2. The legacy billing system was **replaced** by a cloud-native platform.
3. Service stability began to **deteriorate** after the bad deploy.
4. We **cut** two low-priority features from the release.
5. We **adjusted** the retry timeout to avoid cascading failures.
6. The on-call roster was **expanded** to cover the holiday peak.
7. Error handling **improved** significantly once we added structured logging.
8. The runbook had to be **adapted** to the new incident process.
9. Customer satisfaction **varies** a lot by region and channel.
10. The migration **transformed** the way we ship to production.

## 练习二：句子改写
- The number of errors **increased** after the release.
- Latency **dropped sharply** when we cached the responses.
- The load **fluctuated** all night.
- Traffic **peaked at** 12k requests at noon.
- The metric **remained steady** for the whole month.
- We **replaced** the old server with a new one.
- The process **improved** after the retro actions.
- We **expanded** the team for the launch.
- The incident **deteriorated** before we rolled back.
- We **switched** the workload to a different region.

## 练习三：情境对话
见 HTML 版三个场景填空（Support 指标通报 / PM 进度汇报 / Postmortem 迁移说明）。

## 练习四：错误改正
1. ❌ rised → ✅ rose / peaked at
2. ❌ reduced down → ✅ dropped / reduced
3. ❌ replaced ... to → ✅ replaced ... with
4. ❌ remained steadily → ✅ remained steady
5. ❌ transformed（语义过重）→ ✅ improved / changed

## 练习五：翻译（中译英）
- After the deploy, the error rate dropped from 8% to 1.2%.
- Traffic peaked at 2 PM.
- We replaced the legacy system with the new microservices architecture.
- Service stability improved gradually after the fix.
- Daily active users remained constant due to the marketing pause.
- Error rate on checkout increased from 1% to 8% in 20 minutes, affecting ~3,000 orders. Traced to the 2 PM deploy.
- During the incident, error rate increased sharply and remained above 10% for 40 min. Root cause: legacy proxy replaced by new gateway without config tuning. After adjusting timeouts, stability recovered.
- Schedule variance expanded from 5 to 12 days due to vendor API delay. We moved two backend engineers to protect the critical path; velocity should improve gradually next sprint.
