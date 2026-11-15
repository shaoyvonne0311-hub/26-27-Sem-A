---
tags: [finals, mastering, checkpoint]
updated: 2026-11-15
---

# 三日检测 Mastering Checks

> [!info] 用法
> 每 3 天一次，**闭卷 15–20 min**，先写完再看每节底部的折叠答案。得分记进 `PP Analysis & Priority.xlsx` → `07 诊断 Diagnostic` 对应 topic 行（F 列），等级自动刷新。基线卷在 11/16–11/18 做，之后按本页日期推进。

| # | 日期 | 覆盖科目 | 预计 |
|---|---|---|---|
| M1 | 11/18 | GE / CB2203 / MKT3603 / CB2240 / MKT3601 | 20 min |
| M2 | 11/21 | GE / CB2203 / CB2240 / MKT3601 / MKT3603 | 20 min |
| M3 | 11/24 | GE / CB2203 / MKT3601 / CB2240 | 18 min |
| M4 | 11/27 | GE / CB2203 / MKT3603 / MKT3601 / CB2240 | 20 min |
| M5 | 11/30 | CB2203 / MKT3603 / GE | 15 min |
| M6 | 12/03 | CB2203 / GE / MKT3603 / CB2240 | 18 min |
| M7 | 12/06 | MKT3601 / MKT3603 / CB2203 / CB2240 | 20 min |
| M8 | 12/09 | CB2203 / GE / MKT3603 / MKT3601 | 18 min |
| M9 | 12/12 | GE 六 slot 全扫 | 20 min |
| M10 | 12/15 | CB2240 / MKT3601 / MKT3603 | 18 min |

---

## M1 · 11/18

1. **GE** Find the domain of f(x)=√(x+2)/(x−1).
2. **GE** General solution of cos x = 1/2.
3. **CB2203** In one sentence: what does a shadow price of 12 on machine hours allow you to claim?
4. **CB2203** M/M/1: λ=6/h, μ=8/h. Find ρ and L.
5. **MKT3603** Distinguish sunk cost effect and framing effect with one example each.
6. **MKT3603** Give one example of just-noticeable difference (JND) in pricing.
7. **CB2240** Output:
```python
t = 0
for i in range(1, 5):
    t += i if i % 2 else -i
print(t)
```
8. **MKT3601** Define consumption downgrading and give one China example.

> [!success]- 答案 M1
> 1. x ≥ −2 且 x ≠ 1 → **[−2,1) ∪ (1,∞)**。  
> 2. x = ±π/3 + 2kπ。  
> 3. 每多 1 小时机器时间，利润最多增加 12，直到该约束不再 binding。  
> 4. ρ=.75；L=ρ/(1−ρ)=**3**。  
> 5. sunk cost：已付不可回收的钱仍影响决定（演唱会票）；framing：同一事实不同表述改变选择（“90% 存活” vs “10% 死亡”）。  
> 6. 20 元商品涨 3 元会被察觉，2 万元包涨 3 元不会——差异未超过 JND。  
> 7. i=1:+1；2:−2→−1；3:+3→2；4:−4→−2 → **−2**。  
> 8. 消费者从“买贵/炫耀”转向“性价比/理性”，例：拼多多、白牌、临期食品。

## M2 · 11/21

1. **GE** Solve x² − 5x + 6 > 0.
2. **GE** For 2x² − 7x + 3 = 0, write α+β and αβ.
3. **CB2203** How do you balance an unbalanced transportation problem?
4. **CB2203** Cu=12, Co=3. Critical ratio?
5. **CB2240** Output:
```python
a = [1, 2]
b = a
b += [3]
print(a, b is a)
```
6. **CB2240** `d={"x":1}`; `d.get("y")` returns what? How to avoid KeyError on `d["y"]`?
7. **MKT3601** What are tier-1 / tier-3 cities, and why does the gap matter for luxury entry?
8. **MKT3603** Distinguish anchoring and framing.

> [!success]- 答案 M2
> 1. (x−2)(x−3)>0 → **x<2 或 x>3**。  
> 2. α+β=**7/2**，αβ=**3/2**。  
> 3. 加一个 dummy warehouse/plant，补 0 成本列/行，使总供给=总需求。  
> 4. 12/(12+3)=**0.8**。  
> 5. `[1,2,3]`；`True`（`+=` 原地修改）。  
> 6. `None`；用 `d.get("y", 0)` 或 `if "y" in d`。  
> 7. 一线（北上广深）vs 三线（地级市）；消费力、渠道、审美与价格敏感度不同，决定布点与产品线。  
> 8. anchoring：先给参考价（999 后再 699）；framing：改表述方式（打折 vs 满减）。

## M3 · 11/24

