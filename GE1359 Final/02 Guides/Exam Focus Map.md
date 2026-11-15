---
tags: [finals, GE1359, guide]
updated: 2026-11-15
---
# 🎯 GE1359 Exam Focus Map

> [!abstract] 卷面（4 份 Past Final 逐题核对）
> 12/12 Sat 18:30 · 闭卷 2 h · **70%**（期末占分最高的一科）。**6 题 100 分，题位四年不动**：Q1 domain & range（+ 一个轮换小问）→ Q2 exact value + general solution → Q3 Gaussian elimination → Q4 AM-GM + Vieta → Q5 induction + recurrence → Q6 counting。8 个 slot 出现率 4/4，合计 **85–90 分**；只有 15 分是轮换的。

> [!info] 与期中分析的差别
> `GE1359 Revision Vault/02 Guides/Past Paper Analysis` 分析的是 **Past Test Papers**（Ch1–3、7 题）；本页分析的是 **Past Final Exam Papers**（6 题、含 Ch4 induction 与 Ch5 binomial/counting）。两者题位不同，别混用。

---

## 1 · 频次与权重

| 考点 ID | 考点 | S2024 | 2425A | S2025 | 2526A | 期望分 | 占比 | 分配 |
|---|---|---|---|---|---|---|---|---|
| GE-COUNT | counting / arrangements | 20 | 18 | 20 | 21 | 19.8 | 19.8% | 10.9 h |
| GE-GAUSS | Gaussian elimination 讨论解 | 15 | 14 | 14 | 14 | 14.2 | 14.2% | 7.8 h |
| GE-VIETA | Vieta / 三次方程 | 8 | 12 | 12 | 8 | 10.0 | 10.0% | 5.5 h |
| GE-GENSOL | general solution（弧度） | 15 | 7 | 8 | 8 | 9.5 | 9.5% | 5.2 h |
| GE-DR | domain & range | 9 | 9 | 8 | 10 | 9.0 | 9.0% | 5.0 h |
| GE-AMGM | AM-GM 最小值 | 8 | 9 | 8 | 9 | 8.5 | 8.5% | 4.7 h |
| GE-IND | induction（整除/不等式） | 8 | 9 | 8 | 8 | 8.2 | 8.2% | 4.5 h |
| GE-RECUR | recurrence induction | 9 | 8 | 8 | 8 | 8.2 | 8.2% | 4.5 h |
| GE-INEQ | inequality（区间记号） | – | 8 | – | 8 | 4.0 | 4.0% | 2.2 h |
| GE-EXACT | 精确值（不用计算器） | – | 6 | – | 6 | 3.0 | 3.0% | 1.6 h |
| GE-COMP | 三重复合 + 定义域 | 8 | – | – | – | 2.0 | 2.0% | 1.1 h |
| GE-CROOTS | 已知复根求全部根 | – | – | 7 | – | 1.8 | 1.8% | 1.0 h |
| GE-SUM2PROD | 和差化积求 tan(α+β) | – | – | 7 | – | 1.8 | 1.8% | 1.0 h |

**读法**：Q3 + Q6 两题就占 34%，而且都是「分类讨论 + 数清楚」的题；Q4 + Q5 四小问占 27%。这四题合起来 61 分，全靠模板。

---

## 2 · 优先级

- **A 档**：GE-COUNT、GE-GAUSS、GE-VIETA、GE-GENSOL。
- **B 档**：GE-DR、GE-AMGM、GE-IND、GE-RECUR。
- **C 档（只占 1 份卷）**：GE-CROOTS、GE-SUM2PROD、GE-COMP、GE-INEQ、GE-EXACT。

> [!tip] 时间分配原则
> A 档四类必须做到「闭卷、限时、全对」；B 档做到「闭卷做对」；C 档只需认得题型、会起手。

---

## 3 · 模板

