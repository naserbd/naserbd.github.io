## Day 5: The Full Picture — Real Numbers & Classification

---

### Quick recap from Days 1 through 4

We have built our number system piece by piece. Let's look at everything we have so far:

| Set | Symbol | Members | What was added |
|-----|--------|---------|----------------|
| Natural Numbers | ℕ | 1, 2, 3, 4, ... | The original counting numbers |
| Whole Numbers | 𝕎 | 0, 1, 2, 3, ... | Added zero |
| Integers | ℤ | ..., −2, −1, 0, 1, 2, ... | Added the negatives |
| Rational Numbers | ℚ | All fractions p/q (q ≠ 0) | Added fractions and decimals |
| Irrational Numbers | — | √2, π, e, √3, φ, ... | Non-terminating, non-repeating decimals |

Yesterday I left you with this question:

> *Is there a name for the set of ALL numbers on the number line — both rational and irrational combined?*

Today we answer that. And with it, we complete the entire picture of numbers you will use throughout high school mathematics.

---

### The missing piece

Look at our number line right now:

```
←────────────────────────────────────────────────→
    ...  −2   −1    0    1   √2   2    π    3  ...
                              ↑        ↑
                          irrational  irrational
```

Every single point on that line — every possible location, no matter how precise — represents a number. Some of those points are rational. Some are irrational. But together, they cover the **entire line** without leaving a single gap.

That complete, gapless collection of every number on the number line has a name:

$$\text{The Real Numbers} \quad \mathbb{R}$$

---

### Defining the Real Numbers

The **Real Numbers (ℝ)** is the set of all numbers that can be placed on a number line. It includes:

- Every natural number
- Every whole number
- Every integer
- Every rational number
- Every irrational number

In other words:

$$\mathbb{R} = \mathbb{Q} \cup \{\text{irrationals}\}$$

Read that as: "ℝ equals the union of the rationals and the irrationals."

The rationals and irrationals together fill every single point on the number line — there are no gaps, no holes, no missing points. Mathematicians call this the **completeness** of the real numbers.

> **Why "real"?** The name distinguishes these numbers from *imaginary* numbers (like √−1), which we do not cover in this course but exist in higher mathematics. For everything you will do in high school, real numbers are the complete universe of numbers.

---

### The complete classification hierarchy

This is the most important diagram of the entire week. Study it carefully.

```
┌─────────────────────────────────────────────────────────┐
│                    Real Numbers (ℝ)                     │
│                                                         │
│  ┌──────────────────────────────┐  ┌──────────────────┐ │
│  │     Rational Numbers (ℚ)     │  │   Irrational     │ │
│  │                              │  │   Numbers        │ │
│  │  ┌───────────────────────┐   │  │                  │ │
│  │  │     Integers (ℤ)      │   │  │  √2, √3, √5      │ │
│  │  │                       │   │  │  π, e, φ         │ │
│  │  │  ┌─────────────────┐  │   │  │  √7, √11, ...    │ │
│  │  │  │  Whole Nos. 𝕎  │  │   │  │                  │ │
│  │  │  │                 │  │   │  └──────────────────┘ │
│  │  │  │  ┌───────────┐  │  │   │                       │
│  │  │  │  │  Natural  │  │  │   │                       │
│  │  │  │  │  Nos. ℕ   │  │  │   │                       │
│  │  │  │  │  1,2,3,...│  │  │   │                       │
│  │  │  │  └───────────┘  │  │   │                       │
│  │  │  │  + { 0 }        │  │   │                       │
│  │  │  └─────────────────┘  │   │                       │
│  │  │  + negatives          │   │                       │
│  │  │  ..−2, −1             │   │                       │
│  │  └───────────────────────┘   │                       │
│  │  + fractions, decimals       │                       │
│  │  1/2, −3/4, 0.75, 0.333...   │                       │
│  └──────────────────────────────┘                       │
└─────────────────────────────────────────────────────────┘
```

Read this diagram from the **inside out**:

1. Start with ℕ — the smallest set — sitting in the very centre
2. 𝕎 wraps around it, adding zero
3. ℤ wraps around that, adding the negatives
4. ℚ wraps around that, adding all fractions and repeating/terminating decimals
5. On the right side, completely separate from ℚ, sit the irrationals
6. ℝ is the outermost boundary — it contains everything

---

### The complete subset chain

We can now write the full relationship between all our sets:

$$\mathbb{N} \subset \mathbb{W} \subset \mathbb{Z} \subset \mathbb{Q} \subset \mathbb{R}$$