1. **GE** Solve x+y=5, 2x−y=1.
2. **GE** In the induction proof of 1+…+n = n(n+1)/2, write the key step from k to k+1.
3. **CB2203** What does “range of optimality” mean in LP sensitivity?
4. **CB2203** M/M/1: λ=3/h, μ=5/h. Find L and Lq.
5. **MKT3601** List three entry issues for a foreign brand in China.
6. **CB2240** Write a 3-line function `count_vowels(s)`.
7. **MKT3601** What is the downside of relying on guanxi?

> [!success]- 答案 M3
> 1. 相加 3x=6 → x=2, y=3.  
> 2. 假设 k 成立：1+…+k=k(k+1)/2；加 (k+1) 得 k(k+1)/2+(k+1)=(k+1)(k+2)/2。  
> 3. 目标函数系数在此区间内变化时，**最优解不变**（最优值会变）。  
> 4. ρ=.6；L=1.5；Lq=ρ²/(1−ρ)=**0.9**。  
> 5. 假货/水货、渠道冲突、定价与促销、监管审批、品牌定位失真（任三）。  
> 6. `def count_vowels(s): return sum(c in "aeiouAEIOU" for c in s)`  
> 7. 关系可带来交易便利，但抬高合规风险、难以规模化、人走关系断。

## M4 · 11/27

1. **GE** For x>0, minimise 2x + 8/x.
2. **GE** Five people in a row, A and B adjacent: how many arrangements?
3. **CB2203** What does a 90% service level mean in the newsvendor model?
4. **CB2203** Which sequencing rule minimises average flow time?
5. **MKT3603** Primacy vs recency effect — one line each.
6. **MKT3601** Give three de-risking moves for a luxury entrant.
7. **CB2240** Output:
```python
class P:
    def __init__(self, n): self.n = n
    def add(self, k): self.n += k; return self.n
p = P(3); print(p.add(2), p.n)
```

> [!success]- 答案 M4
> 1. 2x+8/x ≥ 2√16=8，等号 x=2 → **8 at x=2**。  
> 2. 捆成一块：2 × 4! = **48**。  
> 3. 有 90% 概率不缺货（需求量 ≤ 订货量），缺货概率 10%。  
> 4. **SPT**（最短加工时间优先）。  
> 5. primacy：先出现的记得牢；recency：最后出现的记得牢。  
> 6. 官方渠道/防伪、价格锚与控价、KOL 合约与合规、库存与退换（任三）。  
> 7. `5 5`（add 返回新值并已改 self.n）。

## M5 · 11/30

1. **CB2203** Regression slope 2.5 with price coefficient — interpret in one sentence.
2. **CB2203** Why order at the critical-ratio quantile rather than the mean in newsvendor?
3. **CB2203** In NW corner, after P1 is exhausted, where does the next allocation go?
4. **MKT3603** Compromise effect vs decoy effect.
5. **MKT3603** What is the extended self? One example.
6. **GE** Solve sin 2x = 0 for 0 ≤ x ≤ 2π.

> [!success]- 答案 M5
> 1. 价格每升 1 单位，y 平均变化 2.5 单位（其余不变）。  
> 2. 因为缺货与过剩成本不对称，最优解在分位点 Cu/(Cu+Co)，不是均值。  
> 3. 移到同一行下一个仓库（W2），用 P2 的剩余供给补。  
> 4. compromise：三个选项选中间；decoy：加一个明显差的选项衬托目标。  
> 5. 把自我延伸到拥有物上（“我的车代表我”）。  
> 6. 2x=kπ → x=0, π/2, π, 3π/2, 2π。

## M6 · 12/03

1. **CB2203** Write the objective and one supply constraint for: plants A/B supply 50/70, warehouse demand 60.
2. **CB2203** In Solver, how do you know a constraint is binding?
3. **GE** Solve |x−3| ≥ 2.
4. **GE** Solve aₙ=2aₙ₋₁+1, a₁=1.
5. **MKT3603** Normative vs informational social influence.
6. **CB2240** Fix: `for i in range(len(lst)): print(lst[i+1])` — what goes wrong at the end?
7. **CB2240** What does `with open(...) as f` guarantee?

> [!success]- 答案 M6
> 1. max Σ c_ij x_ij；x_A1+x_A2 ≤ 50（或 =50，若平衡）。  
> 2. 看 slack/影子价格：slack=0 或 shadow price≠0 即 binding。  
> 3. x−3 ≥ 2 或 x−3 ≤ −2 → **x ≥ 5 或 x ≤ 1**。  
> 4. 令 bₙ=aₙ+1 → bₙ=2bₙ₋₁, b₁=2 → **aₙ=2ⁿ−1**。  
> 5. normative：为被接受而顺从；informational：认为别人信息更准。  
> 6. 最后一次 i=len−1 时 `lst[i+1]` 越界 → IndexError；改为 `range(len(lst)-1)`。  
> 7. 退出块时自动关闭文件，异常时也能关闭。

