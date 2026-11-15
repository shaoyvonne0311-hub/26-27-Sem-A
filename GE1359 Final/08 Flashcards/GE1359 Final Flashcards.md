---
tags: [flashcards, GE1359]
updated: 2026-11-06
---
# 🃏 GE1359 Final Flashcards
> [!tip] How to use
> - **Inside Obsidian:** install the community plugin *Spaced Repetition*. Each `question :: answer` line becomes a card; the `#flashcards/GE1359/<topic>` headings below are the decks.
> - **Without the plugin:** cover the right side and say the answer aloud.
> - **Ali's rules:** recall *before* you reveal; one fact per card; mistakes from the [[Finals 2026/GE1359 Final/07 Mistakes/Mistake Log|Mistake Log]] become new cards.
> - **Ch1–Ch3 cards** stay in the midterm deck: [[GE1359 Revision Vault/08 Flashcards/GE1359 Flashcards|GE1359 Flashcards]] (not copied). This deck only adds the final-exam chapters.

## #flashcards/GE1359/Ch3
**AM-GM**: State the AM-GM inequality for two positive numbers and when equality holds. :: (a+b)/2 ≥ √(ab) for a, b > 0; equality iff a = b.
**Linear system outcomes**: After row-reducing, how do you see unique / no / infinitely many solutions? :: Unique: a pivot in every variable column. None: a row 0 = c (c ≠ 0). Infinitely many: consistent with a free variable (set it = t).
**Roots and coefficients (quadratic)**: For ax² + bx + c = 0 with roots α, β: α + β = ? αβ = ? :: α + β = −b/a ; αβ = c/a.

## #flashcards/GE1359/Ch4
**Induction: the 4 steps**: Write the class template for proof by mathematical induction. :: Let P(n) be … ① show P(1) true (L.H.S. = R.H.S.) ② assume P(k) true for some positive integer k ③ prove P(k+1) USING the assumption ④ 'By the principle of mathematical induction, P(n) is true for all positive integers n.'
**Induction starting at a**: What changes when the statement is for n ≥ a? :: Check P(a) first; assume P(k) for some integer k ≥ a; conclude 'for all integers n ≥ a'.
**Two-step induction**: When do you check P(1) AND P(2) and assume P(k−1), P(k)? :: When P(k+1) depends on the two previous terms (e.g. a recurrence aₙ₊₁ = f(aₙ, aₙ₋₁)).
**Proof by contradiction**: Opening and closing lines? :: 'Assume (the opposite) …' → derive a contradiction → 'Therefore our assumption is wrong, so …'.

## #flashcards/GE1359/Ch5
**nPr and n!**: Formula for arranging r of n distinct objects? What is 0!? :: nPr = n!/(n−r)! ; 0! = 1.
**Repeated letters**: Arrangements of all letters of a word with repeats (e.g. p of one letter, q of another)? :: n!/(p! q! …).
**nCr identities**: Two identities from the Theorem on p.21. :: nCr = nC(n−r) ; nCr + nC(r−1) = (n+1)Cr.
**At least one**: Number of ways to choose at least one of n different things? :: 2ⁿ − 1.
**Binomial general term**: General term of (a + b)ⁿ? :: T(r+1) = nCr · a^(n−r) · b^r, r = 0, 1, …, n.
**Coefficient / constant term**: How do you find the term independent of x? :: Write the general term, collect the power of x, set it to 0 (or to the power you need), solve for r.
**Sum of binomial coefficients**: Σ nCr = ? Even-indexed sum = ? :: 2ⁿ (put a = b = 1). Even = odd = 2ⁿ⁻¹ (put a = 1, b = −1).
