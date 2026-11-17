<!-- 这份文件会被渲染在你的 GitHub 主页顶部。 -->

### 蒲公英

Java 后端，最近在把大模型接进 Spring 服务里。

**入口只有一个：[pgy763.github.io](https://pgy763.github.io/)** —— 书、手册、项目、工具，都在那儿，不用在这儿翻仓库。

---

### 三个不依赖任何服务的小工具

一条命令、单文件输出、不联网。每个都在解决一件"你以为已经解决了"的事：

| | 给谁 | 解决什么 | 先看效果 |
| --- | --- | --- | --- |
| **DiskMap** | 硬盘红了却说不出原因的 Windows 用户 | 扫一遍出一张能下钻的树图，面积就是体积。我自己的 C 盘：214GB / 764,363 个文件 / 209 秒，重复文件 12.8GB、一年没动 16.5GB | [在线报告](https://pgy763.github.io/diskmap/) · [41 秒视频](https://github.com/pgy763/diskmap/blob/main/docs/demo-v1.mp4) |
| **BillBook** | 想看年度账单又不想把账单传上云的人 | 支付宝 / 微信导出文件 → 一份离线 HTML 年报。顺手修掉「不计收支」被算成消费的坑：我这份虚高 34%，多算 6 万 2 | [在线报告](https://pgy763.github.io/billbook/) · [40 秒视频](https://github.com/pgy763/billbook/blob/main/docs/demo-v1.mp4) |
| **silent-audit** | 用 AI 写脚本、然后对着 `exit 0` 说"完成了"的人 | 脚本说处理了 1000 行，它去数一遍：0 行。脚本改写 `data.csv`，它发现你写成了 `data(1).csv`。把「说干了」和「真干了」分成两件事 | [看它怎么抓](https://github.com/pgy763/silent-audit#readme) |

---

这本书、这份手册、这个项目，外加一个检查器，说的是同一件事的几面：

| | 讲什么 | 点开 |
| --- | --- | --- |
| **Hello, AI Backend** | 怎么把 AI 接进 Spring Boot：15 章，每章配一个能跑的模块 | [在线阅读](https://pgy763.github.io/hello-ai-backend/) |
| **LLM 开发踩坑手册** | 接的过程中会踩什么坑：51 条，按报错关键词搜 | [搜报错](https://pgy763.github.io/llm-dev-pitfalls/all) |
| **Shopkeeper Agent** | 完整做一个能用的东西：NL2SQL，12 个 LangGraph 节点 | [看代码](https://github.com/pgy763/shopkeeper-agent) |
| **llm-lint** | 把最贵的十五条坑做成命令行，在 commit 之前拦住；也能出 SARIF 接进 code scanning | [看工具](https://github.com/pgy763/llm-lint) |

<a href="https://pgy763.github.io/algo-stage/">
  <img src="https://raw.githubusercontent.com/pgy763/algo-stage/main/docs/screenshots/home.png" alt="AlgoStage：把算法一行一行演给你看" width="100%">
</a>

<p align="right"><sub>另外还有 <a href="https://pgy763.github.io/algo-stage/">algo-stage</a>：把算法一行一行演给你看，可以拖进度条</sub></p>

---

**还在写的**

| 项目 | 一句话 |
| --- | --- |
| [llm-gateway](https://github.com/pgy763/llm-gateway) | 多个系统共用 AI 时，把调用统一管起来的接入网关（Spring Boot 3 + Java 21） |
| [prompt-ops](https://github.com/pgy763/prompt-ops) | 把 Prompt 当代码管理：版本、diff、回归测试（MVP，12 个接口） |
| [Blog-](https://github.com/pgy763/Blog-) | Spring Boot 3 + Spring AI 的全栈博客：前台、后台、AI 助手 |

**技术栈 · 分别用在哪**

- `Java` `Spring Boot` `Spring AI` `LangChain4j` → hello-ai-backend、llm-gateway
- `Python` `FastAPI` `LangGraph` `RAG` → shopkeeper-agent
- `Vue 3` → algo-stage（渲染层零依赖，手写 SVG / DOM）
- `MySQL` `Redis` `Qdrant` `Elasticsearch` → 上面几个项目的存储层

**最近**

- 2026-11：做了三个小工具 —— [DiskMap](https://github.com/pgy763/diskmap)（磁盘树图）、[BillBook](https://github.com/pgy763/billbook)（账单年报）、[silent-audit](https://github.com/pgy763/silent-audit)（识别"退出码 0 但什么都没干"的脚本）；踩坑手册扩到 51 条并上线可搜索站点；把其中最贵的坑做成 [llm-lint](https://github.com/pgy763/llm-lint)（十五条规则，含 SARIF 输出与行内抑制），一条命令在提交前拦住
- 2026-10：给 algo-stage 补了堆排序、并查集、LIS、编辑距离、Trie 五个算法，加上 CI 门禁和 CHANGELOG

**联系**

开 Issue 就行，报错、勘误、想问的都收。

<sub>这儿的仓库是学习记录，不是生产代码 —— 所以每个项目都写了「已知限制」，能跑通和能上线是两件事。</sub>
