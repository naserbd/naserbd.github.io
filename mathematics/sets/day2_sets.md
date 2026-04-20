# Day 2 — Subsets & Power Sets

---

### Recap from Day 1

Before starting, make sure you are comfortable with:

- A **set** is a well-defined collection of distinct objects
- `∈` means "is an element of", `∉` means "is not an element of"
- **Roster notation**: `A = {1, 2, 3}`
- **Set-builder notation**: `A = {x | x is a natural number, x ≤ 3}`
- The **empty set** `∅` contains no elements
- **Cardinality** `|A|` is the number of elements in set A

---

### Concept 1 — What is a subset?

Set A is a **subset** of set B if every element of A is also an element of B.

```
A ⊆ B   means   "A is a subset of B"
```

Read `A ⊆ B` as: *"A is a subset of B"* or *"A is contained in B."*

### The element-checking method — how to prove A ⊆ B

Take **every single element** from A and verify it exists in B.  
If even **one element** of A is missing from B, then A is **not** a subset of B.

### Examples

Let `B = {1, 2, 3, 4, 5, 6}`

| Set A | A ⊆ B? | Reason |
|---|---|---|
| `{1, 2, 3}` | ✅ Yes | 1, 2, 3 all appear in B |
| `{2, 4, 6}` | ✅ Yes | 2, 4, 6 all appear in B |
| `{1, 2, 7}` | ❌ No | 7 is not in B |
| `{6}` | ✅ Yes | 6 appears in B |
| `∅` | ✅ Yes | explained in Concept 3 below |

### The "not a subset" symbol

```
A ⊄ B   means   "A is NOT a subset of B"
```

---

### Concept 2 — Proper subset

Set A is a **proper subset** of set B if:
1. A ⊆ B (every element of A is in B), **AND**
2. A ≠ B (A is not equal to B — it is missing at least one element of B)

```
A ⊂ B   means   "A is a proper subset of B"
```

### Subset vs proper subset — the key difference

| Symbol | Meaning | Allows A = B? |
|---|---|---|
| `A ⊆ B` | Subset | ✅ Yes |
| `A ⊂ B` | Proper subset | ❌ No |

### Examples

Let `B = {1, 2, 3}`

| Set A | A ⊆ B? | A ⊂ B? | Reason |
|---|---|---|---|
| `{1, 2}` | ✅ Yes | ✅ Yes | Inside B, but not equal to B |
| `{1, 2, 3}` | ✅ Yes | ❌ No | Equal to B — not a *proper* subset |
| `{1, 4}` | ❌ No | ❌ No | 4 is not in B |

> **Analogy:** Think of `⊆` like `≤` (less than or equal) and `⊂` like `<` (strictly less than) for numbers. The proper subset is the stricter version.

---

### Concept 3 — The superset

The **superset** is simply the reverse relationship of a subset.

```
B ⊇ A   means   "B is a superset of A"   (same as A ⊆ B)
B ⊃ A   means   "B is a proper superset of A"   (same as A ⊂ B)
```

### Example

If `A = {1, 2}` and `B = {1, 2, 3, 4}`, then:
- `A ⊆ B` — A is a subset of B
- `B ⊇ A` — B is a superset of A

Both statements say the exact same thing, just from opposite perspectives.

---

### Concept 4 — The empty set is a subset of every set

This is one of the most important (and surprising) facts in set theory:

```
∅ ⊆ A   for every set A, without exception
```

### Why is this true?

To show A is **not** a subset of B, you need to find at least one element in A that is missing from B.

The empty set has **no elements at all** — so there is nothing to check. You cannot find a "counterexample" because there are no elements to begin with.

This is called a **vacuously true** statement — it is true because there is nothing to make it false.

### Examples

- `∅ ⊆ {1, 2, 3}` ✅
- `∅ ⊆ {a, b, c}` ✅
- `∅ ⊆ ∅` ✅ (the empty set is a subset of itself)

> The empty set is a **proper** subset of every non-empty set, because `∅ ≠ A` whenever A has at least one element.

---

### Concept 5 — Every set is a subset of itself

```
A ⊆ A   for every set A
```

This is trivially true: every element of A is clearly in A.  
This is why `A ⊆ A` holds, but `A ⊂ A` does **not** (a set cannot be a *proper* subset of itself).

---

### Concept 6 — The Power Set P(A)

The **power set** of A, written `P(A)`, is the set of **all possible subsets** of A — including the empty set and A itself.

```
P(A) = { all subsets of A }
```

### Step-by-step example

Let `A = {1, 2, 3}`. List every possible subset:

| Subset size | Subsets |
|---|---|
| 0 elements | `∅` |
| 1 element | `{1}`, `{2}`, `{3}` |
| 2 elements | `{1,2}`, `{1,3}`, `{2,3}` |
| 3 elements | `{1,2,3}` |

Therefore:

```
P(A) = { ∅, {1}, {2}, {3}, {1,2}, {1,3}, {2,3}, {1,2,3} }
```

`|P(A)| = 8`

### The power set formula

If a set A has `n` elements, then its power set has exactly `2ⁿ` subsets.

```
|P(A)| = 2^|A|   =   2ⁿ
```

| Set A | \|A\| | \|P(A)\| = 2ⁿ |
|---|---|---|
| `∅` | 0 | 2⁰ = 1 (only subset is ∅ itself) |
| `{a}` | 1 | 2¹ = 2 |
| `{a, b}` | 2 | 2² = 4 |
| `{a, b, c}` | 3 | 2³ = 8 |
| `{a, b, c, d}` | 4 | 2⁴ = 16 |

