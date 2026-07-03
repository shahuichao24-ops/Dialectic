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

**驳真** 是一个从第一性原理出发，通过「解构 → 建模 → 对抗性审查 → 收敛」的循环流程，评估需求、想法或方向的真伪与市场潜力的系统化方法论。

> "没有经过对抗性审查的结论，本质上还是猜测。"

传统的方法论只教你"如何构建"（建模型、画框架），但缺少最关键的一步——**如何摧毁你自己的结论**。Dialectic（驳真）的核心价值不在于"构建框架"，而在于"强制对抗性审查"：假设自己错了，然后证明为什么错。

它不只是一个思维框架，更是一份**可直接在任何 AI 工具中使用**的结构化指令——将 `SKILL.md` 的内容作为 system prompt 或技能指令输入到 Claude Code、Cursor、ChatGPT、GitHub Copilot、DeepSeek 等任何大语言模型工具中，就能获得一致的输出质量。

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
| **① 解构** | 把评估对象分解到不可再分的基本事实和隐藏假设，区分哪些是已知、哪些是推测，标注置信度 | 事实 vs 假设清单（每项有 ✅⚠️❌ 标记） |
| **② 建模** | 构建一个可证伪、可衡量的评估模型。最常用的是三维模型：痛苦(Pain) × 频率(Frequency) × 替代方案不满意(Dissatisfaction)。每个维度必须能被事实推翻 | 带维度的评估框架，每项标注基于"事实"还是"假设" |
| **③ 对抗性审查** | 强制切换立场，从辩护者变成攻击者。≥5 个独立攻击点，覆盖 ≥3 种证据类型（🔬经验/⚙️机制/🎯战略/⚖️伦理/💡启发）。Dissent Quota 强制切换正反立场。每轮通过 Novelty Gate 检验后才结束循环。最后运行 Pre-Mortem（事前验尸） | 漏洞清单 + 最致命问题标记 + 已关闭议题清单 |
| **④ 收敛** | 基于审查结果修正模型，输出带不确定性标记的最终结论。包含少数派报告（"如果这个结论是错的，最可能的原因是什么"） | 最终判定（结论 + 不确定度 + 翻盘条件 + 少数派报告 + 后续建议） |

### 关键机制详解

| 机制 | 来源 | 作用 |
|------|------|------|
| **Evidence Label**（证据标签）🔬⚙️🎯⚖️💡 | Council of High Intelligence | 每个攻击点标注所属的证据类型，确保从多角度审视，防止视角单一化 |
| **Dissent Quota**（异议配额） | Council of High Intelligence | 如果前几个攻击点全部指向同一方向，强制切换正反立场，保证正反两面都被充分审视 |
| **Hemlock Rule**（毒芹规则） | Council of High Intelligence | 已充分讨论并纳入模型修正的攻击点标记为"已关闭"，后续循环不得再攻击同一处（除非出现全新证据） |
| **Novelty Gate**（新颖性门控） | Council of High Intelligence | 每轮审查结束必须检查：本轮是否发现了之前不存在的新攻击点？如果没有，说明审查已收敛，可以结束循环 |
| **Pre-Mortem**（事前验尸） | Council of High Intelligence | 假设基于当前结论去执行了，12 个月后灾难性地失败了，列出最可能的三个失败原因。挖出"低频但高影响"的风险 |
| **Minority Report**（少数派报告） | Council of High Intelligence | 即使在输出最终结论后，也必须记录"如果这个结论是错的，最可能的原因是什么"，防止过度收敛成单一信条 |

---

## 作为 Skill 使用 (Usage as a Skill)

Dialectic 的核心指令全部封装在 `SKILL.md` 中。**它不依赖任何特定平台**，只要 AI 工具支持自定义指令/提示词，就可以使用。

### 在 ZCode 中使用

```bash
# 用户级安装
git clone https://github.com/shahuichao24-ops/Dialectic.git ~/.agents/skills/Dialectic

# 然后通过自然语言触发：
# "帮我用驳真评估一下XXX"
# 或直接调用 /Dialectic
```

### 在其他 AI 工具中使用

将 `SKILL.md` 的完整内容作为 system prompt 或自定义指令输入到以下工具中即可获得一致的输出质量：

- **Claude Code** — 复制 `SKILL.md` 内容到 `.claude/instructions/` 或通过 `-p` 参数传入
- **Cursor** — 复制到 `.cursor/rules/` 或作为 Custom Instructions
- **ChatGPT / DeepSeek / Kimi** — 在对话开始时粘贴 `SKILL.md` 内容作为指令
- **GitHub Copilot CLI** — 通过自定义指令配置
- **任何支持 System Prompt 的 AI 工具** — 直接将 `SKILL.md` 内容设为 system prompt

使用示例对话：

> **你**：帮我评估一下"做一个 AI 生成周报的工具"的需求真伪
>
> **AI（加载了 Dialectic 指令后）** 会按流程输出：
> 1. 解构 → 列出事实（周报是制度性要求）和假设（用户对现状不满）
> 2. 建模 → 三维评估：痛苦(2) × 频率(1) × 替代方案不满意(2) = 4/1000
> 3. 对抗性审查 → 5 个攻击点覆盖 4 种证据类型：AI 不能替代"工作梳理"、频率致命（每周 1 次）、付费动机薄弱、巨头已占位、周报形式在衰落
> 4. 收敛 → **结论：伪需求**。最致命问题：每周 1 次的频率无法支撑独立产品存活

---

