## Day 7: Review, Consolidation & Final Assessment

---

### Welcome to the final day

You made it. Seven days ago you knew how to count. Today you understand the entire Real Number system — one of the most fundamental structures in all of mathematics.

Before we assess what you know, let's do one complete, slow walkthrough of everything we covered this week. Read every section carefully. This is your last chance to fill any gaps before the assessment.

---

### The complete story of this week

We built the real number system the same way mathematicians built it historically — by asking questions that the current system could not answer.

| Day | Question we asked | New set we built | Symbol |
|-----|-------------------|------------------|--------|
| 1 | What numbers do we use to count? | Natural Numbers | ℕ |
| 1 | What if we need zero? | Whole Numbers | 𝕎 |
| 2 | What if we need less than zero? | Integers | ℤ |
| 3 | What if we need the space between integers? | Rational Numbers | ℚ |
| 4 | What if even fractions are not enough? | Irrational Numbers | — |
| 5 | What is the name for all of these combined? | Real Numbers | ℝ |

Each new set contained everything before it, plus something new. That is the nesting doll structure we have been building all week.

---

### Master reference — every set defined

### Natural Numbers (ℕ)

$$\mathbb{N} = \{1, 2, 3, 4, 5, \ldots\}$$

- Counting numbers starting at 1
- No zero, no negatives, no fractions
- Go on forever to the right
- Examples: 1, 7, 100, 1000000

### Whole Numbers (𝕎)

$$\mathbb{W} = \{0, 1, 2, 3, 4, \ldots\}$$

- Identical to ℕ but with zero added
- The only difference between ℕ and 𝕎 is the single number 0
- Examples: 0, 1, 7, 100

### Integers (ℤ)

$$\mathbb{Z} = \{\ldots, -3, -2, -1, 0, 1, 2, 3, \ldots\}$$

- All whole numbers plus their negatives
- Three dots on both sides — infinite in both directions
- Examples: −100, −7, −1, 0, 1, 7, 100

### Rational Numbers (ℚ)

$$\mathbb{Q} = \left\{ \frac{p}{q} \mid p, q \in \mathbb{Z},\ q \neq 0 \right\}$$

- Any number expressible as a fraction of two integers
- In decimal form: always terminates OR repeats
- Every integer is rational (n = n/1)
- Examples: 1/2, −3/4, 0.75, 0.333..., −8, 0

### Irrational Numbers

- Cannot be written as p/q for any integers p, q
- In decimal form: non-terminating AND non-repeating
- Completely separate from ℚ — no overlap
- Examples: √2, √3, √5, π, e, φ

### Real Numbers (ℝ)

$$\mathbb{R} = \mathbb{Q} \cup \{\text{irrationals}\}$$

- The union of all rationals and all irrationals
- Every point on the number line is a real number
- No gaps, no holes — the line is complete
- Contains every number from all five sets above

---

### The complete subset chain

$$\mathbb{N} \subset \mathbb{W} \subset \mathbb{Z} \subset \mathbb{Q} \subset \mathbb{R}$$

And separately, irrationals are a subset of ℝ but share no members with ℚ:

$$\mathbb{Q} \cap \{\text{irrationals}\} = \emptyset$$

---

