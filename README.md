<p align="center">
  <h1 align="center">🛡️ Dialectic · 驳真</h1>
  <p align="center">
    <b>不只是让你构建结论，而是强迫你摧毁它。</b>
    <br/>
    <sub>从第一性原理出发的产品决策对抗性审查框架（偏见检测系统）— 任何 AI 工具即装即用</sub>
  </p>
  <p align="center">
    <img src="https://img.shields.io/badge/version-2.1-3C3489?style=flat-square" alt="v2.1">
    <img src="https://img.shields.io/badge/license-MIT-1D9E75?style=flat-square" alt="MIT">
    <img src="https://img.shields.io/badge/platform-AI%20agnostic-534AB7?style=flat-square" alt="AI agnostic">
    <img src="https://img.shields.io/badge/lines-824-888780?style=flat-square" alt="824 lines">
  </p>
  <p align="center">
    <a href="#快速上手-quick-start">⚡ 快速上手</a> ·
    <a href="#核心流程">📋 核心流程</a> ·
    <a href="#v21-更新">✨ v2.1</a> ·
    <a href="#about">🇬🇧 English</a>
  </p>
</p>

---

> **大多数方法论教你："先建个框架，然后打分评估。"**
> **Dialectic 教你："假设你是错的，然后证明为什么错。"**
>
> 这是两者之间最本质的差距。没有经过对抗性审查的结论，本质上还是猜测。
> 而通过了对抗性审查的需求，也不等于值得做——它只是**还没被证伪**。

---

## 🎯 这解决了什么问题？

| 😵 没有 Dialectic | 🧠 有 Dialectic |
|-------------------|-----------------|
| "我觉得这个需求很真" | Pain(3)×Frequency(2)×Dissatisfaction(1)=**6，伪需求** |
| "竞品没人做=蓝海机会" | "更可能是：没人找到可行的方案" |
| "用户说想要这个功能" | "用户'感兴趣'≠用户'需要'。兴趣免费，需要付费" |
| "只要体验好10%，用户就会来" | "需要 10 倍体验提升才值得改变习惯" |
| 产品做了半年才发现没市场 | 30 分钟内识别 5 个致命攻击点，省下 6 个月 |

---

## ⚡ 快速上手 (Quick Start)

<details open>
<summary><b>👇 点击展开 — 看 Dialectic 如何在 2 分钟内打穿一个需求</b></summary>
<br/>

> **输入**：帮我评估 "做一个 AI 自动生成周报的工具" 的需求真伪

<blockquote>

**⚡ 前置**：三问速筛 → 三问全过则直接决策；任一"建议走"则进入完整流程。小功能、可逆 → 选快速扫描（2 个攻击点即可）

**第一关 · 需求信号检测**

| 步骤 | 内容 |
|------|------|
| ① 解构 | ✅ 周报是制度性要求 | ⚠️ 用户对写周报感到痛苦？ | ❌ 用户愿意为解决方案付费 |
| ② 建模 | Pain(2) × Frequency(1) × Dissatisfaction(2) = **4 → 伪需求信号** |
| ③ 审查 | 🔬 AI 不能替代"梳理工作"这步 | 💡 每周 1 次的频率无法支撑产品存活 | 🎯 ChatGPT 输入框就能做 |
| ④ 收敛 | **结论：伪需求** ⏸ 搁置 | 最致命：频率致命 | 复活条件：除非"企业强制要求用 AI 工具写周报"且可观测，否则不继续 |

**🚦 搁置（附复活条件）。不建议当前投入，但留好重新评估的触发器。**

</blockquote>

> **30 分钟 vs 6 个月** — 正确的问题不需要正确答案，需要正确的问题被及时否决（或在时机未到时被妥善搁置）。
</details>

---

## 📋 核心流程

