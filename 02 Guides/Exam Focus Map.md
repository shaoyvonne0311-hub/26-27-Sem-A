---
tags: [finals, CB2203, guide]
updated: 2026-11-15
---
# 🎯 CB2203 Exam Focus Map

> [!abstract] 卷面（两份真题核对后）
> 12/10 Thu 09:30 · 闭卷 2 h · 50%。**2023-24 卷**：MCQ 20 + Q1 transport 25 + Q2 queue simulation 30 + Q3 scheduling 25；**2021-22 卷**：regression 20 / LP 10 + sensitivity 15 + 5 / NLP 20 / newsvendor simulation 30。两份卷唯一共同点：**都要建 LP、都要手算 simulation**。所以 80 分是可以背模板拿到的。

> [!warning] 你的 pp 文件夹里有假题
> `15-16 pp.pdf`、`19-20 pp.pdf` 是 **CB2200 Business Statistics**，不是本课；`21-22 pp.pdf` 与 `Past Paper.pdf` 是同一份。真正可用的只有 2 份：2021-22、2023-24。

---

## 1 · 频次与权重（按真题分值）

| 考点 ID | 考点 | 2021-22 | 2023-24 | 期望分 | 占本科 | 分配 |
|---|---|---|---|---|---|---|
| CB-SIMNEWS | newsvendor simulation（报童） | 30 | – | 15.0 | 15.0% | 6.0 h |
| CB-QUEUE | queue simulation（clinic，双服务台） | – | 30 | 15.0 | 15.0% | 6.0 h |
| CB-TRANS | transport + location LP | – | 25 | 12.5 | 12.5% | 5.0 h |
| CB-SCHED | scheduling / crashing | – | 25 | 12.5 | 12.5% | 5.0 h |
| CB-REG | regression 读数与预测 | 20 | – | 10.0 | 10.0% | 4.0 h |
| CB-NLP | non-linear program | 20 | – | 10.0 | 10.0% | 4.0 h |
| CB-MCQ | 读 Excel Answer / Sensitivity 报表 | – | 20 | 10.0 | 10.0% | 4.0 h |
| CB-SENS | sensitivity 三连问 | 15 | (MCQ 内) | 7.5 | 7.5% | 3.0 h |
| CB-LP | product-mix LP | 10 | – | 5.0 | 5.0% | 2.0 h |
| CB-LPCON | 加一条比例约束 | 5 | – | 2.5 | 2.5% | 1.0 h |

**读法**：simulation 两种合计 30%（最高），transport + scheduling 合计 25%，两者合起来 55 分；这三类都是「照模板一步步写」的题，不靠灵感。

---

## 2 · 优先级

- **A 档（必须闭眼写）**：CB-SIMNEWS、CB-QUEUE、CB-TRANS、CB-SCHED。
- **B 档（要会读会算）**：CB-REG、CB-NLP、CB-MCQ、CB-SENS。
- **C 档（有余力再碰）**：CB-LP、CB-LPCON（各只在一份卷里占 5–10 分）。

---

## 3 · 模板

### 3.1 Transport + location（25 分）
1. `Let Xij = quantity (litres) shipped from factory i to warehouse j`，i = 3 existing + 1 proposed，j = 4 warehouses。
2. capacity 变量：新厂必须满足 `Σ demand − Σ existing capacity`（数值题，2 分）。
3. 判据一句话：**minimise total production + transport cost**。
4. 目标函数逐个 cost 写：`ΣΣ (prod_i + trans_ij) Xij`；两个候选厂各建一个模型，只改 `prod_i` 与 `trans_ij`。
5. 约束：每厂容量 ≤；每仓需求 =；`Xij ≥ 0`。
6. 比较：算两个 total cost，写「Kumamoto vs Hiroshima 差 $X，故选…」。

### 3.2 Queue simulation（30 分）
固定表头六列；每个病人：`arrival = prev arrival + inter-arrival`；`start = max(arrival, doctor free, nurse free)`；`wait = start − arrival`；`finish = start + service`。三个绩效指标：average waiting time、average time in system、utilisation。**先画表再算平均，别跳步。**

### 3.3 Newsvendor simulation（30 分）
`RN → demand mapping → sales = min(demand, Q) → profit = 10 × sales − 5 × Q`；10 天平均；换一列 RN 说明样本波动；理论均值用概率加权；最优 Q 用 1–7 逐个跑，比平均利润。

### 3.4 Scheduling / crashing（25 分）
网络图（activity-on-node）→ 正推 ES/EF、逆推 LS/LF → slack = LS − ES → 关键路径 slack = 0 → 赶工成本 = (crash cost − normal cost) / weeks saved → 与罚款/工资比较：`crash cost < penalty saving` 才值得。

### 3.5 Regression / NLP（各 20 分）
Regression：`ŷ = b0 + b1x` 直接代入；斜率解释 = 「x 每增 1 单位，y 平均变 b1」；`u` = 其他未观测因素。
NLP：先把 revenue 与 cost 都写成 w 的函数，再写 `max profit(w)` + `s.t.` 预算约束；注意 `N = −2500 + 1000w` 代换。

---

## 4 · 陷阱

- 目标函数漏掉 production cost 或 transport cost 其中一项（25 分题直接掉一半）。
- 仿真表把 `service start` 写成 `arrival`，忽略服务台空闲。
- 赶工题只看 crash cost 不看罚款/工资对比。
- MCQ 报表题把 `allowable increase/decrease` 读成「可以随便改」。
- 单位不统一（litres vs $）。

---

## 5 · 最后 48 小时

1. 三套骨架默写：transport LP、queue 表头、crash 决策。
2. 两个整卷错题清单通读（11/28、11/30 的批改记录）。
3. 不再做新题；只看 `04 Tracker` 的红色。
4. 计算器、直尺、铅笔；12/09 早睡。

数据表：[[Finals 2026/PP Analysis & Priority.xlsx|PP Analysis & Priority.xlsx]] · 逐日：[[Finals 2026/01 Plan/30天逐日任务（PP加权）|30 天逐日任务]]
总纲：[[Finals 2026/00 Exam Brief & Revision Playbook|Exam Brief & Revision Playbook]]
