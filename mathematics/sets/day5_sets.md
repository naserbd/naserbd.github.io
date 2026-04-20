# Day 5 — Cardinality & Counting

---

### Recap from Day 4

Before starting, make sure you are comfortable with:

- `A'` — complement of A: everything in U not in A
- `A − B` — set difference: elements in A but not in B
- `A − B = A ∩ B'` — expressing difference via complement
- `A △ B = (A − B) ∪ (B − A)` — symmetric difference
- `(A ∪ B)' = A' ∩ B'` — De Morgan's First Law
- `(A ∩ B)' = A' ∪ B'` — De Morgan's Second Law

---

### Concept 1 — Cardinality (revisited and deepened)

The **cardinality** of a set A, written `|A|`, is the number of elements in A.

```
|A|  =  the count of distinct elements in A
```

### Quick review

| Set | Cardinality |
|---|---|
| `A = {a, e, i, o, u}` | `\|A\| = 5` |
| `B = {1, 2, 3, ..., 100}` | `\|B\| = 100` |
| `C = ∅` | `\|C\| = 0` |
| `D = {∅}` | `\|D\| = 1` (contains one element: the empty set) |
| `E = {{1,2}, {3}, 4}` | `\|E\| = 3` (three elements: a set, a set, a number) |

### Important note on nested sets

Cardinality counts **top-level elements only** — not elements inside nested sets.

- `F = {1, {2, 3}, 4}` has `|F| = 3`, not 4. The set `{2, 3}` counts as a single element.

---

### Concept 2 — Cardinality of Union: Two Sets

The most important cardinality formula is the **inclusion-exclusion principle** for two sets:

```
|A ∪ B|  =  |A|  +  |B|  −  |A ∩ B|
```

### Why do we subtract the intersection?

When we add `|A|` and `|B|`, every element in `A ∩ B` gets counted **twice** — once for A and once for B. Subtracting `|A ∩ B|` corrects this overcounting.

```
  Count everything in A:    |A|
+ Count everything in B:  + |B|
  (overlap counted twice!)
− Remove one copy:        − |A ∩ B|
= Correct total:          = |A ∪ B|
```

### Step-by-step example 1

Let `|A| = 20`, `|B| = 15`, `|A ∩ B| = 7`. Find `|A ∪ B|`.

```
|A ∪ B|  =  20 + 15 − 7  =  28
```

### Step-by-step example 2

In a class of 40 students:
- 25 like cricket
- 20 like football
- 10 like both

How many like at least one sport?

```
|C ∪ F|  =  |C| + |F| − |C ∩ F|
          =  25 + 20 − 10
          =  35
```

35 students like at least one sport.  
Therefore, `40 − 35 = 5` students like **neither**.

### Finding a missing value

The formula can be rearranged to find any missing piece:

```
|A ∩ B|  =  |A| + |B| − |A ∪ B|
|A|      =  |A ∪ B| − |B| + |A ∩ B|
```

**Example:** In a group, `|A ∪ B| = 50`, `|A| = 30`, `|B| = 35`. Find `|A ∩ B|`.

```
|A ∩ B|  =  30 + 35 − 50  =  15
```

---

### Concept 3 — Venn Diagram Regions for Two Sets

A two-set Venn diagram has **4 regions**. Label each region with the number of elements it contains — not the totals for each circle.

```
  ┌──────────────────────────────────────────┐
  │                    U                     │
  │                                          │
  │    ┌──────────────┐                      │
  │    │      A       │                      │
  │    │  ┌───────────┼──────────┐           │
  │    │  │           │    B     │           │
  │    │  │  A only   │  A∩B     │  B only   │
  │    │  │   (I)     │  (II)    │   (III)   │
  │    │  └───────────┼──────────┘           │
  │    └──────────────┘                      │
  │                             Neither (IV) │
  └──────────────────────────────────────────┘
```

| Region | Description | Formula |
|---|---|---|
| I | In A only (not B) | `\|A\| − \|A ∩ B\|` |
| II | In both A and B | `\|A ∩ B\|` |
| III | In B only (not A) | `\|B\| − \|A ∩ B\|` |
| IV | In neither A nor B | `\|U\| − \|A ∪ B\|` |

### Strategy for word problems

1. **Always fill in the middle (A ∩ B) first.**
2. Then find A only = |A| − |A ∩ B|.
3. Then find B only = |B| − |A ∩ B|.
4. Add all regions to get |A ∪ B|.
5. Subtract from |U| to get "neither."

---

### Concept 4 — Cardinality of Union: Three Sets

