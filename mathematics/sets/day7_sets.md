# Day 7 — Review, Proofs & Exam Prep

---

### What Day 7 Is About

Today is not a new topic — it is a **consolidation day**. The goal is to:

1. Review every symbol, definition, and formula from Days 1–6
2. Learn the two core proof techniques used in set theory
3. Spot and avoid the most common exam traps
4. Solve 15 mixed problems that span all six days
5. See how everything connects into one unified picture
6. Get a glimpse of what lies beyond — functions, infinite sets, and university mathematics

Take your time. If a question reveals a gap, go back to that day's notes before continuing.

---

### Part 1 — Master Symbol Reference (Days 1–6)

### Sets and membership

| Symbol | Meaning | Example |
|---|---|---|
| `{ }` | Curly braces — denotes a set | `A = {1, 2, 3}` |
| `∈` | Is an element of | `2 ∈ {1, 2, 3}` |
| `∉` | Is not an element of | `5 ∉ {1, 2, 3}` |
| `∅` or `{}` | The empty set — no elements | `∅` |
| `U` | The universal set | all relevant elements |
| `\|A\|` | Cardinality — number of elements in A | `\|{a,b,c}\| = 3` |

### Subsets and supersets

| Symbol | Meaning | Example |
|---|---|---|
| `A ⊆ B` | A is a subset of B (allows A = B) | `{1,2} ⊆ {1,2,3}` |
| `A ⊂ B` | A is a proper subset of B (A ≠ B) | `{1,2} ⊂ {1,2,3}` |
| `A ⊄ B` | A is not a subset of B | `{1,4} ⊄ {1,2,3}` |
| `A ⊇ B` | A is a superset of B | `{1,2,3} ⊇ {1,2}` |
| `P(A)` | Power set — all subsets of A | `P({a,b}) = {∅,{a},{b},{a,b}}` |

### Set operations

| Symbol | Meaning | Key word |
|---|---|---|
| `A ∪ B` | Union — in A or B or both | OR |
| `A ∩ B` | Intersection — in both A and B | AND |
| `A'` or `Aᶜ` | Complement — in U but not in A | NOT |
| `A − B` or `A \ B` | Set difference — in A but not in B | MINUS |
| `A △ B` | Symmetric difference — in A or B but not both | XOR |
| `A × B` | Cartesian product — all ordered pairs (a,b) | PAIR |

### Relations

| Symbol | Meaning |
|---|---|
| `(a, b)` | Ordered pair |
| `R ⊆ A × B` | R is a relation from A to B |
| `a R b` | a is related to b — i.e. `(a,b) ∈ R` |
| `Dom(R)` | Domain — all first components of pairs in R |
| `Ran(R)` | Range — all second components of pairs in R |

---

### Part 2 — Master Formula Reference (Days 1–6)

### Power set

```
|P(A)|  =  2^|A|
```

### Cardinality formulas

```
|A ∪ B|       =  |A| + |B| − |A ∩ B|
|A ∪ B ∪ C|   =  |A| + |B| + |C| − |A∩B| − |A∩C| − |B∩C| + |A∩B∩C|
|A'|           =  |U| − |A|
|A − B|        =  |A| − |A ∩ B|
|A △ B|        =  |A| + |B| − 2|A ∩ B|
|A × B|        =  |A| × |B|
```

### Laws of set algebra

```
Commutative:      A ∪ B = B ∪ A                A ∩ B = B ∩ A
Associative:      (A∪B)∪C = A∪(B∪C)           (A∩B)∩C = A∩(B∩C)
Distributive:     A∩(B∪C) = (A∩B)∪(A∩C)       A∪(B∩C) = (A∪B)∩(A∪C)
Identity:         A ∪ ∅ = A                     A ∩ U = A
Domination:       A ∪ U = U                     A ∩ ∅ = ∅
Idempotent:       A ∪ A = A                     A ∩ A = A
Complement:       A ∪ A' = U                    A ∩ A' = ∅
Double complement:(A')' = A
De Morgan 1:      (A ∪ B)' = A' ∩ B'
De Morgan 2:      (A ∩ B)' = A' ∪ B'
```

### Key subset facts

```
∅ ⊆ A                       for every set A
A ⊆ A                       every set is a subset of itself
A ∩ B ⊆ A ⊆ A ∪ B           size ordering
If A ⊆ B: A ∪ B = B          and   A ∩ B = A
A − B = A ∩ B'               difference via complement
```

---