```
         ⚡ 前置：三问速筛（默认入口，3 分钟）
        （三问全过 → 直接决策 / 任一"建议走" → 进完整流程）
                    │
                    ▼
         ⚡ 前置：选择审查深度
        （快速扫描 / 标准审查 / 深度审查）
                    │
     ┌──────────────┼──────────────┐
     ▼              ▼              ▼
  ┌──────┐      ┌──────┐      ┌──────┐
  │ ≥2   │      │ ≥3   │      │ ≥5   │  ← 攻击点数
  │ 攻击  │      │ 攻击  │      │ 攻击  │
  └──────┘      └──────┘      └──────┘
                    │
                    ▼
     ┌─────────────────────────────┐
     │  🔍 第一关：需求信号检测       │
     │  是真需求还是自己骗自己？       │
     │  ① 解构 → ② 建模 → ③ 审查 → ④ 收敛 │
     │  → 真需求 / 弱需求 / 伪需求 / 需要更多数据 │
     └─────────────┬───────────────┘
                   │ 信号足够 ✅
                   ▼
     ┌─────────────────────────────┐
     │  🛠️ 第二关：实现条件扫描       │
     │  能做吗？值得做吗？有什么坑？    │
     │  ① 六维评估 → ② 审查 → ③ 收敛  │
     │  → 可行 / 有条件可行 / 不可行   │
     └─────────────┬───────────────┘
                   │ 条件满足 ✅
                   ▼
     ┌─────────────────────────────┐
     │  🎨 第三关：体验一致性校验      │
     │  交互顺吗？视觉对吗？           │
     │  ① 交互 → ② 视觉 → ③ 审查 → ④ 收敛 │
     │  → 通过 / 有条件通过 / 需重新设计  │
     └─────────────┬───────────────┘
                   │ 通过 ✅
                   ▼
              ✅ 输出评估报告
         → 调用 writing-plans 制定计划
```

### 三道关卡速查

| 关卡 | 回答什么问题 | 信号不足后果 |
|------|------------|-----------|
| 🔍 **需求信号检测** | 有人真的需要这个吗？ | ⏸ 搁置（附复活条件）。信号弱不意味着永远不做 |
| 🛠️ **实现条件扫描** | 技术上能实现吗？成本可控吗？ | ⏸ 搁置（附复活条件）。条件不成熟 |
| 🎨 **体验一致性校验** | 交互和视觉是否匹配产品定位？ | ⚠️ 修复后重新审查 |

> 💡 **任一关卡信号不足 → 输出「搁置 + 复活条件」（可观测触发器 + 复核日期），而非一票否决。** 好创意常因"时机未到"被搁置，而非"被证伪"。

---

## 🧬 6 个关键机制

| 机制 | 一句话解释 |
|------|-----------|
| 🔬⚙️🎯⚖️💡 **Evidence Label** | 每个攻击点标注证据类型，防止只会从一个角度看问题 |
| ⚖️ **Dissent Quota** | 如果前几个攻击点全在否定 → 强制切换到辩护方立场，反之亦然 |
| 🔒 **Hemlock Rule** | 已关闭的议题不许重提，每次审查必须挖"新伤口" |
| 🆕 **Novelty Gate** | 本轮审查发现了新角度吗？没有→审查已收敛，该结束了 |
| 💀 **Pre-Mortem** | 假设 12 个月后惨败，最可能的 3 个死因是什么？ |
| 📝 **Minority Report** | 即使结论确认，也记录"如果错了，最可能是因为……" |

> **v2.1 新增机制**：🛡️ **META-GATE**（承认框架自身也可废止）+ ⚡ **三问速筛**（默认轻量入口）+ ⏸ **复活条件**（搁置而非终止）+ 🟢 **正面信号内嵌 HARD-GATE**（≥3 信号强制攻击点 +1）

---

## 🔧 在任何 AI 工具中使用

Dialectic 是一份 **824 行的纯文本指令文件** (`SKILL.md`)，不依赖任何框架或平台。

### 一行命令安装

```bash
# 克隆到技能目录
git clone https://github.com/shahuichao24-ops/Dialectic-skill.git ~/.agents/skills/Dialectic

# 然后直接说中文即可：
# "帮我用驳真评估一下XXX"
```

### 其他 AI 工具