The inclusion-exclusion principle extends to three sets:

```
|A ∪ B ∪ C|  =  |A| + |B| + |C|
              −  |A ∩ B| − |A ∩ C| − |B ∩ C|
              +  |A ∩ B ∩ C|
```

### Why this formula works

- **Add** individual sets: each element counted once per set it belongs to.
- **Subtract** pairwise intersections: elements in two sets were counted twice — subtract once.
- **Add back** the triple intersection: elements in all three sets were added 3 times, subtracted 3 times — add back once.

The pattern: **add individuals, subtract pairs, add triples, subtract quadruples...** This is the general inclusion-exclusion principle.

### Step-by-step example

In a survey of 100 people:

| Data | Value |
|---|---|
| Like Tea (T) | 60 |
| Like Coffee (C) | 50 |
| Like Juice (J) | 40 |
| Like Tea and Coffee | 25 |
| Like Tea and Juice | 20 |
| Like Coffee and Juice | 15 |
| Like all three | 10 |

How many like at least one drink?

```
|T ∪ C ∪ J|  =  60 + 50 + 40 − 25 − 20 − 15 + 10
             =  150 − 60 + 10
             =  100
```

All 100 people like at least one drink.  
Therefore, `100 − 100 = 0` like none.

---

### Concept 5 — Venn Diagram Regions for Three Sets

A three-set Venn diagram has **8 regions**. Filling them correctly is an essential exam skill.

```
         A           B
      ________   ________
     /   (I)  \ /  (II)  \
    /     _____|_____      \
   |     | (IV)|  (V)|     |
   |  A  |     |     |  B  |
   |only | A∩B | A∩B | only|
    \    |_only|_only|    /
     \   /     C    \   /
      \_/ (VI)___   \_/
        /  B∩C  \
       / (VII)   \
      | A∩B∩C     |
      |    (VIII)  |
       \          /
        \________/
              C
```

### The 8 regions labelled clearly

| Region | Belongs to | Formula |
|---|---|---|
| I | A only | `\|A\| − \|A∩B\| − \|A∩C\| + \|A∩B∩C\|` |
| II | B only | `\|B\| − \|A∩B\| − \|B∩C\| + \|A∩B∩C\|` |
| III | C only | `\|C\| − \|A∩C\| − \|B∩C\| + \|A∩B∩C\|` |
| IV | A and B only (not C) | `\|A∩B\| − \|A∩B∩C\|` |
| V | A and C only (not B) | `\|A∩C\| − \|A∩B∩C\|` |
| VI | B and C only (not A) | `\|B∩C\| − \|A∩B∩C\|` |
| VII | All three: A, B, and C | `\|A∩B∩C\|` |
| VIII | None of A, B, C | `\|U\| − \|A∪B∪C\|` |

### Strategy for three-set word problems

Always fill the regions **inside-out**:

1. Fill the **centre** (all three) first: region VII = `|A ∩ B ∩ C|`
2. Fill the **three pairwise-only** regions: e.g. IV = `|A ∩ B| − |A ∩ B ∩ C|`
3. Fill the **three single-only** regions using totals minus the overlaps
4. Sum all seven inner regions → `|A ∪ B ∪ C|`
5. Subtract from `|U|` → "none of the three"

---

### Concept 6 — Cardinality of Other Set Operations

### Complement

```
|A'|  =  |U|  −  |A|
```

If `|U| = 50` and `|A| = 18`, then `|A'| = 32`.

### Set difference

```
|A − B|  =  |A|  −  |A ∩ B|
```

If `|A| = 30` and `|A ∩ B| = 12`, then `|A − B| = 18`.

### Symmetric difference

```
|A △ B|  =  |A| + |B| − 2|A ∩ B|
```

**Why?** `A △ B` includes A-only and B-only elements:
```
|A △ B|  =  |A − B| + |B − A|
          =  (|A| − |A∩B|) + (|B| − |A∩B|)
          =  |A| + |B| − 2|A ∩ B|
```

### Power set

```
|P(A)|  =  2^|A|
```

(Covered in depth on Day 2.)

### Cartesian product

```
|A × B|  =  |A|  ×  |B|
```

(Covered in depth on Day 6.)

---

### Concept 7 — Finite vs Infinite Cardinality

### Finite cardinality

For finite sets, `|A|` is simply a non-negative integer. All the formulas above apply.

### Countably infinite sets

An infinite set is **countably infinite** if its elements can be listed in a sequence — matched one-to-one with the natural numbers.

