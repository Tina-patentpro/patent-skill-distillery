# patent-skill-distillery

专利 Skill 蒸馏流水线：把本地 / 云端专利知识库（含 TRIZ、审查指南、答复规则等）提炼为**可追溯知识条目**，
经结构化分析与双门准入，产出可直接安装使用的 Agent Skill。

仓库只保留**最终 skill 与使用所需说明**；过程产物、审计往来与内部记录不在本仓库范围内。

## 目录

| 路径 | 说明 |
|---|---|
| `patent-skill-distillery/SKILL.md` | 流水线主 skill（v3.2.11）：六道工序、B 路线七动作、双门准入 |
| `patent-skill-distillery/references/analysis-spec.md` | 知识分析规范（条目结构、标签、证据状态、用途与范围） |
| `patent-skill-distillery/references/sources.md` | 来源口径与四口径重算、八情形覆盖 |
| `drawing-rules/SKILL.md` | 专利附图规则与出图检查（v0.1.6）：任务类型门槛、输入四态、输出分栏、用途准入 |

## 安装

将对应目录复制到你的 Agent 的 skills 目录即可，例如：

```text
<skills 目录>/patent-skill-distillery/
<skills 目录>/drawing-rules/
```

Skill 由 Agent 按触发条件自动加载；无需额外构建或依赖安装。

## 使用要点

1. **输入**：本地知识库目录或 ima 知识库（含订阅库），均为**只读**；受保护原始资料不得改写。
2. **产出**：知识条目（中性句式 + 三标签 + 证据状态）→ 分析 → 候选 skill → 准入通过后安装。
3. **纪律**：法条结论须带来源与核实日期；外部归档只增不改；已安装 skill 无变更单不得修改。

## 版本

- 流水线：`patent-skill-distillery` v3.2.11
- 附图规则：`drawing-rules` v0.1.6

> 本仓库为方法论与工具说明，不构成法律意见；使用请自行核对现行法规与官方文本。