And separately:

$$\text{Irrationals} \subset \mathbb{R}$$

Two critical points about this chain:

**Point 1:** Every arrow goes one way only. Just because 5 is in ℕ does not mean every member of ℚ is in ℕ. The subset relationship is one-directional.

**Point 2:** ℚ and the irrationals do not overlap. A number is either rational or irrational — never both. They are two completely separate regions inside ℝ.

---

### How to classify any real number

Classifying a number means identifying **every set it belongs to**. A number can belong to multiple sets at the same time — remember the nesting dolls.

Here is the decision process to follow every time:

```
Given a number — ask these questions in order:

1. Is it a positive whole number (no zero, no decimals, no negatives)?
   YES → it is in ℕ (and also in 𝕎, ℤ, ℚ, and ℝ)

2. Is it zero?
   YES → it is in 𝕎 (and also in ℤ, ℚ, and ℝ) but NOT in ℕ

3. Is it a negative whole number?
   YES → it is in ℤ (and also in ℚ and ℝ) but NOT in ℕ or 𝕎

4. Is it a fraction, terminating decimal, or repeating decimal?
   YES → it is in ℚ (and ℝ) but NOT in ℤ, 𝕎, or ℕ

5. Is it non-terminating and non-repeating (like √2, π, e)?
   YES → it is irrational — in ℝ only, not in ℚ, ℤ, 𝕎, or ℕ
```

---

### Worked classification examples

Let's classify several numbers together, step by step.

### Example 1 — Classify 7

- Is 7 a positive whole number? **Yes**
- Therefore: 7 ∈ ℕ, 7 ∈ 𝕎, 7 ∈ ℤ, 7 ∈ ℚ, 7 ∈ ℝ
- Sets it belongs to: **ℕ, 𝕎, ℤ, ℚ, ℝ** — all five

### Example 2 — Classify 0

- Is 0 a positive whole number? No
- Is it zero? **Yes**
- Therefore: 0 ∈ 𝕎, 0 ∈ ℤ, 0 ∈ ℚ, 0 ∈ ℝ
- Sets it belongs to: **𝕎, ℤ, ℚ, ℝ** — not ℕ

### Example 3 — Classify −5

- Is −5 positive? No. Is it zero? No.
- Is it a negative whole number? **Yes**
- Therefore: −5 ∈ ℤ, −5 ∈ ℚ, −5 ∈ ℝ
- Sets it belongs to: **ℤ, ℚ, ℝ** — not ℕ, not 𝕎

### Example 4 — Classify 3/4

- Is 3/4 a whole number? No. Is it an integer? No.
- Can it be written as p/q with integers p and q, q ≠ 0? **Yes** (p = 3, q = 4)
- Therefore: 3/4 ∈ ℚ, 3/4 ∈ ℝ
- Sets it belongs to: **ℚ, ℝ** — not ℕ, 𝕎, or ℤ

### Example 5 — Classify √2

- Is √2 a whole number? No. An integer? No. A fraction? No.
- Is its decimal non-terminating and non-repeating? **Yes** (1.41421356...)
- Therefore: √2 is irrational, √2 ∈ ℝ
- Sets it belongs to: **ℝ only** (and the set of irrationals)

### Example 6 — Classify −2/3

- Is −2/3 a whole number? No. An integer? No.
- Can it be written as p/q? **Yes** (p = −2, q = 3)
- Therefore: −2/3 ∈ ℚ, −2/3 ∈ ℝ
- Sets it belongs to: **ℚ, ℝ**

### Example 7 — Classify √9

- √9 = 3. Now classify 3.
- 3 is a positive whole number.
- Sets it belongs to: **ℕ, 𝕎, ℤ, ℚ, ℝ** — all five
- Watch out: even though it started as a square root, simplify first!

---

### The number line — the complete picture

Here is the complete real number line, showing where different types of numbers live:

```
←─────┬────┬────┬────┬────┬────┬────┬────┬────┬────┬────┬───────→
     −π   −√3  −2   −1  −1/2   0   1/2   1    √2   2    π
      ↑    ↑    ↑    ↑    ↑    ↑    ↑    ↑     ↑   ↑    ↑
     irr  irr  int  int  rat  int  rat  int   irr int  irr
```

Notice how rational and irrational numbers are completely interleaved — between any two real numbers of any kind, you can always find both rationals and irrationals.

---

### Every real number has a decimal expansion

One of the defining properties of ℝ is that every real number can be expressed as a decimal — it just might be infinite.