### 3.1 Domain & range（8–10 分）
- Domain：radicand ≥ 0、denominator ≠ 0、log 内 > 0，取交集；写 `ℝ\{a,b}` 或 `[a,b)`。
- Range：配方成 `k/√(c − (x−h)²)` 或 `c + k/(x+a)`，端点开闭逐点判断。
- 常见：`5/√(16 − x²)` → range `[5/4, ∞)`；`(4x−9)/(x−5)` → `(−∞,4) ∪ (4,∞)` 型。

### 3.2 Gaussian elimination（14–15 分）
1. 写增广矩阵。
2. 行变换到 echelon，**不跳步**（步骤分就在这里）。
3. 关键行 `(0 0 … 0 | c)`：
   - `c ≠ 0` → no solution，给出 a（和 b）的取值。
   - `c = 0` → 看 rank：`rank = n − 1` → one free variable；`rank = n − 2` → two free variables。
4. 自由变量设参数 `t, s`，回代写通解。

### 3.3 AM-GM（8–9 分）
把式子拆成 2–4 项，使乘积为常数：`a + b ≥ 2√(ab)`，等号条件写清 `a = b`，并解出 x、y 的具体值。**必须写 equality condition**，否则丢最后一分。

### 3.4 Vieta（8–12 分）
- `α+β+γ = −p`，`αβ+βγ+γα = q`，`αβγ = −r`。
- 求 `α²+β²+γ² = p² − 2q`；求 `α³+β³+γ³` 用 `S1³ − 3S1S2 + 3S3`。
- 求「以 α³, β³, γ³ 为根的三次方程」：算 `S1, S2, S3` 后写 `t³ − S1 t² + S2 t − S3 = 0`。

### 3.5 Induction（8–9 分）
固定四段：`Base case (n = …)` → `Assume true for n = k` → `Show for n = k+1` → `Conclusion`。整除题把 `f(k+1) − f(k)` 提出因子；不等式题从 assumption 直接放缩。

### 3.6 Recurrence induction（8–9 分）
给定 `a1, a2` 与 `a(n+2) = …`：base case 要验 **两个**初始值；step 用两条递推代入目标式化简。

### 3.7 Counting（18–21 分，三小问）
- (a) 全排列：`n!/∏(重复字母阶乘)`。
- (b) 带条件：先算 total，再减「相邻」捆绑法；「no two vowels adjacent」用插空法。
- (c) 取 k 个字母：按「取到几个重复字母」分类，逐类相加。**分类要不重不漏，写清每类数量。**

### 3.8 Exact value / general solution（6–8 分）
- 精确值：`sin10°sin50°sin70°` 这类先乘 `2cos10°` 造倍角，再连锁约分。
- General solution：先化成 `sin/cos/tan = k`，再写 `x = nπ + (−1)ⁿα` 或 `2nπ ± α`；**两组 family 分开写，n ∈ ℤ**。

---

## 4 · 陷阱

- 区间写成 `[a, ∞]`（∞ 永远用圆括号）。
- 行列变换跳步 → 步骤分全丢。
- 自由变量个数数错（= 未知数 − rank，不是看零行）。
- 归纳法 base case 只验一个（递推题要验两个）。
- counting 用「总数 − 相邻」时忘了重复字母已除。
- general solution 只写一组 family，或忘记 `n ∈ ℤ`。

---

## 5 · 最后 48 小时

1. 四份卷的错题清单按 A→B 顺序过一遍（11/23、11/25、12/01、12/03 的批改）。
2. 五套模板默写：DR、Gaussian、AM-GM/Vieta、induction、counting。
3. 12/11 只做 Q1–Q3 的 sweep（75 分钟），不碰新卷。
4. 12/12 上午只看公式表与陷阱清单；晚上 18:30 开考。

数据表：[[Finals 2026/PP Analysis & Priority.xlsx|PP Analysis & Priority.xlsx]] · 逐日：[[Finals 2026/01 Plan/30天逐日任务（PP加权）|30 天逐日任务]]
总纲：[[Finals 2026/00 Exam Brief & Revision Playbook|Exam Brief & Revision Playbook]]