### Part 3 — The Two Core Proof Techniques

### Technique 1 — The element method (proving A ⊆ B)

To prove that set A is a subset of set B:

```
Let x be an arbitrary element of A.
Show, using definitions and logic, that x must also be in B.
Conclude: since x was arbitrary, every element of A is in B, so A ⊆ B.
```

**Template:**

```
Proof:
Let x ∈ A.
[... logical steps using the definition of A ...]
Therefore x ∈ B.
Since x was an arbitrary element of A, we have A ⊆ B. ∎
```

**Example — Prove that `A ∩ B ⊆ A`:**

```
Proof:
Let x ∈ A ∩ B.
By definition of intersection, x ∈ A and x ∈ B.
In particular, x ∈ A.
Since x was arbitrary, every element of A ∩ B is in A.
Therefore A ∩ B ⊆ A. ∎
```

---

### Technique 2 — Double inclusion (proving A = B)

To prove two sets A and B are equal, prove **both directions** of containment:

```
Step 1: Prove A ⊆ B   (using the element method)
Step 2: Prove B ⊆ A   (using the element method in reverse)
Conclude: since A ⊆ B and B ⊆ A, we have A = B.
```

This is the standard technique for ALL set equality proofs. Never try to prove A = B by simplifying — always use double inclusion.

**Template:**

```
Proof:
(⊆) Let x ∈ A. [... show x ∈ B ...] So A ⊆ B.
(⊇) Let x ∈ B. [... show x ∈ A ...] So B ⊆ A.
Since A ⊆ B and B ⊆ A, we conclude A = B. ∎
```

**Example — Prove that `A − B = A ∩ B'`:**

```
Proof:
(⊆) Let x ∈ A − B.
    By definition, x ∈ A and x ∉ B.
    Since x ∉ B, by definition of complement, x ∈ B'.
    So x ∈ A and x ∈ B', which means x ∈ A ∩ B'.
    Therefore A − B ⊆ A ∩ B'.

(⊇) Let x ∈ A ∩ B'.
    Then x ∈ A and x ∈ B'.
    Since x ∈ B', by definition of complement, x ∉ B.
    So x ∈ A and x ∉ B, which means x ∈ A − B.
    Therefore A ∩ B' ⊆ A − B.

Since both inclusions hold, A − B = A ∩ B'. ∎
```

---

### Part 4 — The 10 Most Common Exam Traps

Read every one of these carefully. Each one has caused students to lose marks.

---

### Trap 1 — Confusing ∅ with {∅}

```
∅     has cardinality 0  — it is empty
{∅}   has cardinality 1  — it contains the empty set as an element
```

These are completely different sets. `∅ ∈ {∅}` is TRUE. `∅ = {∅}` is FALSE.

---

### Trap 2 — Confusing ∈ with ⊆

`∈` is for **elements**. `⊆` is for **sets**.

```
3 ∈ {1, 2, 3}          ✅ correct  — 3 is an element
{3} ⊆ {1, 2, 3}        ✅ correct  — {3} is a subset
{3} ∈ {1, 2, 3}        ❌ wrong    — {3} is not an element of {1,2,3}
3 ⊆ {1, 2, 3}          ❌ wrong    — 3 is a number, not a set
```

---

### Trap 3 — Forgetting that A is a subset of itself

```
{1, 2, 3} ⊆ {1, 2, 3}    ✅ TRUE  — every set is a subset of itself
{1, 2, 3} ⊂ {1, 2, 3}    ❌ FALSE — a set is NOT a proper subset of itself
```

---

### Trap 4 — The complement depends on U

```
If U = {1,...,10} and A = {1,2,3}  →  A' = {4,5,6,7,8,9,10}
If U = {1,...,5}  and A = {1,2,3}  →  A' = {4,5}
```

Always identify U before computing any complement.

---

### Trap 5 — Set difference is not commutative

```
A − B  ≠  B − A   in general
```

Example: `{1,2,3} − {3,4,5} = {1,2}` but `{3,4,5} − {1,2,3} = {4,5}`

---

### Trap 6 — Counting elements in a union without subtracting the overlap

A common error in word problems:

```
WRONG: |A ∪ B| = |A| + |B|         (overcounts the intersection)
RIGHT: |A ∪ B| = |A| + |B| − |A ∩ B|
```

If 20 people like cats and 15 like dogs, and 8 like both, the answer is NOT 35 — it is `20 + 15 − 8 = 27`.

---

