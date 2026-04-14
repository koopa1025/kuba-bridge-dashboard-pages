# 📊 Stock Deep Analyst — A股个股深度分析 Skill

> 一个为 [WorkBuddy](https://www.codebuddy.cn/docs/workbuddy/Overview) 打造的 AI Skill，提供标准化的 A 股个股业绩深度分析与投资策略生成能力。

---

## 🎯 能力概览

当你对 AI 说"帮我分析一下 XX 的业绩"，这个 Skill 会自动执行一套**标准化的专业分析流程**，输出包含以下 **10 大板块**的完整投资分析报告：

| # | 板块 | 内容 |
|---|------|------|
| 1 | 📋 业绩核心数据 | 提取公告原文，制作核心指标对比表 |
| 2 | 📈 季度拆解 | 单季度营收/净利趋势，环比分析 |
| 3 | 🎯 超预期分析 | 实际数据 vs 机构一致预期对比 |
| 4 | 💰 估值分析 | PE/PB/PS/PEG + 3种方法交叉验证 |
| 5 | 📉 技术面分析 | 均线/MACD/KDJ/RSI/BOLL/CCI 综合判断 |
| 6 | 💵 资金面分析 | 主力/散户资金流向，机构行为判断 |
| 7 | 🧮 筹码分析 | 获利比例、平均成本、筹码集中度 |
| 8 | 🏦 机构观点 | 最新研报评级与核心逻辑汇总 |
| 9 | ⚠️ 风险矩阵 | 6大风险因子打分评估 |
| 10 | 🎯 投资策略 | 4类投资者分别给出操作建议 + 敏感性分析 |

---

## 📁 文件结构

```
stock-deep-analyst/
├── SKILL.md                        # 核心 Skill 定义（标准化分析 SOP）
├── _skillhub_meta.json             # Skill 元数据
├── README.md                       # 本文件
└── references/
    ├── analysis_templates.md       # 报告模板 + 速查表
    └── valuation_methods.md        # 8种估值方法论详解
```

---

## 🚀 安装方法

### 方式一：手动安装

将本仓库整个目录复制到 WorkBuddy 的 skills 目录：

```bash
# 用户级安装（推荐）
git clone https://github.com/koopa1025/kuba-bridge-dashboard-pages.git ~/.workbuddy/skills/stock-deep-analyst

# 或项目级安装
git clone https://github.com/koopa1025/kuba-bridge-dashboard-pages.git .workbuddy/skills/stock-deep-analyst
```

### 方式二：在 WorkBuddy 中直接导入

在 WorkBuddy 对话中说：
> "帮我安装 GitHub 上的 stock-deep-analyst skill"

---

## 📖 使用方式

安装后，在 WorkBuddy 中对 AI 说以下任何一种：

- "**分析一下沪电股份的业绩预告**"
- "**XX 最新季报出了，帮我深度分析**"
- "**给我出一份 XX 的投资策略报告**"
- "**XX 值不值得买？**"

AI 会自动加载本 Skill，按标准流程采集数据并生成完整报告。

---

## 🔧 前置依赖

- **WorkBuddy**：需要安装 [WorkBuddy](https://www.codebuddy.cn/docs/workbuddy/Overview) IDE 插件
- **westock-data Skill**：本 Skill 依赖 `westock-data` 获取行情、财务、技术指标等原始数据

---

## 📊 支持的分析场景

| 场景 | 触发示例 | 分析侧重 |
|------|---------|---------|
| 业绩预告分析 | "XX发了业绩预告" | 预告增速区间、超预期判断、环比推算 |
| 业绩快报分析 | "XX业绩快报出了" | 全面数据拆解、ROE变动、资产扩张 |
| 年报/季报分析 | "XX年报深度分析" | 毛利率趋势、现金流质量、资产结构 |
| 投资策略 | "XX值不值得买" | 估值合理性、安全边际、建仓策略 |
| 持仓决策 | "我持有XX，该怎么操作" | 技术趋势、资金流向、减仓/加仓节点 |

---

## 🎨 报告示例

报告自动生成为 Markdown 文件，命名格式：`{股票名称}_{分析类型}_{日期}.md`

包含：
- 详细数据表格
- 多种估值方法交叉验证
- 敏感性分析（5种增速假设下的合理股价）
- 4类投资者的差异化操作策略
- 风险评估矩阵
- 关键催化剂与时间节点

---

## ⚠️ 免责声明

本 Skill 生成的分析报告仅供参考，**不构成投资建议**。股市有风险，投资需谨慎。请根据自身风险承受能力独立决策。

---

## 📝 License

MIT License

---

*Made with ⚡ by [WorkBuddy](https://www.codebuddy.cn/docs/workbuddy/Overview)*
