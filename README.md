# Code Style —— LLM 编码行为准则

> 减少 LLM 编码常见错误的行为准则技能：**避免过度工程、外科手术式改动、显式假设、可验证成功标准**。编写、审查、重构、调试任何代码时自动应用。

这是一个 **AI Agent 技能（Skill）**：它不是语法风格指南，而是约束 Agent 编码**行为**的准则——解决 LLM 写代码最常见的通病：过度设计、越界改动、隐藏假设、无验证标准。

## ✨ 核心特性

- **避免过度工程** —— 不为不存在的需求做架构；最简单可行的方案优先
- **外科手术式改动** —— 只改与目标相关的代码，不做顺手的无关重构
- **显式假设** —— 无法验证的假设明确说出口，不默默押注
- **可验证成功标准** —— 每个改动都有明确的验证方式，不做"应该没问题"的交付
- **自动应用** —— 编写、审查、重构、调试代码时无需用户提醒即生效
- **审慎权衡** —— 偏向谨慎而非速度；琐碎任务由 Agent 自行判断简化

## 🧠 设计思路

本技能与 [Code Magician](https://github.com/yarran-eng/yarran-code-magician) 互补：Code Magician 提供端到端编码纪律（流程层面），Code Style 提供微观行为准则（改动层面）。两者可独立使用，也可叠加使用。

## 📦 安装

```bash
# 将技能目录放入你的 Agent 技能发现目录（如 ~/.agents/skills/）
git clone https://github.com/yarran-eng/yarran-code-style ~/.agents/skills/yarran-code-style
# 或手动将 yarran-code-style 目录复制到技能目录
```

支持任何能加载技能（Skill）的 Agent，包括 ZCode、Claude Code、Codex、Trae 等。

## 🚀 使用方法

| 用户输入示例 | 触发行为 |
|---|---|
| 编写 / 审查 / 重构 / 调试任何代码 | 自动应用行为准则，防止过度设计与越界改动 |

## 📁 目录结构

```
yarran-code-style/
└── SKILL.md        # 技能主文档（完整行为准则）
```

## 🤖 兼容性

技能仅定义行为准则，不依赖特定平台 API，适用于所有支持技能调用机制的 AI Agent。

## 🔗 系列技能

| 技能 | 仓库 |
|---|---|
| Browser Prevention（浏览器隐私防护） | [yarran-browser-prevention](https://github.com/yarran-eng/yarran-browser-prevention) |
| Code Magician（编码纪律） | [yarran-code-magician](https://github.com/yarran-eng/yarran-code-magician) |
| English Chat（中译美式口语） | [yarran-english-chat](https://github.com/yarran-eng/yarran-english-chat) |
| English Learn（口语学习笔记） | [yarran-english-learn](https://github.com/yarran-eng/yarran-english-learn) |
| Find Skill（技能发现编排） | [yarran-find-skill](https://github.com/yarran-eng/yarran-find-skill) |
| Paper Reader（论文深度阅读） | [yarran-paper-reader](https://github.com/yarran-eng/yarran-paper-reader) |
| ROS2 Code（ROS2 编码规范） | [yarran-ros2-code](https://github.com/yarran-eng/yarran-ros2-code) |
| Windows Cleanup（C 盘清理卸载） | [yarran-windows-cleanup](https://github.com/yarran-eng/yarran-windows-cleanup) |

## 📄 许可

MIT License（见仓库 LICENSE 文件）。
