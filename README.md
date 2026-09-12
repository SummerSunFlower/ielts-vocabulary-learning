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
│   │   └── reason-result.html         # Unit 2: Reason & Result
│   ├── exercises/                     # 练习页面
│   │   └── reason-result-exercises.html
│   ├── tests/                         # 测试页面
│   │   └── reason-result-test.html
│   └── assets/
│       └── css/
│           └── style.css              # 样式表
│
└── 📂 markdown/                       # Markdown 源文件（便于编辑）
    ├── How_Something_Works_词汇笔记.md
    ├── Reason_Result_ApplicationSupport_定制版.md
    ├── Reason_Result_练习集.md
    └── Reason_Result_严格测试.md
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

### 第二章：Reason & Result
表达"原因、目的、结果"的词汇（已定制为 Application Support 场景）
- **适用场景：** 口语沟通、会议讨论、跨团队协作、故障通报
- **核心词汇：** because, due to, in order to, as a result, consequently 等

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