### Trap 7 — Ordered pairs vs sets

```
(1, 2) ≠ (2, 1)       ordered pairs — order matters
{1, 2}  = {2, 1}       sets — order does not matter
```

---

### Trap 8 — Misapplying De Morgan's Laws

```
(A ∪ B)'  =  A' ∩ B'    ✅  (union becomes intersection)
(A ∪ B)'  =  A' ∪ B'    ❌  (wrong — the operation must flip)
(A ∩ B)'  =  A' ∪ B'    ✅  (intersection becomes union)
```

The operation always flips when the complement moves inside.

---

### Trap 9 — Cardinality of the power set of the empty set

```
|P(∅)|  =  2⁰  =  1
```

The power set of the empty set is NOT empty — it contains exactly one element: `∅` itself.
```
P(∅)  =  {∅}
```

---

### Trap 10 — Assuming A × B = B × A

```
A × B  ≠  B × A   in general
```

The pairs `(a,b)` and `(b,a)` are different ordered pairs unless `a = b`. The only time `A × B = B × A` is when `A = B` or at least one set is empty.

---

### Part 5 — 15 Mixed Practice Problems

These problems are drawn from all six days. No hints are given — this simulates exam conditions.

---

### Section A — Short answer (Days 1–3)

**1.** Let `A = {1, 2, 3, 4, 5, 6}`.
   - a) Write A in set-builder notation.
   - b) Find `|P(A)|`.
   - c) How many proper subsets does A have?

**2.** Let `A = {a, b, c, d}` and `B = {c, d, e, f, g}`.
   - a) Find `A ∪ B`
   - b) Find `A ∩ B`
   - c) Find `A − B`
   - d) Find `A △ B`

**3.** Let `U = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}`, `A = {1, 2, 3, 4, 5}`, `B = {4, 5, 6, 7, 8}`.
   - a) Find `A'`
   - b) Find `B'`
   - c) Find `(A ∩ B)'`
   - d) Find `A' ∪ B'` and verify De Morgan's Second Law

---

### Section B — Venn diagrams and cardinality (Days 4–5)

**4.** In a school of 200 students:
   - 120 study Biology
   - 90 study Chemistry
   - 50 study both

   Find:
   - a) How many study Biology or Chemistry?
   - b) How many study Biology only?
   - c) How many study neither?

**5.** In a survey of 150 people:
   - 80 read newspapers
   - 60 watch TV news
   - 40 listen to radio news
   - 30 read newspapers and watch TV
   - 20 read newspapers and listen to radio
   - 15 watch TV and listen to radio
   - 10 do all three

   Find how many follow at least one news source, and how many follow none.

**6.** Given `|U| = 100`, `|A| = 55`, `|B| = 45`, `|A ∩ B| = 20`. Find:
   - a) `|A ∪ B|`
   - b) `|A'|`
   - c) `|A − B|`
   - d) `|A △ B|`
   - e) `|(A ∪ B)'|`

---

### Section C — Cartesian products and relations (Day 6)

**7.** Let `A = {1, 2, 3}` and `B = {0, 1}`.
   - a) List all elements of `A × B`.
   - b) List all elements of `B × A`.
   - c) Are they equal?

**8.** Find `(x, y)` if `(3x + 1, 2y − 5) = (10, 7)`.

**9.** Let `A = {1, 2, 3, 4, 5}`. Define the relation:
`R = {(a, b) | a² + b² = 25, a ∈ A, b ∈ A}`
   - a) List all elements of R.
   - b) Find Dom(R) and Ran(R).

---

### Section D — Proofs (all days)

**10.** Prove that if `A ⊆ B` and `B ⊆ C`, then `A ⊆ C`.
*(Transitivity of subsets)*

**11.** Prove that `(A ∩ B) ∪ (A − B) = A`.

**12.** Prove that `A ⊆ B` if and only if `A ∩ B = A`.

---

### Section E — Challenge problems

**13.** Let `|A| = m` and `|B| = n` where `A` and `B` are disjoint.
   - a) Find `|A ∪ B|`
   - b) Find `|P(A ∪ B)|`
   - c) Find `|P(A) ∩ P(B)|` — think carefully.

**14.** A set A has the property that `P(A) = {∅, {x}, {y}, {x,y}}`.
   - a) What is A?
   - b) What is `|A|`?
   - c) What is `|A × A|`?
   - d) How many relations are possible on A?