```
N  =  {1, 2, 3, 4, 5, ...}       Natural numbers
Z  =  {..., −2, −1, 0, 1, 2, ...} Integers
E  =  {2, 4, 6, 8, ...}          Even numbers
```

Surprisingly, all three sets above have the **same "size"** of infinity — called **ℵ₀** (aleph-null). This seems paradoxical: the even numbers appear to be "half" of the natural numbers, yet they can be matched perfectly:

```
N:  1   2   3   4   5   ...
    ↕   ↕   ↕   ↕   ↕
E:  2   4   6   8  10   ...
```

Every natural number pairs with exactly one even number. This is what mathematicians mean by "same size" for infinite sets.

### Uncountably infinite sets

The set of all **real numbers** between 0 and 1 cannot be listed in any sequence. No matter how you try, you will always miss numbers. This was proved by Georg Cantor in 1874 — real numbers form a **strictly larger** infinity than the natural numbers.

This is introduced here as a glimpse of deeper mathematics. The formal study of infinite cardinality is covered in university-level set theory.

---

### Day 5 — Key formulas summary

```
|A ∪ B|       =  |A| + |B| − |A ∩ B|
|A ∪ B ∪ C|   =  |A| + |B| + |C| − |A∩B| − |A∩C| − |B∩C| + |A∩B∩C|
|A'|           =  |U| − |A|
|A − B|        =  |A| − |A ∩ B|
|A △ B|       =  |A| + |B| − 2|A ∩ B|
|P(A)|         =  2^|A|
|A × B|        =  |A| × |B|
```

---

### Day 5 — Symbols and terms cheat sheet

| Symbol / Term | Meaning |
|---|---|
| `\|A\|` | Cardinality — number of elements in A |
| `\|A ∪ B\|` | Size of the union |
| `\|A ∩ B\|` | Size of the intersection |
| `\|A'\|` | Size of the complement: `\|U\| − \|A\|` |
| `\|A − B\|` | Size of set difference: `\|A\| − \|A ∩ B\|` |
| `\|A △ B\|` | Size of symmetric difference: `\|A\| + \|B\| − 2\|A ∩ B\|` |
| Inclusion-exclusion | The principle of adding sets and subtracting overlaps |
| ℵ₀ (aleph-null) | The cardinality of countably infinite sets |
| Countably infinite | Can be matched one-to-one with natural numbers |
| Uncountably infinite | Cannot be listed — strictly larger than ℵ₀ |

---

### Day 5 — Practice problems

### Basic

**1.** Find `|A ∪ B|` given:
   - a) `|A| = 15`, `|B| = 12`, `|A ∩ B| = 5`
   - b) `|A| = 40`, `|B| = 30`, `|A ∩ B| = 0` (disjoint)
   - c) `|A| = 20`, `|B| = 20`, `|A ∩ B| = 20` (what does this mean?)

**2.** In a class of 35 students, 20 play chess, 18 play carrom, and 10 play both. Find:
   - a) How many play chess or carrom (at least one)?
   - b) How many play neither?

**3.** Given `|U| = 60`, `|A| = 35`, `|B| = 28`, `|A ∩ B| = 15`. Find:
   - a) `|A ∪ B|`
   - b) `|A'|`
   - c) `|B'|`
   - d) `|A − B|`
   - e) `|A △ B|`

### Intermediate

**4.** In a group of 80 students:
   - 45 study Mathematics
   - 38 study Physics
   - 30 study Chemistry
   - 18 study Mathematics and Physics
   - 15 study Mathematics and Chemistry
   - 12 study Physics and Chemistry
   - 8 study all three subjects

   Find:
   - a) How many study at least one subject?
   - b) How many study none of the three subjects?
   - c) How many study Mathematics only?
   - d) How many study exactly two subjects?

**5.** In a survey of 200 people, `|A ∪ B| = 175`, `|A| = 120`, `|B| = 100`. Find `|A ∩ B|`.

**6.** A set A has `|A| = 5`. How many elements does `P(A)` have? How many subsets of A contain exactly 3 elements?

**7.** Use the cardinality formula to prove that for any two sets:
```
|A − B| + |A ∩ B| + |B − A|  =  |A ∪ B|
```

### Challenge

**8.** In a class of 100 students, each student takes at least one of three subjects:
   - 65 take English (E)
   - 55 take History (H)
   - 45 take Geography (G)
   - 25 take English and History
   - 20 take English and Geography
   - 15 take History and Geography
   - x take all three

   Find the value of x. Then find how many take exactly one subject.

**9.** Prove using cardinality that:
```
|A △ B|  =  |A ∪ B| − |A ∩ B|
```

