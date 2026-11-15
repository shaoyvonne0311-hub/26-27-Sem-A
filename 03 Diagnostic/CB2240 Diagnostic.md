---
tags: [finals, CB2240, diagnostic]
time: 45 min
marks: 38
updated: 2026-11-15
---

# CB2240 诊断卷 Diagnostic（45 min / 38 marks，纸笔）

> [!warning] 纸笔模式
> 不打开电脑。像考场一样手写代码；缩进用 4 个空格画清楚。

## Part A — 10 × 2 = 20 marks

**A1.** 
```python
total = 0
for i in range(1, 6):
    if i % 2 == 0:
        total += i * 2
    else:
        total -= i
print(total)
```
Output? **(LOOP)**

**A2.** 
```python
def f(a, b=2):
    return a * b + 1
print(f(3), f(3, 4))
```
Output? **(FUNC)**

**A3.** Which line is syntactically valid? **(SYN)**
A. `if x = 3:`　B. `for i in range(5)`　C. `while (x > 0):`　D. `def f(x): return x +`

**A4.** 
```python
x = 15
if x < 10:
    print("low")
elif x < 20:
    print("mid")
else:
    print("high")
```
Output? **(IF)**

**A5.** `s = "Python"`. What are `s[1:4]` and `s[::-1]`? **(STR)**

**A6.** 
```python
a = [1, 2, 3]
b = a
b.append(4)
print(a)
```
Output? **(LIST)**

**A7.** `d = {"a": 1}`. What is `d.get("b", 0)`? Then after `d["b"] = 2`, what is `len(d)`? **(DICT)**

**A8.** 
```python
class C:
    def __init__(self, x):
        self.x = x
    def bump(self):
        self.x += 1
c = C(5)
c.bump()
print(c.x)
```
Output? **(CLASS)**

**A9.** Find the bug: **(ERR)**
```python
def total(nums):
    s = 0
    for n in nums:
        s += n
    return s
print(total([1, 2, 3] + 4))
```

**A10.** `with open("data.txt") as f: n = sum(1 for line in f)`. What does `n` count? **(FILE)**

## Part B — 2 × 9 = 18 marks

**B1.** Write `word_count(path)` that reads a text file and returns a dict of lowercase word frequencies. Split on whitespace and strip punctuation `.,!?`. **(9)**

**B2.** Write class `Account` with `balance`, `deposit(amount)` and `withdraw(amount)`; withdraw raises `ValueError` if balance is insufficient. Show one成功 and one失败调用. **(9)**

## 交卷后
1. 对答案，按题号标 topic；写码两题按「能跑 / 边界 / 命名」三项扣分。
2. 填 Excel `07 诊断 Diagnostic`。

> [!success]- 答案（做完再看）
> A1 3 · A2 `7 13` · A3 C · A4 `mid` · A5 `"yth"` / `"nohtyP"` · A6 `[1,2,3,4]` · A7 `0`，len=2 · A8 6 · A9 调用 `[1,2,3]+4` → TypeError · A10 行数
> B1/B2 代码见《Diagnostic Answer Key》。