**15.** Let `U = {1, 2, 3, ..., 30}`.
   - `A = {x | x is divisible by 2}`
   - `B = {x | x is divisible by 3}`
   - `C = {x | x is divisible by 5}`

   Find:
   - a) `|A|`, `|B|`, `|C|`
   - b) `|A ∩ B|`, `|A ∩ C|`, `|B ∩ C|`
   - c) `|A ∩ B ∩ C|`
   - d) `|A ∪ B ∪ C|`
   - e) How many numbers from 1 to 30 are divisible by none of 2, 3, or 5?

---

### Part 6 — Full Worked Answers

### Section A

**1.**
- a) `A = {x | x ∈ ℤ⁺, x ≤ 6}` or `A = {x | x is a positive integer, 1 ≤ x ≤ 6}`
- b) `|P(A)| = 2⁶ = 64`
- c) Proper subsets = all subsets except A itself = `64 − 1 = 63`

**2.**
- a) `A ∪ B = {a, b, c, d, e, f, g}`
- b) `A ∩ B = {c, d}`
- c) `A − B = {a, b}` (remove c and d from A)
- d) `A △ B = (A−B) ∪ (B−A) = {a,b} ∪ {e,f,g} = {a, b, e, f, g}`

**3.**
- a) `A' = {6, 7, 8, 9, 10}`
- b) `B' = {1, 2, 3, 9, 10}`
- c) `A ∩ B = {4, 5}`, so `(A ∩ B)' = {1, 2, 3, 6, 7, 8, 9, 10}`
- d) `A' ∪ B' = {6,7,8,9,10} ∪ {1,2,3,9,10} = {1,2,3,6,7,8,9,10}`
     De Morgan's Second Law: `(A ∩ B)' = A' ∪ B' = {1,2,3,6,7,8,9,10}` ✓

---

### Section B

**4.**
```
|Bio ∪ Chem|  =  120 + 90 − 50  =  160
```
- a) 160 students study Biology or Chemistry
- b) Biology only = `120 − 50 = 70` students
- c) Neither = `200 − 160 = 40` students

**5.**
```
|N ∪ T ∪ R|  =  80 + 60 + 40 − 30 − 20 − 15 + 10  =  125
```
- At least one source: **125 people**
- None: `150 − 125 = 25 people`

**6.**
- a) `|A ∪ B| = 55 + 45 − 20 = 80`
- b) `|A'| = 100 − 55 = 45`
- c) `|A − B| = 55 − 20 = 35`
- d) `|A △ B| = 55 + 45 − 2(20) = 60`
- e) `|(A ∪ B)'| = 100 − 80 = 20`

---

### Section C

**7.**
- a) `A × B = {(1,0),(1,1),(2,0),(2,1),(3,0),(3,1)}`
- b) `B × A = {(0,1),(0,2),(0,3),(1,1),(1,2),(1,3)}`
- c) No — the pairs have components in opposite order and are structurally different sets.

**8.**
- `3x + 1 = 10` → `3x = 9` → `x = 3`
- `2y − 5 = 7` → `2y = 12` → `y = 6`
- Answer: `(x, y) = (3, 6)`

**9.**
Check all pairs (a,b) with a,b ∈ {1,2,3,4,5} and a² + b² = 25:
- 3² + 4² = 9 + 16 = 25 ✓ → (3,4)
- 4² + 3² = 16 + 9 = 25 ✓ → (4,3)

No other combinations work within A.
- a) `R = {(3,4),(4,3)}`
- b) `Dom(R) = {3, 4}`, `Ran(R) = {3, 4}`

---

### Section D

**10.** Proof of transitivity — if `A ⊆ B` and `B ⊆ C`, then `A ⊆ C`:

```
Let x ∈ A.
Since A ⊆ B, we have x ∈ B.
Since B ⊆ C, we have x ∈ C.
Since x was an arbitrary element of A, every element of A is in C.
Therefore A ⊆ C. ∎
```

**11.** Proof that `(A ∩ B) ∪ (A − B) = A`:

```
(⊆) Let x ∈ (A ∩ B) ∪ (A − B).
    Case 1: x ∈ A ∩ B → x ∈ A and x ∈ B → in particular x ∈ A.
    Case 2: x ∈ A − B → x ∈ A and x ∉ B → in particular x ∈ A.
    In both cases x ∈ A. So (A ∩ B) ∪ (A − B) ⊆ A.

(⊇) Let x ∈ A.
    Either x ∈ B or x ∉ B (by the law of excluded middle).
    If x ∈ B: then x ∈ A and x ∈ B, so x ∈ A ∩ B ⊆ (A ∩ B) ∪ (A − B).
    If x ∉ B: then x ∈ A and x ∉ B, so x ∈ A − B ⊆ (A ∩ B) ∪ (A − B).
    So A ⊆ (A ∩ B) ∪ (A − B).

Since both inclusions hold: (A ∩ B) ∪ (A − B) = A. ∎
```

