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

**驳真** 是一个从第一性原理出发，通过**三段审查漏斗**（市场验证 → 可行性评估 → 设计审查）逐级过滤产品想法的系统化方法论。每一关都遵循「解构 → 建模 → 对抗性审查 → 收敛」的循环流程。

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
前置：选择审查深度（⚡快速扫描 / 📋标准审查 / 🔬深度审查）
  │
  ▼
┌──────────────────────────────────────────┐
│ 第一关：市场验证 Gate                      │
│ ① 解构 → ② 建模 → ③ 对抗性审查 → ④ 收敛  │
│ 输出：真需求 / 弱需求 / 伪需求 / 需要更多数据 │
└──────────────────────────────────────────┘
  │ 通过
  ▼
┌──────────────────────────────────────────┐
│ 第二关：可行性 Gate                        │
│ ① 六维评估 → ② 对抗性审查 → ③ 收敛       │
│ 输出：可行 / 有条件可行 / 不可行            │
└──────────────────────────────────────────┘
  │ 通过
  ▼
┌──────────────────────────────────────────┐
│ 第三关：设计审查 Gate                      │
│ ① 交互分析 → ② 视觉评估 → ③ 审查 → ④ 收敛 │
│ 输出：通过 / 有条件通过 / 需重新设计         │
└──────────────────────────────────────────┘
  │ 通过
  ▼
