---
tags: [finals, playbook, index]
updated: 2026-11-15
---
# 🎯 考试总纲 · Exam Brief & Revision Playbook

> [!abstract] 一句话
> 五份卷子、五种题型逻辑，但只有一件事决定分数：**你能不能把真题里反复出现的那个 slot，用完整步骤做出来**。这份总纲给你三样东西：每科最重要的 20%（按 pp 频次算出来的）、每类题的答题模板、以及 30 天的执行规则。

> [!info] 数据来源
> 所有权重来自 [[Finals 2026/PP Analysis & Priority.xlsx|PP Analysis & Priority.xlsx]]：把你标记为 pp / exercise / past paper 的卷子逐题拆开，按考点统计分值，再换算成复习小时。逐日任务在 [[Finals 2026/01 Plan/30天逐日任务（PP加权）|30 天逐日任务（PP 加权）]]。

---

## 一、先说结论：什么最重要

按「expected marks × 科目权重 ÷ 所需小时」排序，真正决定生死的只有下面 9 件事：

| # | 科目 | 最重要的东西 | 真题证据 | 期望分 | 分配 |
|---|---|---|---|---|---|
| 1 | GE1359 | **6 个固定题位**：domain & range → exact value + general solution → Gaussian elimination → AM-GM + Vieta → induction + recurrence → counting | 4/4 份卷同结构，题位不动 | 85–90 / 100 | 55 h 中的 40 h |
| 2 | CB2203 | **simulation by hand**（newsvendor + queueing 两种都考）+ **transport LP** + **scheduling / crashing** | 各 1/2 份卷，但合计 80 分 | 80 / 100 | 40 h 中的 28 h |
| 3 | MKT3603 | **concept discrimination**：L5 decision biases、L2 perception chain、L4 persuasion、L1 motivation | 4 份 in-class quiz 全是同一个句式 | 约 60–70 / 100 | 36 h 中的 23 h |
| 4 | MKT3601 | **luxury-brand case 五问** + consumer trends + standardisation | case 出现在 4/7 份卷 | 一整题 50 分 | 30 h 中的 8 h |
| 5 | CB2240 | **loops + functions（含 recursion）** | 每份卷都出现，命中密度最高 | 40% 中的 55%+ | 28 h 中的 16 h |

**一句话版本**：GE1359 是「稳拿」，CB2203 是「模板题」，MKT3603 是「词汇辨析」，MKT3601 是「写作」，CB2240 是「手速」。时间不够时，先砍 GE1359 的 C 档（complex roots / sum-to-product，各只占 1/4 份卷）和 MKT3601 的 guanxi（1/7 份卷）。

---

## 二、五份卷子长什么样（已核对真题原文）

| 科目 | 时间 | 权重 | 允许材料 | 卷面结构（来自 pp） |
|---|---|---|---|---|
| CB2203 | 12/10 Thu 09:30 | 50% | 闭卷 | 2023-24：**MCQ 20** + Q1 transport 25 + Q2 queue simulation 30 + Q3 scheduling 25；2021-22：5 题（regression 20 · LP 10 + sensitivity 15 + 5 · NLP 20 · newsvendor simulation 30） |
| GE1359 | 12/12 Sat 18:30 | **70%** | 闭卷 + trig formula sheet | **6 题 100 分**：Q1 domain & range（+ inequality / composite / complex roots）· Q2 exact value + general solution · Q3 Gaussian elimination · Q4 AM-GM + Vieta · Q5 induction + recurrence · Q6 counting |
| CB2240 | 12/14 Mon 14:00 | 40% | **cheat sheet** | quiz-style：MCQ（trace / output）+ 3–4 道 code-writing LQ；**coursework 与 exam 都要及格** |
| MKT3601 | 12/15 Tue 09:30 | 40% | **开卷，只准纸质** | 3 题选 2，Q1 必答 = 每周概念定义；Q2/Q3 = essay（旧卷主体是 luxury-brand case 五问 / 宏观题） |
| MKT3603 | 12/16 Wed 14:00 | 50% | 闭卷 + **1 张 A4 单面** | vignette → "which concept does this best illustrate?" + 长题（essay 可能） |

> [!warning] 三个必须先记住的发现
> ① `CB2203/pp/15-16 pp.pdf` 与 `19-20 pp.pdf` 其实是 **CB2200 Business Statistics**——不是本课真题，复习时别用。
> ② `21-22 pp.pdf` 与 `Past Paper.pdf` 是同一份卷（相似度 78%），只算一份。
> ③ MKT3603 没有任何 pp，只有 4 份 in-class quiz，所以它的权重是「quiz 命中 × 讲义页数」推出来的，不是分值。

---

## 三、四套通用训练法（五科共用）