**12.** Proof that `A ⊆ B  ⟺  A ∩ B = A`:

```
(→) Assume A ⊆ B. We prove A ∩ B = A.
    (⊆) A ∩ B ⊆ A always (Day 3 result).
    (⊇) Let x ∈ A. Since A ⊆ B, x ∈ B. So x ∈ A and x ∈ B, meaning x ∈ A ∩ B.
    Therefore A ⊆ A ∩ B. Combined: A ∩ B = A.

(←) Assume A ∩ B = A. We prove A ⊆ B.
    Let x ∈ A. Since A = A ∩ B, we have x ∈ A ∩ B.
    By definition of intersection, x ∈ B.
    Therefore A ⊆ B. ∎
```

---

### Section E

**13.**
- a) Since A and B are disjoint, `A ∩ B = ∅`, so `|A ∪ B| = m + n + 0 = m + n`
- b) `|P(A ∪ B)| = 2^(m+n)`
- c) `P(A) ∩ P(B)`:
     Any set S in `P(A)` satisfies `S ⊆ A`. Any set in `P(B)` satisfies `S ⊆ B`.
     For S to be in both, `S ⊆ A` and `S ⊆ B`, so `S ⊆ A ∩ B = ∅`.
     The only subset of ∅ is ∅ itself.
     Therefore `P(A) ∩ P(B) = {∅}` and `|P(A) ∩ P(B)| = 1`.

**14.**
- a) `P(A) = {∅, {x}, {y}, {x,y}}` — this is the power set of a 2-element set.
     Therefore `A = {x, y}`.
- b) `|A| = 2`
- c) `|A × A| = 2 × 2 = 4`
- d) Relations on A are subsets of `A × A`.
     `|A × A| = 4`, so number of relations = `2⁴ = 16`.

**15.**
Within `U = {1, 2, ..., 30}`:
- a) `|A| = 15` (multiples of 2), `|B| = 10` (multiples of 3), `|C| = 6` (multiples of 5)
- b) `|A ∩ B|` = multiples of 6 = `5`
     `|A ∩ C|` = multiples of 10 = `3`
     `|B ∩ C|` = multiples of 15 = `2`
- c) `|A ∩ B ∩ C|` = multiples of 30 = `1` (only 30 itself)
- d) Applying three-set inclusion-exclusion:
```
|A ∪ B ∪ C|  =  15 + 10 + 6 − 5 − 3 − 2 + 1  =  22
```
- e) Divisible by none = `30 − 22 = 8`
     These 8 numbers are: 1, 7, 11, 13, 17, 19, 23, 29 — all primes (except 1) not equal to 2, 3, or 5. A beautiful result.

---

### Part 7 — What Lies Beyond: A Roadmap

You have now mastered the complete high school foundation of set theory. Here is a glimpse of where these ideas lead.

### Functions (immediate next step)

A **function** is a special type of relation `f ⊆ A × B` where every element of A appears as a first component **exactly once**. Functions are the central object of all of algebra, calculus, and analysis.

```
f: A → B   means f is a function from A to B
f(a) = b   means the pair (a, b) ∈ f
```

The sets you have studied become the domain, codomain, and range of functions.

### Number systems as sets

Every number system is formally defined as a set:
```
ℕ  =  {0, 1, 2, 3, ...}           Natural numbers
ℤ  =  {..., −2, −1, 0, 1, 2, ...}  Integers
ℚ  =  {p/q | p,q ∈ ℤ, q ≠ 0}      Rational numbers
ℝ  =  all points on the number line  Real numbers
ℂ  =  {a + bi | a,b ∈ ℝ}           Complex numbers
```

And crucially: `ℕ ⊂ ℤ ⊂ ℚ ⊂ ℝ ⊂ ℂ` — each is a proper subset of the next.

### Cantor's theorem (a taste of infinity)

Georg Cantor proved in 1891 that for **any** set A — finite or infinite:

```
|A|  <  |P(A)|
```

