---
tags: [finals, CB2203, diagnostic]
time: 50 min
marks: 42
updated: 2026-11-15
---

# CB2203 诊断卷 Diagnostic（50 min / 42 marks）

> [!warning] 闭卷限时
> 不看书、不查 Excel。做完再对 `Diagnostic Answer Key`，把每题得分填进 `PP Analysis & Priority.xlsx` 的 `07 诊断 Diagnostic`。只有闭卷做出来才算 G。

## Part A — MCQ（10 × 2 = 20 marks）

**A1.** Maximise 40x + 30y subject to x + y ≤ 10, 2x + y ≤ 16, x, y ≥ 0. The optimal objective value is
A. 300　B. 320　C. 360　D. 400

**A2.** A shadow price of 20 on a labour-hour constraint means
A. each extra labour hour raises profit by at most 20, valid until the constraint stops binding
B. labour cost is 20 per hour
C. profit rises by 20 for every extra unit produced
D. the constraint is redundant

**A3.** In the north-west corner method, the first allocation is made to
A. the cell with the lowest cost
B. the top-left cell, as much as possible within supply and demand
C. the cell with the highest cost
D. the cell with the largest supply

**A4.** EDD sequencing minimises
A. average flow time　B. maximum lateness　C. makespan　D. number of tardy jobs

**A5.** An M/M/1 queue has λ = 8/hour and μ = 10/hour. Average number in system L is
A. 0.8　B. 1.25　C. 4　D. 5

**A6.** Demand is simulated with cumulative probabilities 0.25 → 20 units, 0.60 → 40 units, 1.00 → 60 units. Random number 0.37 maps to
A. 20　B. 40　C. 60　D. 37

**A7.** A regression gives R² = 0.81. This means
A. 81% of the variation in y is explained by the model
B. the model predicts 81% of cases correctly
C. the slope is 0.81
D. 19% of observations are outliers

**A8.** A newsvendor has underage cost 8 and overage cost 2. The critical ratio (target service level) is
A. 0.2　B. 0.6　C. 0.8　D. 4

**A9.** In Excel, the tool that directly solves a linear programme is
A. Goal Seek　B. Solver　C. PivotTable　D. Data Table only

**A10.** Which point is infeasible for x + y ≤ 10, 2x + y ≤ 16, x, y ≥ 0?
A. (0, 8)　B. (4, 4)　C. (8, 2)　D. (9, 3)

## Part B — Long questions（22 marks）

**B1. Transportation (12 marks)**
Plants P1, P2, P3 supply 100, 150, 100. Warehouses W1, W2, W3 demand 120, 130, 100. Unit costs:

|      | W1 | W2 | W3 |
|------|----|----|----|
| P1   | 5  | 8  | 9  |
| P2   | 6  | 7  | 10 |
| P3   | 8  | 6  | 7  |

(a) Build the north-west corner initial solution and compute its total cost. **(8)**
(b) Write the decision-variable definition and the supply constraint for P1. **(4)**

**B2. Queueing (10 marks)**
Customers arrive at one counter at λ = 8 per hour; service rate μ = 10 per hour (M/M/1).
(a) Compute ρ, P0, L, Lq, W, Wq in hours. **(6)**
(b) If arrivals fall to 4 per hour with the same μ, recompute L and W. **(4)**

## 交卷后
1. 对答案，红笔标失分点。
2. 把每题得分填进 Excel `07 诊断 Diagnostic`，G/Y/O/R 会自动出。
3. 低于 50% 的 topic 写进 Mistake Log，并在接下来 3 天优先排。

> [!success]- 答案（做完再看）
> A1 C · A2 A · A3 B · A4 B · A5 C · A6 B · A7 A · A8 C · A9 B · A10 D
> B1：P1→W1 100；P2→W1 20、W2 130；P3→W3 100；成本 2230。变量 x_ij + 供给约束。
> B2：ρ=.8，P0=.2，L=4，Lq=3.2，W=.5 h，Wq=.4 h；λ=4 → L=.667，W=.167 h。
