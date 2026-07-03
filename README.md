<p align="center">
  <h1 align="center">Dialectic（驳真）</h1>
  <p align="center">
    从第一性原理出发评估需求真伪与市场潜力的系统化方法论
    <br/>
    A systematic methodology for evaluating need authenticity and market potential from first principles
  </p>
  <p align="center">
    <a href="#关于本项目-about">中文</a> ·
    <a href="#about">English</a>
  </p>
</p>

---

## 关于本项目 (About)

[English version below ↓](#about)

**驳真** = 从第一性原理出发，通过「解构 → 建模 → 对抗性审查 → 收敛」的循环流程，评估一个需求、想法或方向的真伪与市场潜力。

> "没有经过对抗性审查的结论，本质上还是猜测。"

传统方法论只教你"如何构建"（建模型、画框架），但缺少最关键的一步——**如何摧毁你自己的结论**。驳真（Dialectic）的核心价值不在于"构建框架"，而在于"强制对抗性审查"：假设自己错了，然后证明为什么错。

这不仅仅是一套思维框架，也是一个可在 ZCode 中直接调用的 AI Skill。

---

## 适用场景 (Use Cases)

| 场景 | 说明 |
|------|------|
| 评估新产品想法 | 这个需求是真实的吗？用户真的需要吗？ |
| 判断需求真伪 | 这个痛点够痛吗？用户现在的替代方案是什么？ |
| 验证商业方向 | 这个方向值得投入时间和资源吗？ |
| 逆向审查决策 | 已有的决策有没有隐藏的致命漏洞？ |
| 分析产品问题 | 为什么用户下载了却不用？哪里出了问题？ |

---

## 核心流程 (Process)

```
① 解构 (Deconstruct) → ② 建模 (Model) → ③ 对抗性审查 (Adversarial Review) → ④ 收敛 (Converge)
                        ↑________________________________________|（循环 / Loop）
```

| 阶段 | 做什么 | 输出 |
|------|--------|------|
| **① 解构** | 分解到不可再分的基本事实和隐藏假设，标注置信度 | 事实 vs 假设清单 |
| **② 建模** | 构建可证伪的评估模型（如三维模型：痛苦×频率×替代方案不满意） | 带维度的评估框架 |
| **③ 对抗性审查** | ≥5 个独立攻击点，≥3 种证据类型，Dissent Quota（强制切换正反立场），Novelty Gate，Pre-Mortem | 漏洞清单 |
| **④ 收敛** | 修正模型，输出带不确定性的结论 + 少数派报告 | 最终判定 |

### 关键机制 (Key Mechanisms)

| 机制 | 来源 | 作用 |
|------|------|------|
| **Evidence Label**（证据标签）🔬⚙️🎯⚖️💡 | Council of High Intelligence | 攻击点标注类型，保证视角多元化 |
| **Dissent Quota**（异议配额） | Council of High Intelligence | 强制切换正反立场，防止一面倒 |
| **Hemlock Rule**（毒芹规则） | Council of High Intelligence | 已充分讨论的点标记关闭，不得反复攻击 |
| **Novelty Gate**（新颖性门控） | Council of High Intelligence | 每轮必须有新发现，否则结束循环 |
| **Pre-Mortem**（事前验尸） | Council of High Intelligence | 模拟 12 个月后失败，挖出低频高影响风险 |
| **Minority Report**（少数派报告） | Council of High Intelligence | 结论附带"最可能翻盘的原因" |

---

## 安装 (Installation)

### ZCode

```bash
# 用户级安装（推荐 / Recommended）
git clone https://github.com/shahuichao24-ops/Dialectic.git ~/.agents/skills/Dialectic

# 或项目级安装
git clone https://github.com/shahuichao24-ops/Dialectic.git .agents/skills/Dialectic
```

安装后在 ZCode 中通过以下方式触发：
- 自然语言："帮我用驳真评估一下XXX"
- 直接调用：`/Dialectic 帮我评估一个想法`

### 其他 AI 工具

Dialectic 的核心逻辑完全封装在 `SKILL.md` 中，理论上可用于任何支持自定义技能/指令的 AI 工具（Claude Code、Cursor、Codex 等）。参考各平台的 skill/instruction 配置方式导入即可。

---

## 使用示例 (Example)

> **用户**：帮我评估一下"做一个 AI 生成周报的工具"的需求真伪
>
> **Dialectic 输出路径**：
> 1. **解构** → 列出事实（周报是制度性要求）和假设（用户对现状不满）
> 2. **建模** → 三维评估：痛苦(2) × 频率(1) × 替代方案不满意(2) = 4/1000
> 3. **对抗性审查** →
>    - 🔬 AI 不能替代"工作梳理"（周报价值是梳理不是写）
>    - 🎯 频率致命（每周 1 次，留存困难）
>    - 🎯 付费动机薄弱（没人愿意为周报付费）
>    - ⚙️ 巨头已占位（飞书/钉钉/ChatGPT 已做）
>    - 💡 周报形式在衰落（赛道本身在萎缩）
> 4. **收敛** → **结论：伪需求**。最致命问题：每周 1 次的频率无法支撑独立产品存活

---

## 灵感来源 (Inspirations)

- **第一性原理思维** — Elon Musk、Aristotle
- **对抗性审查（Adversarial Review）** — 法律交叉审问、科学同行评议
- **[Council of High Intelligence](https://github.com/0xNyk/council-of-high-intelligence)** — 多智能体审议框架（Dissent Quota、Hemlock Rule、Novelty Gate、Pre-Mortem）
- **[Superpowers](https://github.com/obra/superpowers)** — AI 辅助开发中的结构化工作流

---

## License

MIT © 2026 shahuichao

---

<div id="about"></div>

## About (中文版见上方 ↑)

**Dialectic** is a systematic methodology for evaluating need authenticity and market potential from first principles.

> "A conclusion that hasn't survived adversarial review is still just a guess."

Most methodologies teach you *how to build* — construct models, draw frameworks. Dialectic focuses on what they miss: **how to tear down your own conclusions**. The core value isn't the framework itself — it's the *mandatory adversarial review*: assume you're wrong, then prove why.

Dialectic ships as a ZCode-compatible AI skill, but its logic is tool-agnostic and can be adapted to any AI coding assistant.

### The Four-Phase Loop

1. **Deconstruct** — Break down to irreducible facts vs. hidden assumptions, with confidence markers
2. **Model** — Build a falsifiable evaluation model (e.g., Pain × Frequency × Dissatisfaction)
3. **Adversarial Review** — ≥5 independent attack vectors, ≥3 evidence types, Dissent Quota, Novelty Gate, Pre-Mortem
4. **Converge** — Revise the model, output a conclusion with uncertainty level + minority report

### Quick Start

```bash
# Install for ZCode
git clone https://github.com/shahuichao24-ops/Dialectic.git ~/.agents/skills/Dialectic
```

Then ask your AI assistant: *"Use Dialectic to evaluate whether [your idea] is a real need."*
