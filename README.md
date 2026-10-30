<!-- 这份文件会被渲染在你的 GitHub 主页顶部。 -->

### 蒲公英

Java 后端，最近在把大模型接进 Spring 服务里。

这儿的仓库基本是**学习笔记和练习项目**，不是生产代码 —— 但尽量做到每一步能跑、能复现、点开就能看。

<a href="https://pgy763.github.io/algo-stage/">
  <img src="https://raw.githubusercontent.com/pgy763/algo-stage/main/docs/screenshots/home.png" alt="AlgoStage：把算法一行一行演给你看" width="100%">
</a>

<p align="right"><sub>↑ algo-stage：<a href="https://pgy763.github.io/algo-stage/">点开就能拖进度条看</a></sub></p>

---

**能直接点开看的**

| 项目 | 是什么 | 可以验证什么 |
| --- | --- | --- |
| [algo-stage](https://github.com/pgy763/algo-stage) | 把算法一行一行演给你看：18 个算法 + 5 种语言的代码实验台 | [在线试](https://pgy763.github.io/algo-stage/) · 76 个测试 · CI 全绿 |
| [hello-ai-backend](https://github.com/pgy763/hello-ai-backend) | 写给 Java 后端的 AI 接入手册：补「能调通 API」到「能上生产」中间那一段 | [在线阅读](https://pgy763.github.io/hello-ai-backend/) |
| [llm-dev-pitfalls](https://github.com/pgy763/llm-dev-pitfalls) | LLM 开发踩坑手册（Spring AI / LangChain4j），按报错关键词索引，不按阅读顺序 | 1.1 万字，持续更新 |

**在写的代码**

| 项目 | 一句话 |
| --- | --- |
| [llm-gateway](https://github.com/pgy763/llm-gateway) | 多个系统共用 AI 时，把调用统一管起来的接入网关（Spring Boot 3 + Java 21） |
| [shopkeeper-agent](https://github.com/pgy763/shopkeeper-agent) | 中文提问直接出数：FastAPI + LangGraph + RAG 的 NL2SQL 智能体 |
| [prompt-ops](https://github.com/pgy763/prompt-ops) | 把 Prompt 当代码管理：版本、diff、回归测试 |
| [Blog-](https://github.com/pgy763/Blog-) | Spring Boot 3 + Spring AI 的全栈博客：前台、后台、AI 助手 |

**技术栈 · 分别用在哪**

- `Java` `Spring Boot` `Spring AI` `LangChain4j` → llm-gateway、hello-ai-backend
- `Python` `FastAPI` `LangGraph` `RAG` → shopkeeper-agent
- `Vue 3` → algo-stage（渲染层零依赖，手写 SVG / DOM）
- `MySQL` `Redis` → 上面几个项目的存储层

**最近**

- 2026-10：给 algo-stage 补了堆排序、并查集、LIS、编辑距离、Trie 五个算法，并加上 CI 门禁和 CHANGELOG
- 一直在更：hello-ai-backend 的正文、llm-dev-pitfalls 的报错条目

**联系**

开 Issue 就行，报错、勘误、想问的都收。