> **Why 2ⁿ?** For each element in A, you make a binary choice: either include it in the subset, or don't. With n elements and 2 choices each, you get 2 × 2 × 2 × ... (n times) = 2ⁿ total combinations.

---

### Concept 7 — Counting subsets of each size

When listing subsets of A, the number of subsets of size `k` from a set of size `n` is given by the **combination formula**:

```
C(n, k)  =  n! / (k! × (n−k)!)
```

You don't need to memorise this formula yet — but you should notice the pattern:

### For A = {a, b, c, d} with |A| = 4

| Subset size k | Number of subsets | Subsets |
|---|---|---|
| 0 | C(4,0) = 1 | `∅` |
| 1 | C(4,1) = 4 | `{a}`, `{b}`, `{c}`, `{d}` |
| 2 | C(4,2) = 6 | `{a,b}`, `{a,c}`, `{a,d}`, `{b,c}`, `{b,d}`, `{c,d}` |
| 3 | C(4,3) = 4 | `{a,b,c}`, `{a,b,d}`, `{a,c,d}`, `{b,c,d}` |
| 4 | C(4,4) = 1 | `{a,b,c,d}` |
| **Total** | **1+4+6+4+1 = 16 = 2⁴** | |

Notice: the counts 1, 4, 6, 4, 1 form a row of **Pascal's Triangle**!

---

### Day 2 — Key properties summary

```
1.  A ⊆ A                    Every set is a subset of itself
2.  ∅ ⊆ A                    The empty set is a subset of every set
3.  If A ⊆ B and B ⊆ A, then A = B     (set equality via double inclusion)
4.  If A ⊆ B and B ⊆ C, then A ⊆ C    (transitivity of subsets)
5.  |P(A)| = 2^|A|           Power set size formula
```

---

### Day 2 — Symbols cheat sheet

| Symbol | Meaning |
|---|---|
| `A ⊆ B` | A is a subset of B (A ⊆ B allows A = B) |
| `A ⊂ B` | A is a proper subset of B (A ≠ B) |
| `A ⊄ B` | A is NOT a subset of B |
| `B ⊇ A` | B is a superset of A |
| `B ⊃ A` | B is a proper superset of A |
| `P(A)` | The power set of A — all subsets of A |
| `2ⁿ` | Number of subsets when \|A\| = n |

---

### Day 2 — Practice problems

### Basic

**1.** Let `A = {2, 4, 6, 8}` and `B = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}`.
   - a) Is `A ⊆ B`? Justify using the element-checking method.
   - b) Is `A ⊂ B`? Why or why not?
   - c) Is `B ⊆ A`? Why or why not?

**2.** List all subsets of `S = {x, y}`.

**3.** How many subsets does `T = {1, 2, 3, 4, 5}` have?

### Intermediate

**4.** Write out the full power set of `A = {a, b, c}`.

**5.** Determine whether each statement is true or false:
   - a) `{3, 5} ⊆ {1, 2, 3, 4, 5}`
   - b) `{1, 6} ⊆ {1, 2, 3, 4, 5}`
   - c) `∅ ⊆ {7, 8, 9}`
   - d) `{a, b, c} ⊂ {a, b, c}`

**6.** A set A has 6 elements. How many subsets does it have? How many proper subsets?

### Challenge

**7.** If `A ⊆ B` and `|A| = |B|`, what can you conclude about A and B? Prove it.

**8.** How many subsets of `{1, 2, 3, 4, 5}` contain the element 3?

---

### Answers

**1.**
- a) Yes. Check: 2 ∈ B ✓, 4 ∈ B ✓, 6 ∈ B ✓, 8 ∈ B ✓. All elements of A are in B, so A ⊆ B.
- b) Yes. A ⊆ B and A ≠ B (B has elements not in A), so A ⊂ B.
- c) No. 1 ∈ B but 1 ∉ A, so B ⊄ A.

**2.** `P({x, y}) = { ∅, {x}, {y}, {x, y} }` — 4 subsets (2² = 4)

**3.** `|P(T)| = 2⁵ = 32` subsets

**4.**
```
P({a,b,c}) = { ∅, {a}, {b}, {c}, {a,b}, {a,c}, {b,c}, {a,b,c} }
```
8 subsets (2³ = 8)

**5.**
- a) True — 3 and 5 are both in the set
- b) False — 6 is not in the set
- c) True — the empty set is a subset of every set
- d) False — a set cannot be a *proper* subset of itself

**6.**
- Total subsets: `2⁶ = 64`
- Proper subsets: `2⁶ − 1 = 63` (all subsets except the set itself)

**7.** If `A ⊆ B` and `|A| = |B|`, then `A = B`.
- Proof: Since A ⊆ B, every element of A is in B. Since they have the same number of elements and all of A's elements are accounted for in B with no room for extras, B cannot have any element that A doesn't. Therefore every element of B is also in A, so B ⊆ A. Since A ⊆ B and B ⊆ A, we conclude A = B.

**8.** 16 subsets.
- Fix 3 as included. Then choose any combination of the remaining 4 elements {1, 2, 4, 5}.
- Number of choices = 2⁴ = 16.

---

### Connection to Day 3

On Day 3 you will learn **Union (A ∪ B)** and **Intersection (A ∩ B)** — the two main operations that combine sets. Subsets will reappear immediately: after you intersect two sets, the result is always a subset of both originals.