输出：完整评估报告 → 调用 writing-plans 制定实施计划
任一关卡失败即终止
```

| 阶段 | 做什么 | 输出 |
|------|--------|------|
| **⚡ 前置** | 根据决策的错误成本和可逆性选择审查深度：快速扫描（≥2 攻击点）、标准审查（≥3 攻击点）、深度审查（≥5 攻击点） | 审查模式锁定 + 攻击点/证据类型阈值 |
| **第一关：市场验证** | ① 解构（事实 vs 假设）→ ② 建模（Pain × Frequency × Dissatisfaction，附行为锚点评分）→ ③ 对抗性审查（按深度参数化）→ ④ 收敛（四态结论 + 验证行动计划 + 少数派报告） | 真需求 / 弱需求 / 伪需求 / 需要更多数据 |
| **第二关：可行性** | ① 六维评估（技术/成本/依赖/合规/设施/团队）→ ② 对抗性审查 → ③ Pre-Mortem（技术视角）→ ④ 收敛 | 可行 / 有条件可行 / 不可行 + 阻塞项清单 |
| **第三关：设计审查** | ① 交互层评估（任务流/反馈/错误/一致/触达）→ ② 视觉层评估（层次/品牌/可读/留白）→ ③ 三视角攻击 + 设计 Pre-Mortem → ④ 收敛 | 通过 / 有条件通过 / 需重新设计 + 改进优先级 |

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
> **AI（加载了 Dialectic 指令后）** 会按三段漏斗输出：
> 1. **前置** → 确定审查深度（小功能 → ⚡ 快速扫描）
> 2. **第一关** → 解构 + 建模：Pain(2)×Frequency(1)×Dissatisfaction(2) = 4，弱需求信号
> 3. **对抗性审查** → 5 个攻击点：AI 不能替代"工作梳理"、每周一次的频率无法支撑独立产品、付费动机薄弱、巨头已占位、周报形式在衰落
> 4. **收敛** → **结论：伪需求**。最致命问题：频率致命，每周 1 次无法支撑独立产品存活。🚦 终止，不建议继续

---

## 适用边界 (Scope/Boundaries)

### Dialectic 适合评估的问题

```
✅ "这个需求是真还是伪？"
✅ "这个方向值不值得投入？"
✅ "这个产品为什么没人用？"
✅ "我的论证中有没有漏洞？"
✅ "哪些隐藏假设可能不成立？"
```

### Dialectic 不适合评估的问题

```
❌ 需要实地验证的问题（定价测试、A/B 实验）→ 跑实验，不是跑流程
❌ 依赖非逻辑信息的问题（时机判断、人际信任）→ 需要经验直觉
❌ 审美/品味的判断（设计好不好看）→ 主观判断
❌ 极端时间压力下的紧急决策（服务器宕机了怎么办）→ 需要专家直觉
```

**方法论不能替代实地验证。** 如果一个问题可以通过一个简单实验来回答，永远优先做实验。

---

## v2.0 更新 (What's New in v2.0)

相较于 v1.0 的核心优化：

| 新增 | 说明 |
|------|------|
| **三段审查漏斗** | 市场验证 → 可行性评估 → 设计审查，逐级过滤，任一关卡被驳倒即终止 |
| **审查深度分级** | ⚡快速扫描 / 📋标准审查 / 🔬深度审查，根据错误成本与可逆性自适应选择 |
| **评分行为锚点** | Pain/Frequency/Dissatisfaction 每个分数都有对应行为信号，评分不再凭感觉 |
| **验证行动计划** | 每个 ⚠️❌ 假设附带验证方法，分析不终结于"不知道" |
| **正面信号锚定** | 5 个正面信号防止审查偏负滑向"所有需求都是假的" |
| **🚦 流转指令** | 每关收敛后输出明确下一步，形成「评估 → 计划 → 执行」闭环 |
| **硬编码参数化** | 所有攻击点/证据类型数字与深度表对齐，消除矛盾 |

## 输入质量标准 (Input Quality Gate)

Dialectic 的输出质量直接由输入质量决定。在开始之前检查你的输入是否达标：

| 标准 | 好输入 | 差输入 |
|------|--------|--------|
| **可验证的事实** | "10 个用户，自然流量，使用率不高" | "用户需要一个更好的工具" |
| **问题够具体** | "AI 生成周报的工具需求真伪如何？" | "做一个 AI 工具怎么样？" |
| **愿意接受否定结论** | 心理准备好了 | 只想要支持 |
| **适合逻辑分析** | "用户抱怨的是什么？" | "现在的时机对不对？" |

### 输入质量检查清单

```
□ 我至少有 3 个可验证的事实作为分析的起点
□ 我的问题具体到 10 个字能说清楚
□ 我做好了"可能得到否定结论"的心理准备
□ 这个问题适合用逻辑分析（不是需要实验/直觉/审美判断）
□ 如果我错了，我愿意接受这个结果
```

至少 4/5 通过才能开始。否则先去做前置工作。

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

Dialectic is a systematic methodology that evaluates product ideas through a **three-gate review funnel** (Market Validation → Feasibility → Design Review). Each gate follows the same loop: **Deconstruct → Model → Adversarial Review → Converge**.

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

### The Three Gates

| Gate | What you do | Output |
|------|-------------|--------|
| **⚡ Pre-step** | Choose review depth based on error cost and reversibility: Quick Scan (≥2 attacks), Standard (≥3), Deep (≥5) | Depth mode + attack/evidence thresholds |
| **Gate 1: Market** | ① Deconstruct (facts vs. assumptions) → ② Model (Pain × Frequency × Dissatisfaction with behavioral anchors) → ③ Adversarial Review (parameterized by depth) → ④ Converge (4-state conclusion + verification plan + minority report) | True need / Weak need / False need / Need more data |
| **Gate 2: Feasibility** | ① Six-dimension assessment (tech/cost/dependency/compliance/infra/team) → ② Adversarial Review → ③ Pre-Mortem (tech lens) → ④ Converge | Feasible / Conditionally feasible / Infeasible + blocker list |
| **Gate 3: Design** | ① Interaction review (task flow/feedback/errors/consistency/a11y) → ② Visual review (hierarchy/brand/readability/spacing) → ③ Three-perspective attack + Design Pre-Mortem → ④ Converge | Pass / Conditional pass / Redesign + priority fixes |

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
> 1. **Pre-step** → Choose depth (small feature → ⚡ Quick Scan)
> 2. **Gate 1** → Deconstruct + Model: Pain(2) × Frequency(1) × Dissatisfaction(2) = 4, weak need signal
> 3. **Adversarial Review** → 5 attacks: AI can't replace "work review" itself, fatal frequency (once/week), no willingness to pay, incumbents already there, the format itself is dying
> 4. **Converge** → **Conclusion: false need**. Fatal flaw: once-a-week frequency can't sustain an independent product. 🚦 Terminate.

### Inspirations

- **First Principles Thinking** — Elon Musk, Aristotle
- **Adversarial Review** — legal cross-examination, scientific peer review
- **[Council of High Intelligence](https://github.com/0xNyk/council-of-high-intelligence)** — Multi-agent deliberation framework (Dissent Quota, Hemlock Rule, Novelty Gate, Pre-Mortem)
- **[Superpowers](https://github.com/obra/superpowers)** — Structured workflows for AI-assisted development

### License

MIT © 2026 shahuichao