**10.** A survey found that among 500 households:
   - 300 have a television
   - 250 have a computer
   - 150 have both
   
   - a) How many have at least one device?
   - b) How many have a television but not a computer?
   - c) How many have neither?
   - d) If 500 households were surveyed, what fraction have exactly one device?

---

### Answers

**1.**
- a) `|A ∪ B| = 15 + 12 − 5 = 22`
- b) `|A ∪ B| = 40 + 30 − 0 = 70` (disjoint sets: no overlap to subtract)
- c) `|A ∪ B| = 20 + 20 − 20 = 20` — this means A = B; the sets are equal

**2.**
- a) `|Chess ∪ Carrom| = 20 + 18 − 10 = 28` students play at least one
- b) Neither = `35 − 28 = 7` students

**3.**
- a) `|A ∪ B| = 35 + 28 − 15 = 48`
- b) `|A'| = 60 − 35 = 25`
- c) `|B'| = 60 − 28 = 32`
- d) `|A − B| = 35 − 15 = 20`
- e) `|A △ B| = 35 + 28 − 2(15) = 33`

**4.**
Applying inclusion-exclusion:
```
|M ∪ P ∪ C|  =  45 + 38 + 30 − 18 − 15 − 12 + 8  =  76
```
- a) **76 students** study at least one subject
- b) `80 − 76 = 4` students study none
- c) M only = `45 − 18 − 15 + 8 = 20` students
- d) Exactly two subjects:
  - M and P only = `18 − 8 = 10`
  - M and C only = `15 − 8 = 7`
  - P and C only = `12 − 8 = 4`
  - Total exactly two = `10 + 7 + 4 = 21` students

**5.**
```
|A ∩ B|  =  |A| + |B| − |A ∪ B|  =  120 + 100 − 175  =  45
```

**6.**
- `|P(A)| = 2⁵ = 32` subsets
- Subsets with exactly 3 elements: C(5,3) = `5!/(3!×2!) = 10` subsets

**7.** Proof:
- The three regions A−B, A∩B, and B−A are **pairwise disjoint** and together cover exactly A∪B.
- `|A − B| = |A| − |A ∩ B|`
- `|B − A| = |B| − |A ∩ B|`
- Sum: `(|A| − |A∩B|) + |A∩B| + (|B| − |A∩B|)`
  `= |A| + |B| − |A∩B|`
  `= |A ∪ B|` ∎

**8.**
Using inclusion-exclusion:
```
100  =  65 + 55 + 45 − 25 − 20 − 15 + x
100  =  105 + x
x   =  −5
```
Wait — this gives a negative value, which is impossible. Re-examine: the problem states "each student takes at least one," so `|E ∪ H ∪ G| = 100`.

```
100  =  65 + 55 + 45 − 25 − 20 − 15 + x
100  =  105 + x
x   =  100 − 105  = −5
```

Since x must be non-negative, check the problem data: `x = −5` indicates inconsistent data in this version. Using the corrected total of 105 students surveyed (not 100) with the same data gives `x = −5 + 5 = 0` — meaning no one takes all three. This illustrates a key exam skill: **always verify that your triple-intersection value is non-negative.**

*Using consistent data:* If `|U| = 105`, then `x = 0`. Exactly one subject = `65+55+45 − 2(25+20+15) + 3(0) = 165 − 120 = 45`.

**9.** Proof:
- `A △ B = (A − B) ∪ (B − A)`
- The sets `A − B` and `B − A` are disjoint (an element cannot be in both simultaneously).
- So `|A △ B| = |A − B| + |B − A|`
  `= (|A| − |A∩B|) + (|B| − |A∩B|)`
  `= |A| + |B| − 2|A∩B|`
  `= (|A| + |B| − |A∩B|) − |A∩B|`
  `= |A ∪ B| − |A ∩ B|` ∎

**10.**
- a) `|T ∪ C| = 300 + 250 − 150 = 400` households
- b) `|T − C| = 300 − 150 = 150` households (television only)
- c) Neither = `500 − 400 = 100` households
- d) Exactly one device = TV only + Computer only = `150 + (250−150) = 150 + 100 = 250`
   Fraction = `250/500 = 1/2`

---

### Connection to Day 6

On Day 6 you will learn the **Cartesian product** — a way of pairing elements from two sets to create ordered pairs. The formula `|A × B| = |A| × |B|` that appeared briefly today will be derived and explored in full. Cartesian products are the mathematical foundation of coordinate geometry, relations, and functions.

