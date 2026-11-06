# Decision Ledger (定论账本)

> **Purpose**: Prevent teams and solo builders from re-debating settled decisions over and over.  
> **Readback Rule**: When Dialectic triggers, it first checks this ledger.  
> - **Hit & Premises Unchanged** → Surface prior verdict & premises, ask strictly *"Have the underlying premises changed?"*, and immediately stop debate.  
> - **Premises Flipped** → Reopen and proceed with a full 30-second stress test.

---

## 1. [Example] Rewrite Core Backend in Rust · Rejected

- **Verdict**: Drop it. Maintain existing TypeScript/Go services.
- **Why Rejected**: Current p99 latency is under 40ms. The engineering team has zero production Rust experience; estimated delivery delay would exceed 4 months.
- **Underlying Premises**:
  1. Service traffic remains below 15,000 QPS.
  2. Cloud compute costs remain within budget (<$1,500/mo).
  3. Team hiring profile is centered on Go/TypeScript.
- **Reopen Condition**: Single-node memory leakage becomes unresolvable, or sustained QPS exceeds 50,000.

---

## 2. [Example] Introduce In-App Social Feed & Comments · Rejected

- **Verdict**: Drop it. Focus strictly on core utility workflows.
- **Why Rejected**: Adding community features shifts product into content moderation, spam compliance, and UGC notification fatigue. Churn risk outweighs viral upside.
- **Underlying Premises**:
  1. Product positioning is an asynchronous utility/efficiency tool.
  2. Zero dedicated community moderation staff.
- **Reopen Condition**: Business model explicitly pivots to a creator community platform with dedicated moderation budget.

---

## 3. [Example] Self-Hosted Kubernetes Cluster · Suspended

- **Verdict**: Suspended. Stay on PaaS / Managed Container Services.
- **Why Rejected**: SRE team consists of 1 part-time engineer. The operational overhead of cluster maintenance, upgrades, and ingress debugging exceeds productivity gains.
- **Underlying Premises**:
  1. Production services count <= 6.
  2. No dedicated 24/7 on-call infrastructure engineers.
- **Reopen Condition**: Microservice fleet exceeds 15 discrete services or dedicated DevOps hire arrives.

---

## Readback Audit Log (读回记录)

> Append one line each time Dialectic halts or reopens a debate. Count monthly; prune entries that never get challenged.

- `2026-11-06` · [Topic: Rust Rewrite] · Halted re-debate (Premises unchanged).
