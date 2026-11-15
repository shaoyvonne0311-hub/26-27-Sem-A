---
tags: [finals, diagnostic, answer-key]
updated: 2026-11-15
---

# Diagnostic Answer Key（先做完再打开）

## CB2203（42）

| 题 | 答 | 要点 |
|---|---|---|
| A1 | C | 角点 (6,4)：240+120=360 |
| A2 | A | shadow price 的有效范围到下一个 binding 变化为止 |
| A3 | B | 左上角、取 min(供给,需求) |
| A4 | B | EDD 最小化最大延迟 |
| A5 | C | ρ=.8，L=ρ/(1−ρ)=4 |
| A6 | B | .37 落在 .25–.60 → 40 |
| A7 | A | R² 是解释变异比例 |
| A8 | C | 8/(8+2)=0.8 |
| A9 | B | Solver |
| A10 | D | 9+3=12>10 |

**B1 (a)** P1→W1 100；P2→W1 20、P2→W2 130；P3→W3 100。  
Cost = 100×5 + 20×6 + 130×7 + 100×7 = **2230**。  
**(b)** 令 x_ij = 从厂 i 运到仓 j 的数量；P1 供给约束 x11+x12+x13 ≤ 100（供需相等时可写 =100）。

**B2 (a)** ρ=0.8；P0=0.2；L=4；Lq=3.2；W=0.5 h；Wq=0.4 h。  
**(b)** λ=4 → ρ=0.4；L=0.667；W=0.167 h（10 min）。

## GE1359（50）

**Q1 (a)** −1 < x < 6 → (−1, 6)。  
**(b)** x ≥ 1 且 x ≠ ±2 → **[1,2) ∪ (2,∞)**。  
**(c)** (x−5)(x+2) ≤ 0 → **[−2, 5]**。

**Q2 (a)** (2cos x +1)(cos x −1)=0 → cos x=1: x=0, 2π；cos x=−1/2: x=2π/3, 4π/3。答案 **0, 2π/3, 4π/3, 2π**。  
**(b)** 2x = π/3 + kπ → **x = π/6 + kπ/2, k∈Z**。

**Q3** 由 eq2−2eq1: −3y − z = −9；eq3−eq1: y − 2z = −4。解得 **x=1, y=2, z=3**。

**Q4 (a)** AM–GM: x + 4/x ≥ 2√4 = 4，等号 x=2 → **min 4 at x=2**。  
**(b)** α+β=5, αβ=6 → α²+β²=25−12=**13**；α³+β³=125−3×6×5=**35**。

**Q5 (a)** n=1: 1=1。假设 n=k 成立，则 n=k+1 时前 k+1 项 = k² + (2k+1) = (k+1)²。成立。  
**(b)** 令 bₙ=aₙ+1，则 bₙ=3bₙ₋₁，b₁=2 → **aₙ = 2·3^{n−1} − 1**。

**Q6 (a)** 6! − 2×5! = 720−240 = **480**。  
**(b)** 个位 2 或 4（2 种），百位 4 种，十位 3 种 → **24**。

## CB2240（38）

| 题 | 答 |
|---|---|
| A1 | 3 |
| A2 | `7 13` |
| A3 | C |
| A4 | `mid` |
| A5 | `"yth"` / `"nohtyP"` |
| A6 | `[1, 2, 3, 4]`（b 与 a 同一对象） |
| A7 | `0`；之后 len=2 |
| A8 | 6 |
| A9 | 调用处 `[1,2,3] + 4` 触发 TypeError；应传 `[1,2,3,4]` 或 `+ [4]` |
| A10 | 文件行数 |

**B1 参考**
```python
def word_count(path):
    counts = {}
    with open(path) as f:
        for line in f:
            for w in line.split():
                w = w.strip(".,!?").lower()
                if w:
                    counts[w] = counts.get(w, 0) + 1
    return counts
```
**B2 参考**
```python
class Account:
    def __init__(self, balance=0):
        self.balance = balance
    def deposit(self, amount):
        self.balance += amount
    def withdraw(self, amount):
        if amount > self.balance:
            raise ValueError("insufficient funds")
        self.balance -= amount
```

## MKT3601（50）评分看关键词

**Q1（每题 2）**：TRENDS 升级/降级 + 例；REGION 一线/三线差距；ECON-TRANS 计划→市场；KOL 大 V vs KOC 素人；ECOMM 社交/直播/拼单；GUANXI 关系网络 + 交易成本。

**Q2（每小问 4）**  
(a) 明确 segment 维度（年龄/城市/收入/动机）+ 为什么；  
(b) 直营/旗舰/代理/电商的取舍 + 两个 issue（假货、渠道冲突、定价、审批）；  
(c) 三条 derisk（定价锚、官方渠道、KOL 合约、库存）；  
(d) 全球标准 vs 本地表达（产品/店装/传播）；  
(e) KOL 角色 + 风险（翻车、水军、合规）。

**Q3（18）**：SOE 改革（产权、混合所有制、效率）+ 可持续（治理、ESG、绿色消费）+ 二者共同点（激励与问责）+ 市场结果。

## MKT3603（42）

| 题 | 答 | 题 | 答 |
|---|---|---|---|
| 1 | B | 9 | A |
| 2 | A | 10 | B |
| 3 | A | 11 | A |
| 4 | C | 12 | B |
| 5 | B | 13 | B |
| 6 | A | 14 | A |
| 7 | A | 15 | C |
| 8 | B | | |

**B1** sunk cost：已付出不可回收仍影响决策；mental accounting：把钱分账（娱乐账户/生活账户）。例：演唱会票；违背理性因为忽略边际成本。  
**B2** attitude = 评价倾向（认知+情感+行为）；memory = 存储与提取。强态度 → 更快、更稳定选择，抗说服。  
**B3** 参照群体提供规范/信息；brand community 通过认同与仪式强化忠诚，也可能排斥外人。