| 工具 | 使用方式 |
|------|---------|
| **Claude Code** | 复制到 `.claude/instructions/` |
| **Cursor** | 复制到 `.cursor/rules/` |
| **ChatGPT / DeepSeek / Kimi** | 对话开头粘贴 `SKILL.md` 全文 |
| **GitHub Copilot** | 自定义指令配置 |
| **任意 AI 工具** | 将 `SKILL.md` 作为 system prompt 注入 |

<details>
<summary><b>📋 使用场景清单</b></summary>

| 场景 | 触发语 |
|------|--------|
| 评估新产品想法 | "帮我用驳真评估一下 [XXX]" |
| 判断需求真伪 | "你觉得 [XXX] 这个需求是真还是假？" |
| 验证商业方向 | "帮我想想 [XXX] 要不要做" |
| 逆向审查决策 | "帮我审查一下 [XXX] 方案有没有漏洞" |
| 分析产品问题 | "为什么 [XXX] 下载了但没人用？" |
</details>

---

## ✨ v2.0 更新

```
v1.0 (593 行) ──────────────→ v2.0 (800 行, +35%)
 单一循环                            三段漏斗
 固定 5 攻击点                        ⚡2 / 📋3 / 🔬5 自适应
 纯文字流程                           Mermaid 可视化
 评分凭感觉                          行为锚点校准
 假设止于"不知道"                      验证行动计划
 只破不立                             正面信号平衡
```

| 新增 | 解决什么问题 |
|------|------------|
| **三段审查漏斗** | 逐级过滤，不在错误阶段浪费精力 — 市场没通过就不谈可行性 |
| **审查深度分级** | 小决定不用硬凑 5 个攻击点，大决定不会止于 2 个 |
| **评分行为锚点** | "Pain=6" 必须有行为证据，不再凭直觉打分 |
| **🚦 流转指令** | 每关输出明确的"下一步"，不让人猜 |
| **验证行动计划** | 每个 ⚠️❌ 假设都匹配验证方法、成本和预期时间 |
| **正面信号锚定** | 防止审查滑向"所有需求都是假的"的偏见 |
| **设计 Pre-Mortem** | 第三关补齐 — "如果因为设计问题流失用户，最可能的三个原因？" |
| **技能联动** | 设计审查可调用 ui-ux-pro-max，评估完成衔接 writing-plans |

---

## ✨ v2.1 更新

```
v2.0 (800 行) ──────────────→ v2.1 (824 行)
三段审查漏斗                      偏见检测系统（重新定位）
终止即关闭通道                    搁置 + 复活条件
推翻权限宽松（1 理由可跳过）        证据 + 期限重审（临时可收回）
无轻量入口                        三问速筛默认入口
正面信号只是建议                  正面信号内嵌 HARD-GATE（≥3 则攻击点 +1，强制）
```

| 改动 | 为什么 |
|------|--------|
| **重新定位：偏见检测系统** | 元评估发现原"判定框架"定位导致自指悖论——要求一切结论经过审查，却无法审查自身。改为"暴露盲区、对抗确认偏误"的检测系统，悖论自消解 |
| **META-GATE 元声明** | 开头声明"驳真也可能错、本身在迭代"，并给出可废止的推翻权限（需具体证据 + 期限），防止框架沦为僵化教条或逃避审查的后门 |
| **搁置替代终止** | 每个负面结论不再"判死刑"，而是输出「可观测触发器 + 复核日期」的复活条件——好创意因时机未到而被搁置，而非被证伪 |
| **三问速筛（默认入口）** | 800 行门槛太高。3 个问题 3 分钟判断值不值得走完整流程，降低使用门槛；并修正了"有人反对→跳过"的逻辑错误（应为"必须走"） |
| **正面信号内嵌 HARD-GATE** | ≥3 信号时攻击点 +1（强制规则），并新增第 6 条带硬标准（可量化 = 有历史/可观测基线），对抗"过度驳回" |
| **核心原则 13→16** | 新增可废止性、不输出停止、三问优先；修正"对抗性审查只能揭示假、不能证明真" |

---

## 🧪 输入质量门控

> ⚠️ 垃圾进 → 垃圾出。不管你用了什么方法论。