| Number | Decimal expansion | Type |
|--------|-------------------|------|
| 3 | 3.000000... | Rational (terminating) |
| 1/3 | 0.333333... | Rational (repeating) |
| 5/11 | 0.454545... | Rational (repeating) |
| √2 | 1.41421356... | Irrational |
| π | 3.14159265... | Irrational |
| −7/4 | −1.75000... | Rational (terminating) |

The decimal either terminates, repeats, or goes on forever without repeating. Those are the only three possibilities — and they map exactly onto rational, rational, and irrational respectively.

---

### Summary of the complete classification

| Number | ℕ | 𝕎 | ℤ | ℚ | Irrational | ℝ |
|--------|---|---|---|---|-----------|---|
| 8 | ✅ | ✅ | ✅ | ✅ | ❌ | ✅ |
| 0 | ❌ | ✅ | ✅ | ✅ | ❌ | ✅ |
| −3 | ❌ | ❌ | ✅ | ✅ | ❌ | ✅ |
| 2/5 | ❌ | ❌ | ❌ | ✅ | ❌ | ✅ |
| √5 | ❌ | ❌ | ❌ | ❌ | ✅ | ✅ |
| π | ❌ | ❌ | ❌ | ❌ | ✅ | ✅ |
| −√9 | ❌ | ❌ | ✅ | ✅ | ❌ | ✅ |
| 0.7̄ | ❌ | ❌ | ❌ | ✅ | ❌ | ✅ |

> Notice: every single number in the table has ✅ under ℝ. That is the point — ℝ contains everything.

---

### Common mistakes — don't fall for these!

**Mistake 1:** "A number can only belong to one set."
→ Wrong. The sets are nested. The number 5 belongs to ℕ, 𝕎, ℤ, ℚ, and ℝ all at the same time.

**Mistake 2:** "Irrational numbers are not real."
→ Wrong. Irrational numbers are absolutely real — they have precise locations on the number line. The word "real" in mathematics does not mean the opposite of "fake."

**Mistake 3:** "√9 is irrational because it has a square root sign."
→ Wrong. Always simplify first. √9 = 3, which is a natural number — as rational as it gets.

**Mistake 4:** "ℚ and irrationals overlap somewhere."
→ They never overlap. A number is rational or irrational — never both. This is not a grey area.

**Mistake 5:** "ℝ is the same as ℚ."
→ No. ℚ is a proper subset of ℝ. The irrationals are in ℝ but not in ℚ. ℝ is strictly larger.

---

### Try yourself

Classify each number below — list every set it belongs to (ℕ, 𝕎, ℤ, ℚ, irrational, ℝ):

1. 12
2. −9
3. 5/6
4. √16
5. −√7
6. 0.252525...
7. 0
8. −4/1
9. √50
10. e

---

### Answers

| # | Number | Classification |
|---|--------|----------------|
| 1 | 12 | ℕ, 𝕎, ℤ, ℚ, ℝ |
| 2 | −9 | ℤ, ℚ, ℝ |
| 3 | 5/6 | ℚ, ℝ |
| 4 | √16 = 4 | ℕ, 𝕎, ℤ, ℚ, ℝ |
| 5 | −√7 | Irrational, ℝ |
| 6 | 0.252525... | ℚ, ℝ (repeating decimal = 25/99) |
| 7 | 0 | 𝕎, ℤ, ℚ, ℝ |
| 8 | −4/1 = −4 | ℤ, ℚ, ℝ |
| 9 | √50 = 5√2 | Irrational, ℝ |
| 10 | e | Irrational, ℝ |

---

### Homework

Draw the **complete classification hierarchy** from memory — the nested diagram with all five sets labelled. Include at least **two example numbers** placed inside each region.

Then answer this question in two or three sentences:

> *Why is it important that ℚ and the irrationals do not overlap? What would happen to our number system if a number could be both rational and irrational at the same time?*

---

### Something to think about tonight...

We now have the complete Real Number system. Every number you have ever used in your life — every measurement, every calculation, every score — is a real number.

But here is something worth noticing. We built this entire system by asking one simple question at each stage:

- "What if I need to count things?" → ℕ
- "What if I need zero?" → 𝕎
- "What if I need less than zero?" → ℤ
- "What if I need the space between integers?" → ℚ
- "What if even fractions aren't enough?" → Irrationals → ℝ

Each question revealed a gap. Each gap demanded a new kind of number.

So here is your final question for tonight:

> *What if I need the square root of a negative number? For example, what is √−1? Is there a number for that?*

Try it on your calculator. It will say **ERROR** or **undefined**.

