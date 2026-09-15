# IELTS Vocabulary Learning 📚

基于《Check Your English Vocabulary for IELTS》的专业词汇学习系统，提供精美的 HTML 交互式学习界面。

[![HTML Version](https://img.shields.io/badge/HTML-精美版-blue)](https://summersunflower.github.io/ielts-vocabulary-learning/) [![Markdown](https://img.shields.io/badge/Markdown-源文件-green)](./markdown/)

## 🌐 在线访问

**https://summersunflower.github.io/ielts-vocabulary-learning/**

手机、平板、电脑均可直接访问，无需下载。

---

## 🚀 本地使用（可选）

```bash
git clone https://github.com/SummerSunFlower/ielts-vocabulary-learning.git
cd ielts-vocabulary-learning/docs/
python3 -m http.server 8000
```
然后访问 `http://localhost:8000`（或直接用浏览器打开 `docs/index.html`）

---

## 📚 项目结构

```
ielts-vocabulary-learning/
│
├── 📂 docs/                          # ⭐ HTML 学习网站（GitHub Pages 部署目录）
│   ├── index.html                     # 首页（导航、进度追踪）
│   ├── chapters/                      # 章节内容
│   │   ├── how-something-works.html   # Unit 1: How Something Works
│   │   ├── reason-result.html         # Unit 2: Reason & Result (Support 版)
│   │   ├── reason-result-postmortem.html # Unit 2 场景: 事故报告书面版
│   │   ├── reason-result-pm.html      # Unit 2 场景: PM 项目管理
│   │   ├── reason-result-agile.html   # Unit 2 场景: 敏捷会议
│   │   ├── reason-result-external.html # Unit 2 场景: 客户/供应商
│   │   ├── changes-support.html       # Unit 3: Changes (Support 版)
│   │   ├── changes-postmortem.html    # Unit 3 场景: 事故报告书面版
│   │   ├── changes-pm.html            # Unit 3 场景: PM 项目管理
│   │   ├── changes-agile.html         # Unit 3 场景: 敏捷会议
│   │   └── changes-external.html      # Unit 3 场景: 客户/供应商
│   ├── exercises/                     # 练习页面
│   │   ├── reason-result-exercises.html
│   │   └── changes-exercises.html
│   ├── tests/                         # 测试页面
│   │   ├── reason-result-test.html
│   │   └── changes-test.html
│   └── assets/
│       └── css/
│           └── style.css              # 样式表
│
└── 📂 markdown/                       # Markdown 源文件（便于编辑）
    ├── How_Something_Works_词汇笔记.md
    ├── Reason_Result_ApplicationSupport_定制版.md
    ├── Reason_Result_事故报告_书面版.md
    ├── Reason_Result_PM场景_定制版.md
    ├── Reason_Result_敏捷会议_定制版.md
    ├── Reason_Result_客户供应商沟通_定制版.md
    ├── Reason_Result_练习集.md
    ├── Reason_Result_严格测试.md
    ├── Changes_ApplicationSupport_定制版.md
    ├── Changes_事故报告_书面版.md
    ├── Changes_PM场景_定制版.md
    ├── Changes_敏捷会议_定制版.md
    ├── Changes_客户供应商沟通_定制版.md
    ├── Changes_练习集.md
    └── Changes_严格测试.md
```

### 💡 为什么有两个版本？

- **HTML 版本（`docs/`）：** 精美设计，交互式学习，适合日常使用，已部署为在线网站
- **Markdown 版本（`markdown/`）：** 纯文本格式，方便用任何编辑器修改内容

---

## 🎯 HTML 版本特点

- 📖 **精美设计**：现代化 UI，渐变背景，卡片式布局
- 🔍 **清晰导航**：首页 → 章节 → 练习 → 测试，结构清晰
- 📱 **响应式布局**：完美支持手机、平板、电脑
- 🎨 **专业排版**：对话场景、词汇卡片、练习交互
- 📊 **进度追踪**：可视化学习进度展示

---

## 📝 学习内容

### 第一章：How Something Works
描述设备/系统工作原理的词汇
- **适用场景：** 雅思听力、写作 Task 1
- **核心词汇：** component, mechanism, function, operate, generate 等

### 第二章：Reason & Result（5 大业务场景定制）
表达"原因、目的、结果"的词汇 —— 同一套 15 个核心词，5 个场景定制版：

| 场景 | 页面 | 适用 |
|------|------|------|
| 💬 Application Support | `chapters/reason-result.html` | 故障通报、会议讨论、跨团队协作（口语） |
| 📄 事故报告书面版 | `chapters/reason-result-postmortem.html` | Postmortem / RCA / Incident Report 书面写作 |
| 📋 PM 项目管理 | `chapters/reason-result-pm.html` | 进度汇报、延期解释、风险上报、资源协调 |
| 🏃 敏捷会议 | `chapters/reason-result-agile.html` | Daily Standup、Sprint Review、Retrospective |
| 🤝 客户/供应商 | `chapters/reason-result-external.html` | 延误通知、SLA 沟通、期望管理（对外正式） |

**核心词汇：** due to, owing to, on the grounds that, in order to, with the aim of, as a result, as a consequence, ensued, affect, motive 等 15 词

### 第三章：Changes（5 大业务场景定制）
描述"变化与趋势"的词汇 —— 同一套约 40 个核心词，5 个场景定制版，适用于雅思写作 Task 1（图表题）、状态汇报、RCA、进度趋势沟通：

| 场景 | 页面 | 适用 |
|------|------|------|
| 💬 Application Support | `chapters/changes-support.html` | 故障指标趋势、系统迁移、工具切换（口语/会议） |
| 📄 事故报告书面版 | `chapters/changes-postmortem.html` | RCA 时间线、指标演变、修复前后对比（书面） |
| 📋 PM 项目管理 | `chapters/changes-pm.html` | 进度偏差趋势、范围/资源调整、风险等级演变 |
| 🏃 敏捷会议 | `chapters/changes-agile.html` | Sprint 速率、燃尽图趋势、流程改进（Standup/Review/Retro） |
| 🤝 客户/供应商 | `chapters/changes-external.html` | SLA 指标变化通知、交付范围调整、期望管理（对外正式） |

**核心词汇（Changes 1 趋势）：** increase, rise, go up, peak at, reach a peak of, decrease, decline, drop, fall, go down, fluctuate, remain constant, remain steady, dramatically, sharply, steadily, gradually, slightly, upward/downward trend
**核心词汇（Changes 2 状态变化动词）：** adjust, alter, deteriorate, exchange, fade, reduce, renovate, swell, switch, vary, adapt, cut, decline, disappear, expand, improve, promote, relax, replace, transform

---

## 🛠️ 技术栈

- **前端：** HTML5 + CSS3
- **部署：** GitHub Pages（静态托管）
- **设计：** 响应式设计、CSS Grid、Flexbox
- **特色：** 渐变背景、卡片布局、流畅动画

---

## 📄 许可证

学习用途，请遵守原书版权。

---

**项目创建：** 2026-03-19  
**HTML 版本：** 2026-05-09  
**在线部署：** 2026-09-12  
**Chapter 3 (Changes) 上线：** 2026-09-14