| 标准 | ✅ 好输入 | ❌ 差输入 |
|------|----------|----------|
| 有可验证的事实 | "10 个用户，自然流量，使用率不高" | "用户需要一个更好的工具" |
| 问题够具体 | "AI 生成周报的需求真伪？" | "做个 AI 工具怎么样？" |
| 愿意接受否定结论 | 心理准备好了 | 只想找人背书 |
| 适合逻辑分析 | "用户抱怨什么？" | "现在时机对不对？" |

```
□ 我至少有 3 个可验证的事实
□ 我的问题 10 个字能说清楚  
□ 我接受"可能得到否定结论"
□ 这个问题适合逻辑分析（不是实验/直觉/审美）
□ 如果我错了，我认

→ 至少 4/5 通过才能开始 ←
```

---

## 🙏 灵感来源

- **第一性原理** — Aristotle, Elon Musk
- **对抗性审查** — 法律交叉审问、科学同行评议
- **[Council of High Intelligence](https://github.com/0xNyk/council-of-high-intelligence)** — 多智能体审议框架
- **[Superpowers](https://github.com/obra/superpowers)** — AI 辅助开发结构化工作流

---

## 📄 License

MIT © 2026 [shahuichao](https://github.com/shahuichao24-ops)

---

<div id="about"></div>

## 🇬🇧 About

> **Most methodologies teach you: "Build a framework, then score it."**
> **Dialectic teaches you: "Assume you're wrong, then prove why."**
>
> That's the fundamental gap. A conclusion that hasn't survived adversarial review is still just a guess.
> And a need that survived adversarial review isn't proven real — it's merely **not yet falsified**.

---

### 🎯 What Problem Does This Solve?

| 😵 Without Dialectic | 🧠 With Dialectic |
|----------------------|-------------------|
| "I feel this is a real need" | Pain(3)×Freq(2)×Dissatisfaction(1)=**6, false need** |
| "No competitors = blue ocean" | "More likely: nobody found a viable approach" |
| "Users said they want this" | "Interest ≠ Need. Interest is free; need pays" |
| "A 10% better UX will win" | "Users need 10× improvement to switch habits" |
| 6 months wasted on wrong idea | 30 min, 5 fatal attacks identified, 6 months saved |

---

### ⚡ Quick Try

<details open>
<summary><b>👇 Click to expand — see Dialectic destroy a bad idea in 2 minutes</b></summary>
<br/>

> **Input**: "Evaluate whether an AI weekly-report generator is a real need"

<blockquote>

**⚡ Pre-step**: Three-Question Screen → all pass = decide now; any "recommend full" = run full flow. Small idea, reversible → Quick Scan (≥2 attacks)

**Gate 1 · Need Signal Detection**

| Step | Finding |
|------|---------|
| ① Deconstruct | ✅ Reports are mandatory | ⚠️ Users hate writing them? | ❌ Users will pay? |
| ② Model | Pain(2) × Frequency(1) × Dissatisfaction(2) = **4 → false need signal** |
| ③ Review | 🔬 AI can't replace "work reflection" | 💡 Once/week can't sustain a product | 🎯 ChatGPT already does this |
| ④ Converge | **Verdict: false need** ⏸ Hold | Fatal: frequency kills it | Revival: unless "companies mandate AI tools" + observable, don't proceed |

**🚦 Hold (with revival conditions). Don't invest now, but keep the trigger for re-evaluation.**

</blockquote>

> **30 minutes vs 6 months** — The right question doesn't need the right answer. It needs to be killed quickly if it's wrong (or held properly if the timing is off).
</details>

---

### 📋 Core Process

```
         ⚡ Pre-step: Three-Question Screen (default entry, 3 min)
        (all pass → decide now / any "recommend full" → run full flow)
                    │
                    ▼
         ⚡ Pre-step: Choose review depth
        (Quick Scan / Standard / Deep)
                    │
     ┌──────────────┼──────────────┐
     ▼              ▼              ▼
  ┌──────┐      ┌──────┐      ┌──────┐
  │ ≥2   │      │ ≥3   │      │ ≥5   │  ← attacks
  │attacks│     │attacks│     │attacks│
  └──────┘      └──────┘      └──────┘
                    │
                    ▼
     ┌─────────────────────────────┐
     │  🔍 Gate 1: Need Signal       │
     │  Is this a real need?        │
     │  ① Deconstruct → ② Model → ③ Review → ④ Converge │
     │  → True / Weak / False / Need more data            │
     └─────────────┬───────────────┘
                   │ Signal strong enough ✅
                   ▼
     ┌─────────────────────────────┐
     │  🛠️ Gate 2: Feasibility      │
     │  Can we build it? Worth it?  │
     │  ① 6-Dim Assessment → ② Review → ③ Converge │
     │  → Feasible / Conditional / Infeasible       │
     └─────────────┬───────────────┘
                   │ Conditions met ✅
                   ▼
     ┌─────────────────────────────┐
     │  🎨 Gate 3: Design Review    │
     │  Does UX match the product?  │
     │  ① Interaction → ② Visual → ③ Review → ④ Converge │
     │  → Pass / Conditional / Redesign                  │
     └─────────────┬───────────────┘
                   │ Pass ✅
                   ▼
              ✅ Final report
         → Invoke writing-plans for implementation
```

#### Gate Quick Reference

| Gate | Answers | If Signal Weak |
|------|---------|-----------|
| 🔍 **Need Signal** | Does anyone actually need this? | ⏸ Hold (+ revival conditions). Weak ≠ never |
| 🛠️ **Feasibility** | Can we build it? Cost? Risk? | ⏸ Hold (+ revival conditions). Conditions not ripe |
| 🎨 **Design** | Does UX match product positioning? | ⚠️ Fix and re-review |

> 💡 **Any gate with weak signal → output "Hold + revival conditions" (observable trigger + review date), not a veto.** Good ideas are often held for "bad timing", not "proven false".

---

### 🧬 6 Key Mechanisms

| Mechanism | One-liner |
|-----------|-----------|
| 🔬⚙️🎯⚖️💡 **Evidence Label** | Tag each attack with evidence type — prevents single-perspective blindness |
| ⚖️ **Dissent Quota** | After N attacks all pointing one way → force-switch to the opposite stance |
| 🔒 **Hemlock Rule** | Closed issues stay closed. Every review loop must find *new* wounds |
| 🆕 **Novelty Gate** | Did this loop uncover a new angle? No → converged, stop looping |
| 💀 **Pre-Mortem** | Fast-forward 12 months — we failed catastrophically. Top 3 causes? |
| 📝 **Minority Report** | Even in the final verdict: "If this is wrong, the most likely reason is…" |

> **v2.1 new**: 🛡️ **META-GATE** (the framework itself is falsifiable) + ⚡ **Three-Question Screen** (default light entry) + ⏸ **Revival Conditions** (hold, not terminate) + 🟢 **Positive Signals in HARD-GATE** (≥3 → attacks +1, forced)

---

### 🔧 Use with Any AI Tool

Dialectic is an **824-line plain-text instruction file** (`SKILL.md`). Platform-agnostic. No dependencies.

```bash
# One-line install
git clone https://github.com/shahuichao24-ops/Dialectic-skill.git ~/.agents/skills/Dialectic

# Then say in natural language:
# "Use Dialectic to evaluate [XXX]"
```

| Tool | How to Use |
|------|-----------|
| **Claude Code** | Copy to `.claude/instructions/` |
| **Cursor** | Copy to `.cursor/rules/` |
| **ChatGPT / DeepSeek / Kimi** | Paste `SKILL.md` at conversation start |
| **GitHub Copilot** | Custom instruction config |
| **Any AI tool** | Inject `SKILL.md` as system prompt |

<details>
<summary><b>📋 Trigger phrases</b></summary>

| Scenario | Trigger |
|----------|---------|
| Evaluate a new idea | "Use Dialectic to evaluate [XXX]" |
| Judge need authenticity | "Is [XXX] a real need or not?" |
| Validate a direction | "Should I pursue [XXX]?" |
| Reverse-audit a decision | "Review my [XXX] plan for flaws" |
| Diagnose product issues | "Why is [XXX] downloaded but not used?" |
</details>

---

### ✨ v2.0 Highlights

```
v1.0 (593 lines) ──────────→ v2.0 (800 lines, +35%)
 Single loop                       Three-gate funnel
 Fixed ≥5 attacks                  ⚡2 / 📋3 / 🔬5 adaptive
 Plain-text flow                   Mermaid visualization
 Gut-feel scoring                  Behavioral anchors
 Assumptions left "unknown"        Verification action plans
 Tear-down only                    Positive signal counterbalance
```

| Addition | Problem Solved |
|----------|---------------|
| **Three-gate funnel** | Filter progressively — don't discuss feasibility when market is dubious |
| **Depth levels** | Small decisions don't need 5 attacks; big ones won't stop at 2 |
| **Behavioral anchors** | "Pain=6" must cite evidence, not intuition |
| **🚦 Routing instructions** | Every gate outputs a clear "next step" |
| **Verification action plan** | Every ⚠️❌ assumption gets a verification method + cost + timeline |
| **Positive signals** | Counterbalances the natural skew toward "everything is false" |
| **Design Pre-Mortem** | Gate 3: "If users churn due to UX, the top 3 reasons are…" |
| **Skill chaining** | Design gate links to ui-ux-pro-max; completion links to writing-plans |

---

### ✨ v2.1 Highlights

```
v2.0 (800 lines) ──────────→ v2.1 (824 lines)
 Three-gate funnel                  Bias-detection system (repositioned)
 Terminate = close channel          Hold + revival conditions
 Loose override (1 reason)          Evidence + time-boxed override
 No light entry                     Three-Question Screen (default)
 Positive signals = suggestion      Positive signals in HARD-GATE (≥3 → +1, forced)
```

| Change | Why |
|--------|-----|
| **Reposition: bias-detection system** | Meta-review found the "judge framework" framing caused a self-reference paradox — it demanded all conclusions be reviewed yet couldn't review itself. Reframed as "expose blind spots, fight confirmation bias" — paradox dissolves |
| **META-GATE declaration** | Opens by stating "Dialectic can be wrong, is itself iterating", with a falsifiable override (needs concrete evidence + time-box) — prevents dogma or an escape hatch |
| **Hold instead of Terminate** | Negative verdicts no longer "execute" — they output revival conditions (observable trigger + review date). Good ideas are held for timing, not proven false |
| **Three-Question Screen (default)** | 800 lines is a high bar. 3 questions in 3 min decide whether the full flow is worth it; also fixes the "opposition → skip" logic bug (should be "must run") |
| **Positive signals in HARD-GATE** | ≥3 signals → attacks +1 (forced rule); adds signal #6 with a hard standard (quantifiable = has historical/observable baseline) to fight "over-rejection" |
| **Core principles 13→16** | Adds falsifiability, "don't output stop", three-question-first; corrects "adversarial review reveals false, doesn't prove true" |

---

### 🧪 Input Quality Gate

> ⚠️ Garbage in → garbage out. Methodology can't save bad inputs.

| Standard | ✅ Good Input | ❌ Bad Input |
|----------|--------------|--------------|
| Verifiable facts | "10 users, organic, low usage" | "Users need a better tool" |
| Specific problem | "Is AI weekly-report a real need?" | "How about an AI tool?" |
| Open to negative results | Mentally prepared | Just looking for validation |
| Suits logical analysis | "What are users complaining about?" | "Is this the right timing?" |

```
□ I have ≥3 verifiable facts
□ I can state the problem in 10 words
□ I accept "possibly a false need"
□ This suits logical analysis (not experiment/intuition/aesthetics)
□ If I'm wrong, I'll own it

→ ≥4/5 to proceed ←
```

---

### 🙏 Inspirations

- **First Principles** — Aristotle, Elon Musk
- **Adversarial Review** — legal cross-examination, scientific peer review
- **[Council of High Intelligence](https://github.com/0xNyk/council-of-high-intelligence)** — Multi-agent deliberation framework
- **[Superpowers](https://github.com/obra/superpowers)** — Structured workflows for AI-assisted development

---

### 📄 License

MIT © 2026 [shahuichao](https://github.com/shahuichao24-ops)