The power set is always strictly larger than the original set. Applied to infinite sets, this means there are **infinitely many different sizes of infinity**. The natural numbers, the integers, and the rational numbers all have the same infinite size (ℵ₀). But the real numbers are provably larger — an infinity that cannot be matched with the natural numbers.

### Axiomatic set theory (university level)

At university, you will learn that all of mathematics — numbers, functions, geometry, probability — can be built from sets using a small list of **axioms** (the Zermelo-Fraenkel axioms). The set is the single most fundamental object in all of mathematics.

---

### Part 8 — Final Self-Assessment Checklist

Before you close these notes, check off each item honestly:

### Day 1 — Foundations
- [ ] I can define a set and explain the three rules (well-defined, distinct, no order)
- [ ] I can use ∈ and ∉ correctly
- [ ] I can write sets in both roster and set-builder notation
- [ ] I understand ∅ and the difference between ∅ and {∅}
- [ ] I know what cardinality |A| means

### Day 2 — Subsets
- [ ] I can prove A ⊆ B using the element-checking method
- [ ] I know the difference between ⊆ and ⊂
- [ ] I can find and list the power set P(A)
- [ ] I can apply |P(A)| = 2ⁿ confidently

### Day 3 — Union and Intersection
- [ ] I can find A ∪ B and A ∩ B correctly
- [ ] I can draw and interpret Venn diagrams for two and three sets
- [ ] I know all the algebraic laws (commutative, associative, distributive, identity)
- [ ] I know that A ∩ B ⊆ A ⊆ A ∪ B

### Day 4 — Complement and Difference
- [ ] I can find A', A − B, and A △ B given U
- [ ] I know A − B = A ∩ B'
- [ ] I can state and apply both De Morgan's Laws
- [ ] I always identify U before computing a complement

### Day 5 — Cardinality and Counting
- [ ] I can apply |A ∪ B| = |A| + |B| − |A ∩ B|
- [ ] I can apply the three-set inclusion-exclusion formula
- [ ] I can fill a Venn diagram inside-out to solve word problems
- [ ] I know the formulas for |A'|, |A−B|, and |A△B|

### Day 6 — Cartesian Product and Relations
- [ ] I know that ordered pairs (a,b) ≠ (b,a) in general
- [ ] I can list A × B systematically using the grid method
- [ ] I know |A × B| = |A| × |B|
- [ ] I can define a relation and find its domain and range

### Proof techniques
- [ ] I can prove A ⊆ B using the element method
- [ ] I can prove A = B using double inclusion

---

### Complete Symbol Quick-Reference Card

Cut out or screenshot this card for revision:

```
╔══════════════════════════════════════════════════════════════╗
║                  SETS — MASTER REFERENCE                     ║
╠══════════════════════════════════════════════════════════════╣
║  ∈        is an element of                                   ║
║  ∉        is not an element of                               ║
║  ∅        empty set                                          ║
║  U        universal set                                      ║
║  |A|      cardinality of A                                   ║
║  A ⊆ B    A is a subset of B                                 ║
║  A ⊂ B    A is a proper subset of B                          ║
║  P(A)     power set of A   →   |P(A)| = 2^|A|                ║
║  A ∪ B    union (OR)                                         ║
║  A ∩ B    intersection (AND)                                 ║
║  A'       complement (NOT A in U)                            ║
║  A − B    set difference (A but NOT B)  =  A ∩ B'            ║
║  A △ B    symmetric difference  =  (A−B) ∪ (B−A)            ║
║  A × B    Cartesian product   →   |A×B| = |A|×|B|            ║
║  (a,b)    ordered pair — order matters                       ║
║  R⊆A×B   R is a relation from A to B                         ║
╠══════════════════════════════════════════════════════════════╣
║  KEY FORMULAS                                                ║
║  |A ∪ B| = |A|+|B|−|A∩B|                                     ║
║  |A∪B∪C| = |A|+|B|+|C|−|A∩B|−|A∩C|−|B∩C|+|A∩B∩C|             ║
║  |A'|    = |U|−|A|                                           ║
║  |A−B|   = |A|−|A∩B|                                         ║
║  |A△B|   = |A|+|B|−2|A∩B|                                    ║
╠══════════════════════════════════════════════════════════════╣
║  DE MORGAN'S LAWS                                            ║
║  (A ∪ B)' = A' ∩ B'                                          ║
║  (A ∩ B)' = A' ∪ B'                                          ║
╚══════════════════════════════════════════════════════════════╝
```


