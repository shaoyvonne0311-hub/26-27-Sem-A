---
tags: [finals, GE1359, playbook]
updated: 2026-11-06
---
# ➕ Final additions: Ch3 remainder, Ch4, Ch5

> [!abstract] How this fits with the midterm guides
> The midterm guides stay where they are and still apply (Ch1–Ch3 p.1–35). **Linked, not copied:**
> - 📘 [[GE1359 Revision Vault/02 Guides/Question-Type Playbook|Question-Type Playbook]] (17 types)
> - 🧠 [[GE1359 Revision Vault/02 Guides/Memorise Sheet (NOT on formula sheet)|Memorise Sheet]]
> - ❌ [[GE1359 Revision Vault/07 Mistakes/Mistake Log|Mistake Log]] · 🧭 [[GE1359 Revision Vault/02 Guides/Revision Guide|Revision Guide]] · [[GE1359 Revision Vault/02 Guides/Past Paper Analysis|Past Paper Analysis]]
>
> This note adds the **new final-exam types** in the same format (Spot it · Write this · Check · Your traps). Fill "Your traps" from your Ch4–5 practice. Scope is provisional (Ch1–5) until the final scope is announced.
> Correction carried over: $\sin x=\sin\alpha \Rightarrow x=n\pi+(-1)^n\alpha$ (not "arcsin + nπ").

Sources: [[Finals 2026/GE1359 Final/09 Source PDFs/Lecture notes/GE1359_MA1502_2627A_Ch4.pdf|Ch4 notes]] · [[Finals 2026/GE1359 Final/09 Source PDFs/Lecture notes/GE1359_MA1502_2627A_Ch5.pdf|Ch5 notes]] · [[Finals 2026/GE1359 Final/09 Source PDFs/Lecture notes/GE1359_MA1502_2627A_Ch3.pdf|Ch3 notes (full)]]

---

## Ch3 · remainder (after p.35)

### 🆕 C3-REST · Inequalities (AM-GM), linear systems, theory of equations
**Spot it:** "Prove that … ≥ …" for positive numbers; "Solve the system … / for which k does it have no / infinitely many solutions"; "α, β, γ are roots of … find α² + β² + γ²".

**Write this:**
- *AM-GM:* state that the numbers are positive → $\frac{a+b}{2}\ge\sqrt{ab}$ → equality iff $a=b$.
- *Linear systems:* augmented matrix → row-echelon form (write each row operation) → read the case: unique / none ($0=c$) / infinitely many (free variable $=t$).
- *Theory of equations:* write the sum/product (pairs) relations first, then express the target in terms of them.

**Check:** substitute your solution back into every original equation.

**Your traps:** _(fill in after the Ch3 remainder drills on Thu 12 / Fri 13 Nov)_

---

## Ch4 · Mathematical induction

### 🆕 C4-IND · Prove by mathematical induction
**Spot it:** "Prove, by mathematical induction, that for all positive integers n …" (sums, inequalities, divisibility).

**Write this (class template, Ch4 p.9):**
1. *Let P(n) be* the statement.
2. **Step 1:** for $n=1$: L.H.S. $=\dots$, R.H.S. $=\dots$, so P(1) is true.
3. **Step 2:** *Assume P(k) is true for some positive integer k*, i.e. (write it out).
4. **Step 3:** When $n=k+1$: start from the L.H.S. of P(k+1), split off the last term, use the assumption (label it "by induction assumption"), simplify to the R.H.S.
5. **Step 4:** *By the principle of mathematical induction, P(n) is true for all positive integers n.*

**Variants:** start at $n=a$ (check P(a), assume $k\ge a$); two-step induction (check P(1), P(2); assume P(k−1) and P(k)); divisibility (write $P(k)$ as "= m·(divisor)" for an integer m).

**Also in Ch4:** proof by contradiction (√2 irrational; rational + irrational is irrational): "Assume …" → contradiction → "Therefore our assumption must be wrong."

**Check:** factorise the R.H.S. of P(k+1) yourself first, so you know the target while simplifying.

**Your traps:** _(fill in)_

---

## Ch5 · Binomial theorem and combinatorics

### 🆕 C5-COMB · Counting, permutations, combinations
**Spot it:** "In how many ways …", words with repeated letters, committees, "at least", "always together", "begin and end with".

**Write this:**
- Multiplication principle: $n_1 n_2\cdots n_k$.
- $^nP_r=\frac{n!}{(n-r)!}$ (order matters) · $^nC_r=\frac{n!}{r!(n-r)!}$ (order doesn't).
- Repeated letters: $\frac{n!}{p!\,q!\cdots}$. "Together": glue them into one block, then multiply by the block's internal arrangements. Fixed positions: fill those first.
- "At least one" of n things: $2^n-1$. Split "at least k" into cases or use the complement.

**Check:** does order matter? Is anything repeated? Did you count a case twice?

**Your traps:** _(fill in)_

### 🆕 C5-BIN · Binomial theorem
**Spot it:** "Find the coefficient of $x^5$ / the term independent of x in the expansion of …"; "first three terms are …, find a, b, n"; "evaluate $(1.01)^9$ to 6 d.p."

**Write this:**
1. General term $T_{r+1}={}^nC_r\,a^{n-r}b^r$.
2. Collect the power of x into one exponent (e.g. $x^{20-5r}$).
3. Set the exponent equal to what you need, solve for r (must be an integer $0\le r\le n$), substitute back.
- Sum of coefficients $=2^n$ ($a=b=1$); even-indexed $=$ odd-indexed $=2^{n-1}$ ($a=1,b=-1$).
- Approximation: expand $(1+x)^n$ and stop when terms are below the required accuracy.

**Check:** r is a non-negative integer ≤ n; signs of $(-b)^r$.

**Your traps:** _(fill in)_