### The classification diagram

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
│  │  │  ..., −2, −1          │   │                       │
│  │  └───────────────────────┘   │                       │
│  │  + fractions & decimals      │                       │
│  │  1/2, −3/4, 0.333...         │                       │
│  └──────────────────────────────┘                       │
└─────────────────────────────────────────────────────────┘
```

---

### The six properties of real numbers — quick reference

| Property | Addition | Multiplication |
|----------|----------|----------------|
| **Closure** | a + b ∈ ℝ | a × b ∈ ℝ |
| **Commutativity** | a + b = b + a | a × b = b × a |
| **Associativity** | (a+b)+c = a+(b+c) | (a×b)×c = a×(b×c) |
| **Distributivity** | a×(b+c) = a×b + a×c | — |
| **Identity** | a + 0 = a | a × 1 = a |
| **Inverse** | a + (−a) = 0 | a × (1/a) = 1, a ≠ 0 |

> Commutativity and Associativity do **NOT** apply to subtraction or division.
> Zero has **NO** multiplicative inverse — division by zero is undefined.

---

### The master classification table

Use this as your final reference. For any number, tick every column that applies:

| Number | ℕ | 𝕎 | ℤ | ℚ | Irrational | ℝ |
|--------|---|---|---|---|-----------|---|
| 1 | ✅ | ✅ | ✅ | ✅ | ❌ | ✅ |
| 0 | ❌ | ✅ | ✅ | ✅ | ❌ | ✅ |
| −4 | ❌ | ❌ | ✅ | ✅ | ❌ | ✅ |
| 3/7 | ❌ | ❌ | ❌ | ✅ | ❌ | ✅ |
| 0.6̄ | ❌ | ❌ | ❌ | ✅ | ❌ | ✅ |
| √4 = 2 | ✅ | ✅ | ✅ | ✅ | ❌ | ✅ |
| √3 | ❌ | ❌ | ❌ | ❌ | ✅ | ✅ |
| π | ❌ | ❌ | ❌ | ❌ | ✅ | ✅ |
| −2/5 | ❌ | ❌ | ❌ | ✅ | ❌ | ✅ |
| 1000 | ✅ | ✅ | ✅ | ✅ | ❌ | ✅ |

> Every number in this table has ✅ under ℝ. That will always be true for any real number — ℝ contains everything.

---

### The top 10 misconceptions of the week

These are the mistakes that appear most often. Read each one carefully and make sure you are not carrying any of them into the assessment.

**Misconception 1:** "Zero is a natural number."
→ Zero is in 𝕎 and ℤ and ℚ and ℝ — but NOT in ℕ. Natural numbers start at 1.

**Misconception 2:** "Negative numbers are whole numbers."
→ Whole numbers are {0, 1, 2, 3, ...}. Negative numbers first appear in ℤ — not before.

**Misconception 3:** "−7 is bigger than −3 because 7 > 3."
→ On the number line, further right = bigger. −3 is to the right of −7, so −3 > −7.

**Misconception 4:** "0.333... is approximately 1/3."
→ They are exactly equal. 0.333... = 1/3. A repeating decimal is not an approximation.

**Misconception 5:** "√9 is irrational because it has a square root sign."
→ Always simplify first. √9 = 3, which is a natural number — the most rational number possible.

**Misconception 6:** "22/7 = π."
→ 22/7 ≈ 3.142857... It is a rational approximation of π. They are not equal. π is irrational.

**Misconception 7:** "A number can only belong to one set."
→ The sets are nested. The number 5 belongs to ℕ, 𝕎, ℤ, ℚ, and ℝ simultaneously.

**Misconception 8:** "Irrational means impossible or not real."
→ Irrational simply means not expressible as a ratio. Irrationals are perfectly real — they live on the number line.

**Misconception 9:** "Subtraction is commutative — just like addition."
→ 8 − 3 = 5 but 3 − 8 = −5. These are different. Only addition and multiplication are commutative.

**Misconception 10:** "Zero has a multiplicative inverse of zero."
→ 0 × 0 = 0, not 1. Zero has no multiplicative inverse — it is the only real number without one.

---

### Final assessment

This assessment covers all seven days of learning. Work through each section carefully. Show your reasoning where asked.

---

### Section A — Classification (20 marks)

Classify each number below. For each one, list **every set it belongs to** from: ℕ, 𝕎, ℤ, ℚ, Irrational, ℝ.

**(2 marks each)**

1. 15
2. −6
3. 0
4. 7/8
5. √49
6. −√2
7. 0.121212...
8. 4.5
9. −3/1
10. √20

---

### Section A — Answers

| # | Number | Sets |
|---|--------|------|
| 1 | 15 | ℕ, 𝕎, ℤ, ℚ, ℝ |
| 2 | −6 | ℤ, ℚ, ℝ |
| 3 | 0 | 𝕎, ℤ, ℚ, ℝ |
| 4 | 7/8 | ℚ, ℝ |
| 5 | √49 = 7 | ℕ, 𝕎, ℤ, ℚ, ℝ |
| 6 | −√2 | Irrational, ℝ |
| 7 | 0.121212... | ℚ, ℝ (= 12/99 = 4/33, repeating) |
| 8 | 4.5 | ℚ, ℝ (= 9/2, terminating) |
| 9 | −3/1 = −3 | ℤ, ℚ, ℝ |
| 10 | √20 = 2√5 | Irrational, ℝ |

---

### Section B — True or False (10 marks)

State whether each statement is **True** or **False**. If false, correct it in one sentence.

**(1 mark each)**

1. Every integer is a rational number.
2. Every rational number is an integer.
3. Zero is a natural number.
4. π = 22/7
5. The decimal 0.454545... is irrational.
6. √16 is irrational.
7. Between any two real numbers there is always another real number.
8. Subtraction of real numbers is commutative.
9. The multiplicative identity is 1.
10. Every real number is either rational or irrational, but not both.

---

### Section B — Answers

| # | Statement | Answer |
|---|-----------|--------|
| 1 | Every integer is rational | **True** — n = n/1 for any integer |
| 2 | Every rational is an integer | **False** — e.g. 1/2 is rational but not an integer |
| 3 | Zero is a natural number | **False** — zero is in 𝕎 but not in ℕ |
| 4 | π = 22/7 | **False** — 22/7 is a rational approximation; π is irrational |
| 5 | 0.454545... is irrational | **False** — it repeats (45 repeats), so it is rational = 45/99 = 5/11 |
| 6 | √16 is irrational | **False** — √16 = 4, a natural number |
| 7 | Between any two reals there is another | **True** — this is the density property |
| 8 | Subtraction is commutative | **False** — 8−3 = 5 but 3−8 = −5 |
| 9 | Multiplicative identity is 1 | **True** — a × 1 = a for all a ∈ ℝ |
| 10 | Every real is rational or irrational, not both | **True** — ℚ and irrationals never overlap |

---

### Section C — Properties (15 marks)

Name the property demonstrated in each statement.

**(2 marks each)**

1. 7 + 3 = 3 + 7
2. (2 × 5) × 4 = 2 × (5 × 4)
3. 6 × (3 + 4) = 6 × 3 + 6 × 4
4. −√5 + √5 = 0
5. 99 × 1 = 99
6. (8 + 1) + 9 = 8 + (1 + 9)
7. 3/4 × 4/3 = 1 *(1 mark — name the property AND state what type of inverse)*

---

### Section C — Answers

| # | Statement | Property |
|---|-----------|----------|
| 1 | 7 + 3 = 3 + 7 | **Commutative property of addition** |
| 2 | (2×5)×4 = 2×(5×4) | **Associative property of multiplication** |
| 3 | 6×(3+4) = 6×3 + 6×4 | **Distributive property** |
| 4 | −√5 + √5 = 0 | **Additive inverse property** |
| 5 | 99 × 1 = 99 | **Multiplicative identity property** |
| 6 | (8+1)+9 = 8+(1+9) | **Associative property of addition** |
| 7 | 3/4 × 4/3 = 1 | **Multiplicative inverse property** — 4/3 is the reciprocal of 3/4 |

---

### Section D — Short answer (15 marks)

**(3 marks each)**

1. Explain in your own words why √2 is irrational. You do not need to write the full proof — just explain the key idea in 2 or 3 sentences.

2. A student writes: "0.999... is less than 1 because it never quite reaches 1." Is the student correct? Explain why or why not.

3. Give an example of a real-world measurement that would produce an irrational number. Explain why it is irrational.

4. What is the difference between the **density** property and the **completeness** property of ℝ? Use one sentence for each.

5. Place these numbers in the correct order from least to greatest, then identify which set each one belongs to:
$$-\sqrt{3}, \quad 0, \quad \frac{1}{2}, \quad -2, \quad \pi, \quad 1$$

---

### Section D — Answers

**Question 1:**
√2 is irrational because it cannot be written as a fraction p/q where p and q are integers. When you compute √2 on a calculator, the decimal goes on forever without ever repeating a pattern. Any number whose decimal is non-terminating and non-repeating cannot be expressed as a fraction, which is the definition of irrational.

**Question 2:**
The student is incorrect. 0.999... is exactly equal to 1 — not approximately, but precisely. One way to see this: let x = 0.999..., then 10x = 9.999..., subtract to get 9x = 9, so x = 1. The notation 0.999... represents the limit of an infinite process that converges exactly to 1.

**Question 3:**
Many valid answers. Example: the circumference of a circle with diameter 1 metre is exactly π metres. Since π is irrational — its decimal never terminates and never repeats — the circumference is irrational. No fraction, however precise, can capture its exact value.

**Question 4:**
Density means that between any two real numbers there is always another real number — there is no "next" number after any given one. Completeness means that the real number line has no gaps or holes — every point on the line corresponds to exactly one real number.

**Question 5:**

Order from least to greatest:

$$-2 \quad < \quad -\sqrt{3} \approx -1.732 \quad < \quad 0 \quad < \quad \frac{1}{2} \quad < \quad 1 \quad < \quad \pi \approx 3.14159$$

| Number | Classification |
|--------|----------------|
| −2 | ℤ, ℚ, ℝ |
| −√3 | Irrational, ℝ |
| 0 | 𝕎, ℤ, ℚ, ℝ |
| 1/2 | ℚ, ℝ |
| 1 | ℕ, 𝕎, ℤ, ℚ, ℝ |
| π | Irrational, ℝ |

---

### How did you do? — Marking guide

| Score | Out of | Percentage | What it means |
|-------|--------|------------|---------------|
| 54–60 | 60 | 90–100% | Excellent — you have mastered the Real Number system |
| 42–53 | 60 | 70–89% | Strong — review the sections where you lost marks |
| 30–41 | 60 | 50–69% | Developing — revisit Days 3, 4, and 5 in particular |
| Below 30 | 60 | Below 50% | Go back to Day 1 and work through the week again slowly |

---

### Week summary — the complete picture

You started this week knowing how to count. You end it understanding the architecture of the entire real number system. Here is everything you built:

```
Week 1 journey:

Day 1:  ℕ = {1, 2, 3, ...}              "I can count things"
        𝕎 = {0, 1, 2, 3, ...}          "I can include nothing"

Day 2:  ℤ = {..., −1, 0, 1, ...}        "I can go below zero"

Day 3:  ℚ = {p/q | q ≠ 0}               "I can live between integers"

Day 4:  Irrationals = {√2, π, e, ...}   "I cannot be caught by any fraction"

Day 5:  ℝ = ℚ ∪ {irrationals}           "I am every point on the number line"

Day 6:  Properties of ℝ                  "I understand how these numbers behave"

Day 7:  Classification mastery           "I can identify any real number"
```

And the complete chain:

$$\mathbb{N} \subset \mathbb{W} \subset \mathbb{Z} \subset \mathbb{Q} \subset \mathbb{R}$$

---

### What comes next?

The Real Number system is the foundation for everything that follows in your mathematics education:

- **Algebra** — solving equations using real numbers and their properties
- **Geometry** — lengths, areas, and angles are all real numbers (many irrational)
- **Trigonometry** — sin, cos, tan produce real number outputs
- **Calculus** — built entirely on the completeness of ℝ
- **Statistics** — every data value is a real number
- **Complex Numbers** — the next frontier, extending ℝ by introducing i = √−1

You now have the foundation. Everything else builds on what you learned this week.

---

### A final thought

When the ancient Greeks discovered that √2 could not be written as a fraction, it shook their entire understanding of mathematics. They had believed that all numbers were rational — that the universe was built from simple ratios. That discovery forced them to expand their idea of what a number could be.

That same spirit of expansion drove everything we did this week. Every time we hit a wall — zero, negative numbers, fractions, square roots of non-perfect squares — we did not say "impossible." We said "let's build something bigger."

That is what mathematics is. Not a fixed set of rules to memorise, but a living, growing language for describing the world. You are now part of that tradition.

Well done for completing the course. 😊
