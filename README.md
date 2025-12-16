# 📚 Software Engineering Notes & Coursework (COMP201)

![Markdown](https://img.shields.io/badge/format-Markdown-informational)
![Topic](https://img.shields.io/badge/topic-Software%20Engineering-blue)
![Focus](https://img.shields.io/badge/focus-Requirements%20%7C%20Use%20Cases%20%7C%20Process%20%7C%20Testing-success)

> 一份面向课程复习/作业对照的 **软件工程学习笔记合集**：覆盖需求工程、用例分析、软件过程模型、复杂性控制、测试与敏捷术语速查。

---

## ✨ 你能在这里找到什么

- **需求工程（Requirements Engineering）**：需求定义、需求类型、功能/非功能/领域需求、写作规范  
- **用例分析（Use Case Analysis）**：Actor、Use-case、替代流程、`<<include>>` / `<<extend>>`、用例模板  
- **软件过程（Software Process）**：SDLC 阶段、瀑布/演化/敏捷 & Scrum  
- **复杂性与设计原则**：复杂性来源、模块化、封装、低耦合高内聚  
- **测试（Testing）**：黑盒 vs 白盒、规格驱动测试与可追溯性  
- **Scrum 术语速查**：Backlog、Sprint、Daily Scrum、Scrum Master 等

---

## 🗂️ 仓库结构

```text
.
├── 需求.md                       # 需求工程：定义/类型/功能&非功能/写作规范
├── Coursework1.1 and Use Case Analysis.md
│                                # 用例核心概念：Actor、Use-case、include/extend、模板
├── Software Processes.md         # 软件过程模型：瀑布/演化/敏捷
├── T1.md                         # 课程要点 + SDLC + OO/测试等复习题整理
└── T2.md                         # 复杂性/规格vs设计/测试重要性/Scrum 术语等整理
🚀 推荐阅读顺序（按“从需求到交付”）
需求：先明确“系统要做什么”（功能/非功能/领域）

用例：把需求落成可执行的用户任务与流程

过程模型 & SDLC：把工作拆成阶段，明确产出物（artifacts）

设计原则：用封装、低耦合高内聚控制复杂性

测试：用规格作为验收标准，做黑盒/白盒覆盖

🧠 关键概念速查
1) 需求工程三段式（写给谁 → 写多细 → 用来干嘛）
类型	面向对象	典型形式	用途
用户需求	客户/用户	自然语言 + 图表	让客户确认“要什么”
系统需求	客户 ↔ 承包商	结构化文档	合同/验收依据
软件规范	开发人员	更技术化的细节描述	设计与实现的基础

✅ 写需求时建议统一格式；用 shall / should 表达强制与期望；并确保文档自包含（术语表/示例齐全）。

2) 用例图关系：<<include>> vs <<extend>>
关系	含义	判断口诀
<<include>>	总是复用的子功能	“每次都要做”
<<extend>>	特定条件下的可选分支	“有时才会发生”

✅ 推荐用例描述包含：ID、名称、描述、前置条件、事件流、后置条件、包含关系、扩展点、触发器。

3) SDLC（软件生命周期）阶段与产出物
阶段	关键词	常见产出
需求	获取/分析/确认	SRS、用例、用户故事
架构设计	模块/接口/技术栈	架构图、API、ER 图
详细设计	类/算法/数据结构	类图、顺序图、伪代码
实现	编码/评审/单测	可运行代码、单元测试
测试	集成/系统/验收	测试报告、缺陷列表
部署	发布/配置/自动化	部署脚本、上线版本
运维维护	监控/修复/迭代	补丁、升级、运维文档

4) 复杂性从哪来？怎么压下去？
规模上升时，代码之间的“潜在交互”会接近 平方级增长

通过 模块化、封装、作用域与访问控制 降低不必要依赖

用 高内聚、低耦合 让系统更可维护、更易测试

🧪 测试速查：黑盒 vs 白盒
类别	关注点	常见方法
黑盒测试	输入输出/功能规格	等价类、边界值、状态转换、验收测试
白盒测试	代码结构/路径覆盖	语句/分支/条件覆盖、路径测试、静态分析

✅ 实务上：测试用例应从规格/需求出发，建立“需求 ↔ 设计 ↔ 测试”的追踪链。

🧰 工具与术语（快速提醒）
版本控制：SVN（集中式）、Git（分布式，主流）

测试框架：JUnit（Java 单元测试）

开发环境：Eclipse（Java IDE）

Java 关键字：final（变量/方法/类限制）、interface、abstract class

🤝 使用建议
把每个主题当作考点清单：读完一节就尝试用自己的话复述 + 做小例子

写作业时优先保证：清晰、可验证、可追溯（从需求到测试都能对得上）