## 灵感来源 (Inspirations)

- **第一性原理思维** — Elon Musk、Aristotle
- **对抗性审查（Adversarial Review）** — 法律交叉审问、科学同行评议
- **[Council of High Intelligence](https://github.com/0xNyk/council-of-high-intelligence)** — 多智能体审议框架（Dissent Quota、Hemlock Rule、Novelty Gate、Pre-Mortem）
- **[Superpowers](https://github.com/obra/superpowers)** — AI 辅助开发中的结构化工作流体系

---

## License

MIT © 2026 shahuichao

---

<div id="about"></div>

## About (中文版见上方 ↑)

Dialectic is a systematic methodology for evaluating need authenticity and market potential from first principles. It follows a four-phase loop: **Deconstruct → Model → Adversarial Review → Converge**.

> "A conclusion that hasn't survived adversarial review is still just a guess."

Most methodologies teach you *how to build* — construct models, draw frameworks. They miss the most critical step: **how to tear down your own conclusions**. Dialectic's core value isn't the framework itself — it's the *mandatory adversarial review*: assume you're wrong, then prove why.

Dialectic is platform-agnostic. The complete methodology is encapsulated in `SKILL.md`, which can be used as a system prompt or custom instruction in **any AI tool** — Claude Code, Cursor, ChatGPT, GitHub Copilot, DeepSeek, Kimi, or any other LLM-based assistant. No plugin or framework required.

### Use Cases

| Scenario | Description |
|----------|-------------|
| Evaluate a new product idea | Is this need real? Do users actually need it? |
| Judge need authenticity | Is the pain point sharp enough? What are users doing today? |
| Validate a business direction | Is this worth time and resources? |
| Reverse-audit a decision | What hidden fatal flaws does your current decision have? |
| Diagnose product issues | Why did users download but not return? |

### The Four Phases

| Phase | What you do | Output |
|-------|-------------|--------|
| **① Deconstruct** | Break down to irreducible facts vs. hidden assumptions. Mark confidence levels | Facts vs. assumptions inventory (✅⚠️❌) |
| **② Model** | Build a falsifiable evaluation model. Classic: Pain × Frequency × Dissatisfaction. Every dimension must be provably wrong | Dimensioned framework labeled "fact" or "assumption" |
| **③ Adversarial Review** | Switch from advocate to attacker. ≥5 independent attacks covering ≥3 evidence types (🔬Empirical/⚙️Mechanistic/🎯Strategic/⚖️Ethical/💡Heuristic). Dissent Quota forces perspective switching. Novelty Gate validates each loop. Pre-Mortem exercises simulate failure | Vulnerability map + most critical flaw identified |
| **④ Converge** | Revise model based on findings. Output conclusion with uncertainty markers + minority report ("If this conclusion is wrong, the most likely reason is…") | Final verdict (conclusion + uncertainty + falsification condition + minority report + recommendation) |

### Key Mechanisms

| Mechanism | Source | Purpose |
|-----------|--------|---------|
| **Evidence Label** 🔬⚙️🎯⚖️💡 | Council of High Intelligence | Tag each attack with its evidence type. Ensures multi-perspective review |
| **Dissent Quota** | Council of High Intelligence | If first N attacks all point the same way, force a switch to the opposite stance |
| **Hemlock Rule** | Council of High Intelligence | Mark fully-addressed points as closed. No re-attacking without new evidence |
| **Novelty Gate** | Council of High Intelligence | Each loop must uncover at least one new angle not seen before. If not, convergence is reached |
| **Pre-Mortem** | Council of High Intelligence | "Fast-forward 12 months — we failed catastrophically. What are the three most likely reasons?" |
| **Minority Report** | Council of High Intelligence | Even in the final verdict, document "If this conclusion is wrong, here's why" — prevents over-convergence |

### How to Use as a Skill

Dialectic works in **any AI tool**. No platform lock-in.

**Copy the full content of `SKILL.md`** as a system prompt or custom instruction into:

- **Claude Code** → `.claude/instructions/` or `-p` flag
- **Cursor** → `.cursor/rules/` or Custom Instructions
- **ChatGPT / DeepSeek / Kimi** → paste at the start of conversation
- **GitHub Copilot CLI** → custom instruction config
- **Any AI tool with custom prompts** → set `SKILL.md` content as system prompt

**Example interaction:**

> **You**: "Use Dialectic to evaluate whether an AI weekly-report generator is a real need."
>
> **AI** (with Dialectic loaded):
> 1. **Deconstruct** → facts (reports are mandatory at many companies) vs. assumptions (users are dissatisfied)
> 2. **Model** → Pain(2) × Frequency(1) × Dissatisfaction(2) = 4/1000
> 3. **Adversarial Review** → 5 attacks across 4 evidence types: AI can't replace "work review" itself, fatal frequency (once/week), no willingness to pay, incumbents already there, the weekly report format itself is dying
> 4. **Converge** → **Conclusion: weak/false need**. Fatal flaw: once-a-week frequency can't sustain an independent product

### Inspirations

- **First Principles Thinking** — Elon Musk, Aristotle
- **Adversarial Review** — legal cross-examination, scientific peer review
- **[Council of High Intelligence](https://github.com/0xNyk/council-of-high-intelligence)** — Multi-agent deliberation framework (Dissent Quota, Hemlock Rule, Novelty Gate, Pre-Mortem)
- **[Superpowers](https://github.com/obra/superpowers)** — Structured workflows for AI-assisted development

### License

MIT © 2026 shahuichao
