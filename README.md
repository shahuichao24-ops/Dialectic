<p align="center">
  <h1 align="center">🛡️ 驳真 · Dialectic</h1>
  <p align="center">
    <b>拍板“做不做”前的 30 秒极限压力测试。</b><br/>
    <sub>在写下第一行代码前做一次极限压力测试，拒绝无脑捧场，否定必给生路。</sub>
  </p>
  <p align="center">
    <img src="https://img.shields.io/badge/version-5.0.0-black?style=flat-square" alt="v5.0.0">
    <img src="https://img.shields.io/badge/dependencies-0-brightgreen?style=flat-square" alt="Zero Dependencies">
    <img src="https://img.shields.io/badge/prompt-~1.2k%20tokens-blue?style=flat-square" alt="~1.2k tokens">
    <img src="https://img.shields.io/badge/license-MIT-green?style=flat-square" alt="MIT">
  </p>
  <p align="center">
    <img src="assets/banner.jpg" alt="Dialectic Banner" width="100%">
  </p>
</p>

---

## 🇨🇳 中文版

### 1. 是什么？

**驳真 (Dialectic) 是一个专为你挑方案死穴的“AI 挑刺合伙人”。**

主流大模型几乎全是“奉承大师”，无论你说什么方案都顺着夸“太棒了、很有前景”。  
但在真实商业与产品立项中，**最昂贵的成本不是代码写得慢，而是做了一个根本没人要的伪需求。**

驳真在你投入任何研发资源、写下第一行代码之前，对你的想法做一次**残酷但理性的极限压力测试**：
- **拒绝捧场应声虫**：像挑剔的设计与业务评审一样，30 秒直击方案最薄弱的死穴。
- **好方案大方放行 (PASS)**：对低成本、高确定性的好方案直接放行，绝不为了显摆深刻而无病呻吟。
- **否定必给生路**：只要否定原方案，必须提炼底层核心诉求，给出一个仅需 **1/10 成本试水**的替代方案。

---

### 2. 标准输出长什么样？

一屏读完，30 秒直面真相，绝不废话：

```markdown
# 🔪 [功能必要 ｜ 组织阻力 ｜ 战略方向 ｜ 合规红线] 审查：[方案名称]
- 一句话结论：[大方通过 (PASS) ｜ 建议放弃 ｜ 小步快跑 ｜ 暂缓立项 / 补齐证据] ｜ 更好做法：[...]
- 别人踩过的坑 (全自动搜寻)：[自动嗅探检索到的代表竞品真实差评与痛点事实]
- 三句大实话：
  1. 谁吃亏：给谁添麻烦，会不会表面配合私下糊弄；
  2. 卡在哪：不做业务是否卡死，做砸几天能恢复；
  3. 出事谁背锅：自己能扛还是直接被罚停。
- 💡 更省钱省事的做法：[如果不做原方案，怎么花 1/10 的成本试水]
```

---

### 3. 四大不可妥协的底线

1. **Gate 0 误触即退**：常规文档审校、找错别字、代码审查 (Code Review)、代码编写等执行任务，**坚决不触发驳真**，直接转由常规助理角色处理。
2. **Gate 1 先顾人再顾事**：察觉用户疲惫或明确叫停（如“别驳我”）立刻退出，不追问、不输出卡片。
3. **Gate 2 好方案大方放行**：对低成本可逆、证据确凿的好方案大方 PASS，绝不抬杠。
4. **Gate 3 否定必给生路**：拒绝无建设性的泼冷水，否定必附带 1/10 成本验证方案。

---

### 4. 怎么使用？（零依赖 · 10 秒上手）

**纯提示词框架，无须安装任何环境或依赖：**

1. 打开本仓库的 [`SKILL.md`](SKILL.md)，复制全部文本；
2. 粘贴到你的任意 AI 环境中：
   - **Cursor / Windsurf Rules**（工作区或全局规则）
   - **Claude Project**（项目知识库 / 自定义说明）
   - **ChatGPT Custom Instructions**（自定义指令 / GPTs）
   - **Google Antigravity / OpenClaw 技能库**
3. 平时像正常聊天一样抛出你的点子：
   > *“我想给我的小工具加个每日打卡积分系统提高次留，帮我做个方案压力测试。”*

---

## 🇬🇧 English Version

### 1. What is it?

**Dialectic is an adversarial "Idea Challenger" AI designed to stress-test your product decisions.**

Mainstream LLMs are echo chambers. Whatever feature you propose, they praise it with *"Great idea!"* or *"Huge potential!"*.  
In real-world product development, **the most expensive mistake isn't slow coding — it's building something nobody actually wants.**

Dialectic subjects your proposal to a rigorous **30-second stress test** before you burn engineering hours:
- **Zero Sycophantic Flattery**: Refuses to be a yes-man; exposes fatal blind spots like a demanding design and business reviewer.
- **Clear Approval for Good Ideas (PASS)**: Approves low-cost, high-conviction ideas immediately. No nitpicking just to appear smart.
- **Mandatory Fallback Solution**: Every rejection must come with an actionable alternative that tests the core hypothesis at **1/10 of the original cost**.

---

### 2. Standard Output

Read in one screen, clear and actionable:

```markdown
# 🔪 [Necessity ｜ Friction ｜ Direction ｜ Compliance] Review: [Feature Name]
- Verdict: [PASS ｜ Drop It ｜ Small Step ｜ Hold / Needs Proof] ｜ Better Way: [...]
- Traps Others Fell Into: [Real user complaints and churn reasons scraped from competitor tools]
- Three Hard Truths:
  1. Who bears the burden: Whose workflow is disrupted? Will they secretly work around it?
  2. Where does it choke: If skipped, does business stop? If ruined, recovery time?
  3. Who takes the blame: Can you absorb the blow, or does it trigger regulatory shutdown?
- 💡 1/10 Cost Alternative: [How to test this value proposition with minimal resources]
```

---

### 3. Four Non-Negotiable Gates

1. **Gate 0: Mis-trigger Guard**: For doc review, typo correction, code reviews, or writing code, **Dialectic exits immediately** and lets standard assistants handle it.
2. **Gate 1: Empathy First**: If the user is exhausted or asks to stop (e.g., *"don't challenge me, just write code"*), exit silently.
3. **Gate 2: Generous Pass for Solid Ideas**: Low-cost, reversible, well-evidenced ideas get an immediate `PASS`.
4. **Gate 3: Constructive Rejection**: Never criticize without a way forward. Every rejection must offer a 1/10 cost alternative.

---

### 4. How to Use (Zero Dependencies · 10 Seconds)

**Pure markdown skill. No local runtime or setup required:**

1. Copy the contents of [`SKILL.md`](SKILL.md);
2. Paste it into your AI environment:
   - **Cursor / Windsurf Rules**
   - **Claude Project Instructions**
   - **ChatGPT Custom Instructions / GPTs**
   - **Google Antigravity / OpenClaw Skills**
3. Talk naturally:
   > *"I want to add a daily streak and loyalty points system to my app to boost retention. Give me an adversarial stress test on this proposal."*