1. **Blank-page recall**：合上书，先写考点名与步骤，再对答案。写不出来的才是要复习的。
2. **Timed rep**：同一个 slot 连做 3 遍——第 1 遍不限时求对，第 2 遍限时求快，第 3 遍只写骨架求稳。
3. **Mistake → Rule**：Mistake Log 只写一句「下次怎么做」，不抄题。例：`Dom(G⁻¹) = Ran(G)，不要用反函数的自然定义域`。
4. **Spaced revisit N+1 / N+3 / N+7**：同一考点至少三次不同日期的涂色；颜色比次数重要。

---

## 四、五套答题模板

### 4.1 CB2203 · LP / transport
1. 写 `Let Xij = ...`（下标含义 + 单位，一句话）。
2. 目标函数：`Min ΣΣ (production cost + transport cost) × Xij`。
3. 约束：每条一行，右边常数；容量 ≤，需求 =。
4. 收尾 `All Xij ≥ 0`。比较两个候选厂址时只比总成本，不重写模型。

### 4.2 CB2203 · simulation by hand
固定表头：`RN → inter-arrival → arrival → service start → service time → finish → wait`。先算累计再算平均，每步写公式不心算。排队题注意 **doctor 与 nurse 同时空闲**才可开始服务。

### 4.3 GE1359 · domain & range
- Domain：radicand ≥ 0、denominator ≠ 0，取交集，写 `ℝ\{…}` 或区间。
- Range：配方法或 `k/√(quadratic)`，注意端点开闭；`Dom(G⁻¹) = Ran(G)`。

### 4.4 GE1359 · Gaussian elimination
增广矩阵 → 行变换到 echelon → 看最后一行 `0 = c`：
- `0 = 非零` → no solution；自由变量数 = 未知数 − rank；再分别写 one free / two free 的参数解。

### 4.5 MKT3601 · essay（55 分钟）
`Thesis（1 句）→ Define（术语 + 框架）→ 3 段论证（每段 concept + case/number）→ Counter-argument（to what extent）→ Recommendation（manager / policy 视角）`。每段必须有一个英文术语 + 一个具体例子。

### 4.6 MKT3603 · vignette → concept
先给场景贴标签（谁、什么 threat、什么 motive），再排除三个「看似相关但层级不对」的术语，最后一句写「为什么是这个而不是那个」。

---

## 五、考场时钟

| 科目 | 总时长 | 分配 |
|---|---|---|
| CB2203 | 120 min | MCQ 20′ · Q1 30′ · Q2 40′ · Q3 30′ |
| GE1359 | 120 min | 6 题各 15–18′；Q3 与 Q6 各留 20′；检查 8′ |
| CB2240 | 120 min | MCQ 40′ · LQ 每题 20–25′；先骨架后细节 |
| MKT3601 | 120 min | Q1 50′ · essay 55′ · 检查 15′（开卷只查定义，不读书） |
| MKT3603 | 120 min | MCQ 45′ · 长题 55′ · A4 查证 ≤ 10′ |

---

## 六、30 天规则

1. **先红后绿**：每天第一块时间永远给 Tracker 上的 `R`。
2. **写作前置**：MKT3601 的 2 篇 essay、MKT3603 的长题，必须在 **12/07** 前各写完 2 遍。
3. **整卷节奏**：GE1359 四份卷放在 11/23、11/25、12/01、12/03；CB2203 两份放在 11/28、11/30；最新一份留最后。
4. **最后 48 小时只做三件事**：模板默写、错题清单、A4 / cheat sheet 定稿。不刷新题。
5. **掉队处理**：删 C 档，不删 A 档；宁可少做一类，不可跳过红色。

> [!note] 关于 11/16
> 全库、`plan.json`、CityU 日历都没有 11/16 的考试。若确有，只有 MKT3603 的单日稿可用；否则从今天起按这份 30 天表走。

---

## 七、文件索引

- 逐日任务：[[Finals 2026/01 Plan/30天逐日任务（PP加权）|30 天逐日任务（PP 加权）]]
- 数据表：[[Finals 2026/PP Analysis & Priority.xlsx|PP Analysis & Priority.xlsx]]（`01 题库` · `02 频次` · `03 权重` · `04 Tracker` · `06 逐日`）
- 各科细化：[[Finals 2026/CB2203 Data-driven Business Modeling/02 Guides/Exam Focus Map|CB2203]] · [[Finals 2026/GE1359 Final/02 Guides/Exam Focus Map|GE1359]] · [[Finals 2026/CB2240 Python/02 Guides/Exam Focus Map|CB2240]] · [[Finals 2026/MKT3601 China Business Environment/02 Guides/Exam Focus Map|MKT3601]] · [[Finals 2026/MKT3603 Consumer Behaviour/02 Guides/Exam Focus Map|MKT3603]]
- 原计划：[[Finals 2026/01 Plan/Calendar|Calendar]] · `01 Plan/plan.json`（**时间仍以它为准**，本页只改权重与内容）
