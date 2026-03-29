# Open Source Deep Dive / 开源项目深度拆解

一个用于 [Claude Code](https://claude.ai/claude-code) 的 Skill，帮助非技术人员（产品经理、创始人、市场负责人）系统性地深度拆解一个开源项目——理解它的产品逻辑、架构设计、竞争格局和商业机会。

## 这是什么？

当你看到一个火爆的开源项目，想搞清楚"它到底怎么做的、为什么能火、有没有创业机会"，但你不是工程师——这个 Skill 就是为你设计的。

它不教你读代码，而是帮你用**产品视角**理解技术系统：从产品定位到架构全景，从核心模块到商业机会，一层层递进。

**核心思路**：先问"为谁解决什么问题"，再看"怎么实现"。从产品约束推导技术方案，不是反过来。每个技术模块都连接到"对做产品/创业有什么用"。

## 五阶段分析框架

| 阶段 | 内容 | 要回答的核心问题 |
|------|------|-----------------|
| 1. 项目扫描 | 快速判断值不值得深入 | 社区健康吗？有什么独特价值？值得花时间吗？ |
| 2. 产品拆解 | 不看代码，纯产品视角 | 它是什么？为谁？为什么火？跟竞品有什么本质区别？ |
| 3. 架构认知 | 建立全局心智模型 | 系统分几层？一条消息/请求怎么走完全流程？ |
| 4. 核心深潜 | 逐模块三层递进 | 架构（有什么）→ 设计决策（为什么）→ 数据流（怎么流动） |
| 5. 商业洞察 | 技术理解转化为商业判断 | 有什么创业机会？风险在哪？什么设计思路可以迁移？ |

## 适用场景

- **产品经理**想深度理解一个开源项目的实现原理和产品设计
- **创始人**想评估一个开源项目的商业机会或技术壁垒
- **市场/投资人**想理解一个技术产品为什么能成功
- **AI 领域从业者**想从优秀开源项目中学习可迁移的架构设计
- 任何非技术人员想"把一个开源仓库学透"

## 核心原则

| # | 原则 | 说明 |
|---|------|------|
| 1 | 先产品后技术 | 先问"为谁解决什么问题"，再看"怎么实现" |
| 2 | 模块选择靠调研 | 全面扫描后按产品价值排序，不是"想到什么学什么" |
| 3 | 端到端流程是锚点 | 走完一条完整用户路径后，每次深潜都知道"我在哪" |
| 4 | 三层递进 | 架构（有什么）→ 设计决策（为什么）→ 数据流（怎么流动） |
| 5 | 从产品约束推导技术 | 不是"用了什么技术"，而是"什么约束导致了这个选择" |
| 6 | 具体例子串全流程 | 抽象概念必须用具体场景落地 |
| 7 | 每个模块都有产出 | 产品启发/创业启发不是附录，是每个模块的核心交付物 |

## 安装

### 方式一：直接复制

将 `SKILL.md` 文件复制到你的 Claude Code skills 目录：

```bash
mkdir -p ~/.claude/skills/opensource-deep-dive
cp SKILL.md ~/.claude/skills/opensource-deep-dive/
```

### 方式二：克隆仓库

```bash
git clone https://github.com/hunterr198/opensource-deep-dive-skill.git ~/.claude/skills/opensource-deep-dive
```

## 使用方法

安装后，在 Claude Code 中直接提出分析需求即可。以下提示方式都会触发此技能：

```
帮我深度分析一下这个开源项目
```

```
我想理解这个仓库的实现原理和商业机会
```

```
用产品视角帮我拆解这个开源项目，看看有什么创业机会
```

```
帮我做一个这个开源项目的 deep dive
```

## 输出示例

分析会产出一份结构化的完整文档，包含：

- **项目扫描结论** — 值不值得深入，为什么
- **产品定位拆解** — 是什么、为谁、为什么火、跟竞品的本质区别
- **架构全景** — 分层图 + 端到端流程图
- **核心模块深潜**（每个模块包含）：
  - 一句话总结
  - 架构地图（组件 + 关系）
  - 核心数据流（端到端图示）
  - 关键设计决策（约束 → 方案 → 取舍）
  - 产品启发（可迁移的思路）
  - 关键术语表
- **商业洞察** — 创业机会 + 风险评估 + 方向选择框架 + 可迁移的设计模式

## 设计原则

- **面向非技术用户**：不需要读代码，用类比和场景解释技术概念
- **产品约束驱动**：不是"它用了什么技术"，而是"什么约束导致了这个选择"
- **对话式探索**：先对话再文档，用户的追问驱动分析深度
- **务实产出导向**：每个模块都连接到"对我做产品/创业有什么用"

## 方法论来源

- [a16z: Open Source From Community to Commercialization](https://a16z.com/open-source-from-community-to-commercialization/) — 开源项目商业化框架
- [Stack Overflow: The Product Approach to Open Source](https://stackoverflow.blog/2023/11/08/the-product-approach-to-open-source-communities/) — 产品思维看开源
- [CHAOSS: Open Source Project Health Metrics](https://chaoss.community/kb/metrics-model-starter-project-health/) — 社区健康度评估
- [GitHub OSPO: Health Metrics](https://github.com/github/github-ospo/blob/main/docs/open-source-health-metrics.md) — GitHub 官方健康指标
- [Linux Foundation: Setting an Open Source Strategy](https://www.linuxfoundation.org/resources/open-source-guides/setting-an-open-source-strategy) — 开源战略制定

## License

MIT
