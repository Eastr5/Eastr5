# 你好，我是 Eastr5 👋

央财产业经济学硕士在读（数字经济方向，2028 届），本科电子商务。现在做 AI 产品 / 数据产品方向，日常处理的是大模型应用里的问题定义、边界设计和效果验证。

有一段 AI 中台的算法产品经理实习，面向投放团队做多 Agent 辅助系统，也参与过回本模型准度归因和用户标签体系的设计；自己也从 0 到 1 做过 Text2SQL 取数产品和 UGC 商业价值指标体系。写需求文档、定产品边界、设计评测口径的时间比写代码多。SQL / Python / n8n 是常用工具，但我更在意一个功能该不该做、上线后用什么判断它有效。

![AI Product](https://img.shields.io/badge/AI_Product-37474F?style=flat-square)
![Product Spec](https://img.shields.io/badge/Product_Spec-37474F?style=flat-square)
![Agent Workflow](https://img.shields.io/badge/Agent_Workflow-37474F?style=flat-square)
![Text2SQL](https://img.shields.io/badge/Text2SQL-37474F?style=flat-square)
![LLM Evaluation](https://img.shields.io/badge/LLM_Evaluation-37474F?style=flat-square)

## 🛠️ 项目：问题与取舍

| 项目 | 要解决的问题 | 关键取舍 |
| --- | --- | --- |
| **ChatBI**（Text2SQL） | 中小商家做数据分析要依赖专业人员 | 准确率不能只靠 Prompt，所以做了业务元数据字典 + 动态 Few-Shot + AST 校验三层风控，而不是继续调提示词 |
| **UGC 情感挖掘** | 评论里的负面信号发现得太晚 | 把静态分类做成滑动时间窗口的预警，并自研 CPIV / VPV 指标，让结果能直接对应到运营动作 |
| **销售预测与库存预警** | 「断货」和「滞销」同时存在 | 用 WRMSSE 替代通用误差指标，让模型优化方向和财务风险对齐 |

## 💼 实习：AI 中台的算法产品工作

有一段休闲竞技手游公司 AI 中台的算法产品经理实习，面向投放团队做智能诊断与方案创编。下面只写方法层面的判断，不涉及公司内部数据。

- **角色边界**：系统负责生成方案，投手是 Operator 而不是决策者。这个区分决定了交互怎么设计、演示能说到哪一步。
- **两种 Agent 用了两种范式**：诊断是按规则检查，用代码控流程；创编要在多个解法之间路由，交给模型决策。把两者当成同一类 Agent 是常见的返工来源。
- **Prompt 是产品契约**：输入数据契约、输出格式、枚举含义、异常边界、执行前自检，这一层和写 PRD 是同一件事，严谨度直接决定输出质量。领域知识再拆成按场景加载的 Skills，避免把所有规则塞进一条长提示词。
- **系统边界要写进文档**：已完成方案生成与预览，自动下发尚未实现。对外演示不暗示「一键上量」。

另一条线是向数据科学团队提归因分析需求：先给出分层归因框架和参考 SQL，再让对方启动，而不是只丢一个问题过去；也参与过算法侧标签体系与数据团队 CDP 的差异化定位讨论。

## 📦 开源技能仓库

三个给 AI agent 用的技能仓库，和上面的产品工作是两条线：

| 仓库 | 一句话 |
| --- | --- |
| [**academic-tikz**](https://github.com/Eastr5/academic-tikz) | 📐 论文级 TikZ / PGFPlots 绘图技能包，187 个模板全部真实编译过——编译不过的活该被删 |
| [**literature-access-skills**](https://github.com/Eastr5/literature-access-skills) | 📚 文献检索 → 按 DOI 批量下全文 → 进 Zotero，一条链跑通，不人肉搬运 |
| [**skill-router-v3**](https://github.com/Eastr5/skill-router-v3) | 🔀 给 AI coding agent 用的 MCP / Skill / Tool 路由器，跨 Trae / Claude / Cursor / VSCode |

## 🎵 平时

音乐、hiphop。平时也会把几家模型放在同一个任务上对比失败类型，这个习惯后来影响到我设计评测口径。

## 📫 联系

`zhangshawn123@gmail.com` · WeChat: `eastr5`