## M7 · 12/06

1. **MKT3601** Essay 结构：thesis 之外还需要哪两块？
2. **MKT3601** Three points of SOE reform.
3. **MKT3603** What is a brand community and how does it influence purchase?
4. **MKT3603** Mental accounting — one example.
5. **CB2203** Given μ=10/h and Wq=0.4h, find W.
6. **CB2240** Write pseudocode for word frequency counting.
7. **MKT3601** How does sustainability connect to consumer market outcomes?

> [!success]- 答案 M7
> 1. **claims（3 个）+ evidence（案例/数据）**；结尾重申立场。  
> 2. 产权多元化/混合所有制；市场化激励与考核；去产能与效率提升。  
> 3. 共享品牌认同的群体（仪式、符号、交流）；提供归属与信息，强化忠诚。  
> 4. 把 2000 元奖金放进“娱乐账户”更容易花掉。  
> 5. W = Wq + 1/μ = 0.4 + 0.1 = **0.5 h**。  
> 6. 打开文件 → 逐行 split → 小写去标点 → `counts[w]+=1` → 返回 dict。  
> 7. 绿色消费/ESG 偏好改变需求结构，合规成本改变供给，双向影响。

## M8 · 12/09

1. **CB2203** Constraints x+y≤8, x+2y≤12. Which is binding at (4,4)?
2. **CB2203** Shadow price 15, extra hour costs 10 — accept? Why?
3. **GE** Solve 2sin²x − 1 = 0 for 0 ≤ x ≤ 2π.
4. **GE** A 3×3 linear system has no solution when…
5. **MKT3603** JND and Weber’s law in one line.
6. **MKT3601** KOL vs KOC: reach and trust.

> [!success]- 答案 M8
> 1. x+y=8（binding）；x+2y=12 也等（12=12）→ 两个都 binding。  
> 2. 接受：净收益 15−10=+5>0（在 shadow price 有效范围内）。  
> 3. sin²x=1/2 → sin x=±√2/2 → x=π/4, 3π/4, 5π/4, 7π/4。  
> 4. 消元后出现 0=非零常数（矛盾行），即 rank(A) < rank([A|b])。  
> 5. 可察觉的最小差异随刺激强度成比例（Weber: ΔS/S=k）。  
> 6. KOL：覆盖广、信任较弱；KOC：覆盖小、信任强、转化高。

## M9 · 12/12（GE 六 slot 全扫）

1. **DR** Domain of √(4−x²).
2. **EXACT** Solve 2cos²x−cosx−1=0 on [0,2π].
3. **GAUSS** Solve x+y+z=6, 2x−y+z=3, x+2y−z=2.
4. **AMGM/VIETA** Min of x+4/x (x>0); α²+β² for roots of x²−5x+6.
5. **IND/RECUR** Σ(2k−1)=n² proof idea; solve aₙ=3aₙ₋₁+2, a₁=1.
6. **COUNT** 6 people, A/B not adjacent; 3-digit even from {1..5}.

> [!success]- 答案 M9
> 1. 4−x² ≥ 0 → **[−2,2]**。  
> 2. 0, 2π/3, 4π/3, 2π。  
> 3. x=1, y=2, z=3。  
> 4. 4 at x=2；13。  
> 5. 归纳用 k²+(2k+1)=(k+1)²；aₙ=2·3^{n−1}−1。  
> 6. 480；24。

## M10 · 12/15

1. **CB2240** Output:
```python
s = 0
for i in range(3):
    for j in range(2):
        s += i*j
print(s)
```
2. **CB2240** Write class `Account` withdraw rule in 3 lines.
3. **CB2240** Why `with open` better than `f=open`?
4. **MKT3601** Case 五问是哪五类？
5. **MKT3603** A shopper picks the middle subscription — which effect?
6. **MKT3603** “My watch defines me” — which concept?
7. **MKT3601** One-line thesis for SOE + sustainability essay.

> [!success]- 答案 M10
> 1. i=0→0；i=1: j=0,1 → 0+1=1；i=2: 0+2=2 → **3**。  
> 2. `if amount > self.balance: raise ValueError(...)`；否则 `self.balance -= amount`。  
> 3. 自动关闭、异常安全、代码短。  
> 4. 细分/定位、进入模式与 issue、去风险、全球-本地标准、KOL/渠道。  
> 5. compromise effect。  
> 6. extended self。  
> 7. 例：“SOE 改革与可持续不是两件事，而是同一套激励与问责机制的两面。”
