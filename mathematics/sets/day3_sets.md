# Day 3 — Union & Intersection

---

### Recap from Day 2

Before starting, make sure you are comfortable with:

- `A ⊆ B` — every element of A is also in B (subset)
- `A ⊂ B` — A is a subset of B and A ≠ B (proper subset)
- `∅ ⊆ A` — the empty set is a subset of every set
- `P(A)` — the power set of A (all possible subsets)
- `|P(A)| = 2ⁿ` — if A has n elements, it has 2ⁿ subsets

---

## Concept 1 — Union (A ∪ B)

The **union** of two sets A and B is the set of all elements that are in A, in B, or in **both**.

```
A ∪ B  =  { x | x ∈ A  OR  x ∈ B }
```

Read `A ∪ B` as: *"A union B"* or *"A or B."*

The key word is **OR** — an element only needs to belong to at least one of the sets.

### Step-by-step example

Let `A = {1, 2, 3, 4}` and `B = {3, 4, 5, 6}`

- Collect everything in A: 1, 2, 3, 4
- Collect everything in B: 3, 4, 5, 6
- Combine, removing duplicates: **1, 2, 3, 4, 5, 6**

```
A ∪ B  =  {1, 2, 3, 4, 5, 6}
```

Notice: 3 and 4 appear in both sets, but they are only written **once** in the union.

### Venn diagram — union

```
        A                 B
   ___________       ___________
  /           \     /           \
 /  1   2      \   /      5   6  \
|         3  4  | |  3  4        |
 \             / \ \             /
  \___________/   \___________/

  ╔═══════════════════════════╗
  ║  A ∪ B  =  shade ALL      ║
  ║  (everything in both      ║
  ║   circles combined)       ║
  ╚═══════════════════════════╝
```

In a Venn diagram, the **union shades the entire area of both circles** — left region, middle overlap, and right region.

---

### Concept 2 — Intersection (A ∩ B)

The **intersection** of two sets A and B is the set of all elements that are in **both** A and B simultaneously.

```
A ∩ B  =  { x | x ∈ A  AND  x ∈ B }
```

Read `A ∩ B` as: *"A intersection B"* or *"A and B."*

The key word is **AND** — an element must belong to **both** sets at the same time.

### Step-by-step example

Let `A = {1, 2, 3, 4}` and `B = {3, 4, 5, 6}`

- Ask: which elements appear in A **AND** also in B?
- 1 is in A, but not in B — excluded
- 2 is in A, but not in B — excluded
- 3 is in A and in B — **included**
- 4 is in A and in B — **included**
- 5 is in B, but not in A — excluded
- 6 is in B, but not in A — excluded

```
A ∩ B  =  {3, 4}
```

### Venn diagram — intersection

```
        A                 B
   ___________       ___________
  /           \     /           \
 /  1   2      \   /      5   6  \
|         3  4  | |  3  4        |
 \             / \ \             /
  \___________/   \___________/

  ╔═══════════════════════════╗
  ║  A ∩ B  =  shade ONLY     ║
  ║  the overlapping middle   ║
  ╚═══════════════════════════╝
```

In a Venn diagram, the **intersection shades only the overlapping middle region** of the two circles.

---

### Concept 3 — Union vs Intersection — side by side

Using the same sets `A = {1, 2, 3, 4}` and `B = {3, 4, 5, 6}`:

| Operation | Symbol | Key word | Result | What it shades |
|---|---|---|---|---|
| Union | `A ∪ B` | OR | `{1, 2, 3, 4, 5, 6}` | Both circles entirely |
| Intersection | `A ∩ B` | AND | `{3, 4}` | Middle overlap only |

### Memory trick

- The **union** symbol `∪` looks like the letter **U** — think **U**nion, think **U**nderline (everything underneath both circles).
- The **intersection** symbol `∩` looks like a bridge or arch — only what is **directly under the arch** (the middle) counts.

---

### Concept 4 — Disjoint sets

Two sets are **disjoint** if they share no elements — their intersection is the empty set.

```
A and B are disjoint  ⟺  A ∩ B = ∅
```

### Example

Let `A = {1, 2, 3}` and `B = {4, 5, 6}`

- Do they share any elements? No.
- Therefore `A ∩ B = ∅` — A and B are disjoint.

### Venn diagram — disjoint sets

```
        A              B
   ___________    ___________
  /           \  /           \
 /   1  2  3   \/   4  5  6   \
|               ||              |
 \             /\              /
  \___________/  \___________/

  (Two separate circles that do NOT overlap)
```

Disjoint sets are drawn as two completely separate circles with no overlap region.

---

### Concept 5 — Laws of Union and Intersection

These are the fundamental algebraic laws. They work exactly like number algebra, but for sets.

### Commutative laws

```
A ∪ B  =  B ∪ A
A ∩ B  =  B ∩ A
```

Order does not matter — the result is the same either way.

### Associative laws

```
(A ∪ B) ∪ C  =  A ∪ (B ∪ C)
(A ∩ B) ∩ C  =  A ∩ (B ∩ C)
```

When combining three or more sets, the grouping does not matter.

### Distributive laws

```
A ∩ (B ∪ C)  =  (A ∩ B) ∪ (A ∩ C)
A ∪ (B ∩ C)  =  (A ∪ B) ∩ (A ∪ C)
```

Intersection distributes over union, and union distributes over intersection — just like multiplication distributes over addition in arithmetic.

### Identity laws

```
A ∪ ∅  =  A          (union with empty set changes nothing)
A ∩ U  =  A          (intersection with universal set changes nothing)
```

Where `U` is the universal set (the master set containing everything).

### Idempotent laws

```
A ∪ A  =  A
A ∩ A  =  A
```

A set combined with itself is just itself.

### Domination laws

```
A ∪ U  =  U          (union with universal set gives the universal set)
A ∩ ∅  =  ∅          (intersection with empty set gives the empty set)
```

---

### Concept 6 — Subset relationship after operations

Two important results that connect Day 2 and Day 3:

```
A ∩ B  ⊆  A    and    A ∩ B  ⊆  B
A  ⊆  A ∪ B    and    B  ⊆  A ∪ B
```

In words:
- The **intersection** is always a subset of both original sets (it can only be smaller).
- Both original sets are always subsets of their **union** (the union can only be larger).

### Proof that A ∩ B ⊆ A

Let `x ∈ A ∩ B`.  
By definition of intersection, `x ∈ A` AND `x ∈ B`.  
In particular, `x ∈ A`.  
Since every element of `A ∩ B` is in A, we have `A ∩ B ⊆ A`. ∎

---

### Concept 7 — Working with three sets

Union and intersection extend naturally to three sets.

### Three-set union

```
A ∪ B ∪ C  =  { x | x ∈ A  OR  x ∈ B  OR  x ∈ C }
```

Everything in at least one of the three sets.

### Three-set intersection

```
A ∩ B ∩ C  =  { x | x ∈ A  AND  x ∈ B  AND  x ∈ C }
```

Only elements that appear in **all three** sets simultaneously.

### Step-by-step example

Let:
- `A = {1, 2, 3, 4}`
- `B = {2, 4, 6, 8}`
- `C = {1, 2, 3, 6}`

**Finding A ∪ B ∪ C:**

Collect all elements, remove duplicates:
```
A ∪ B ∪ C  =  {1, 2, 3, 4, 6, 8}
```

**Finding A ∩ B ∩ C:**

Which elements appear in ALL three sets?
- 1: in A ✓, in B ✗ — stop, 1 is out
- 2: in A ✓, in B ✓, in C ✓ — **included**
- 3: in A ✓, in B ✗ — stop, 3 is out
- 4: in A ✓, in B ✓, in C ✗ — stop, 4 is out

```
A ∩ B ∩ C  =  {2}
```

### Three-set Venn diagram regions

A three-set Venn diagram has **8 distinct regions**:

```
  Region  |  Contents
  --------|------------------------------------------
  I       |  In A only
  II      |  In B only
  III     |  In C only
  IV      |  In A and B only (not C)
  V       |  In A and C only (not B)
  VI      |  In B and C only (not A)
  VII     |  In A, B, and C (the centre)
  VIII    |  In none of A, B, C (outside all circles)
```

Understanding these 8 regions is essential for solving word problems on Day 5 (Cardinality & Counting).

---

### Day 3 — Key results summary

```
A ∪ B  = B ∪ A                    (commutative)
A ∩ B  = B ∩ A                    (commutative)
A ∪ ∅  = A                        (identity)
A ∩ U  = A                        (identity)
A ∪ U  = U                        (domination)
A ∩ ∅  = ∅                        (domination)
A ∩ (B ∪ C) = (A ∩ B) ∪ (A ∩ C)   (distributive)
A ∪ (B ∩ C) = (A ∪ B) ∩ (A ∪ C)   (distributive)
A ∩ B ⊆ A ⊆ A ∪ B                 (size ordering)
```

---

### Day 3 — Symbols cheat sheet

| Symbol | Meaning |
|---|---|
| `A ∪ B` | Union — everything in A or B (or both) |
| `A ∩ B` | Intersection — only what is in both A and B |
| `∪` | OR |
| `∩` | AND |
| `A ∩ B = ∅` | A and B are disjoint (no shared elements) |
| `U` | Universal set — the master set |

---

### Day 3 — Practice problems

### Basic

**1.** Let `A = {a, b, c, d}` and `B = {c, d, e, f}`. Find:
   - a) `A ∪ B`
   - b) `A ∩ B`

**2.** Let `P = {2, 4, 6, 8, 10}` and `Q = {1, 3, 5, 7, 9}`. Find:
   - a) `P ∪ Q`
   - b) `P ∩ Q`
   - c) Are P and Q disjoint? Why?

**3.** Let `X = {1, 2, 3}` and `Y = {1, 2, 3, 4, 5}`. Find `X ∪ Y` and `X ∩ Y`. What do you notice?

### Intermediate

**4.** Let `A = {1, 2, 3, 4, 5, 6}`, `B = {2, 4, 6, 8}`, `C = {1, 3, 5, 7}`. Find:
   - a) `A ∩ B`
   - b) `A ∩ C`
   - c) `B ∩ C`
   - d) `A ∪ B ∪ C`
   - e) `A ∩ B ∩ C`

**5.** Using the same sets from Q4, verify the distributive law:
   `A ∩ (B ∪ C) = (A ∩ B) ∪ (A ∩ C)`

**6.** Let `A = {x | x is a multiple of 2, 1 ≤ x ≤ 20}` and `B = {x | x is a multiple of 3, 1 ≤ x ≤ 20}`. Find `A ∩ B`. What kind of numbers are these?

### Challenge

**7.** Prove that if `A ⊆ B`, then `A ∪ B = B`.

**8.** Prove that if `A ⊆ B`, then `A ∩ B = A`.

**9.** A class of 30 students: 18 study French, 15 study Spanish, and 7 study both. Draw a Venn diagram and find:
   - a) How many study French only?
   - b) How many study Spanish only?
   - c) How many study at least one language?
   - d) How many study neither language?

*(Note: The formula for cardinality of a union is covered fully on Day 5. Try to solve this using the Venn diagram alone.)*

---

### Answers

**1.**
- a) `A ∪ B = {a, b, c, d, e, f}`
- b) `A ∩ B = {c, d}`

**2.**
- a) `P ∪ Q = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}`
- b) `P ∩ Q = ∅`
- c) Yes — P contains only even numbers and Q contains only odd numbers. They share no elements, so P ∩ Q = ∅.

**3.**
- `X ∪ Y = {1, 2, 3, 4, 5} = Y`
- `X ∩ Y = {1, 2, 3} = X`
- Notice: because X ⊆ Y, the union gives Y and the intersection gives X. This confirms the laws: if A ⊆ B then A ∪ B = B and A ∩ B = A.

**4.**
- a) `A ∩ B = {2, 4, 6}`
- b) `A ∩ C = {1, 3, 5}`
- c) `B ∩ C = ∅` (B has only even numbers, C has only odd numbers — disjoint)
- d) `A ∪ B ∪ C = {1, 2, 3, 4, 5, 6, 7, 8}`
- e) `A ∩ B ∩ C = ∅` (since B ∩ C = ∅, the triple intersection is also ∅)

**5.**
- Left side: `B ∪ C = {1, 2, 3, 4, 5, 6, 7, 8}`, then `A ∩ (B ∪ C) = {1, 2, 3, 4, 5, 6}`
- Right side: `(A ∩ B) ∪ (A ∩ C) = {2,4,6} ∪ {1,3,5} = {1, 2, 3, 4, 5, 6}`
- Both sides equal `{1, 2, 3, 4, 5, 6}` ✓ — distributive law verified.

**6.**
- `A = {2, 4, 6, 8, 10, 12, 14, 16, 18, 20}` (multiples of 2)
- `B = {3, 6, 9, 12, 15, 18}` (multiples of 3)
- `A ∩ B = {6, 12, 18}` — these are multiples of **6** (i.e., multiples of both 2 and 3, which means multiples of lcm(2,3) = 6).

**7.** Proof that if `A ⊆ B`, then `A ∪ B = B`:
- We must show (i) `A ∪ B ⊆ B` and (ii) `B ⊆ A ∪ B`.
- (i) Let `x ∈ A ∪ B`. Then x ∈ A or x ∈ B. If x ∈ B, done. If x ∈ A, then since A ⊆ B, x ∈ B. Either way, x ∈ B. So `A ∪ B ⊆ B`.
- (ii) Let `x ∈ B`. Then certainly x ∈ A or x ∈ B (it satisfies the OR). So `x ∈ A ∪ B`. Thus `B ⊆ A ∪ B`.
- From (i) and (ii): `A ∪ B = B`. ∎

**8.** Proof that if `A ⊆ B`, then `A ∩ B = A`:
- (i) `A ∩ B ⊆ A`: Let `x ∈ A ∩ B`. Then x ∈ A and x ∈ B. In particular, x ∈ A. So `A ∩ B ⊆ A`.
- (ii) `A ⊆ A ∩ B`: Let `x ∈ A`. Since A ⊆ B, x ∈ B as well. So x ∈ A and x ∈ B, meaning `x ∈ A ∩ B`. Thus `A ⊆ A ∩ B`.
- From (i) and (ii): `A ∩ B = A`. ∎

**9.** Venn diagram setup:

```
  Let the two circles be F (French) and S (Spanish).
  Middle overlap (both) = 7

  French only  = 18 − 7 = 11
  Spanish only = 15 − 7 = 8
```

- a) French only = **11 students**
- b) Spanish only = **8 students**
- c) At least one language = 11 + 7 + 8 = **26 students**
- d) Neither = 30 − 26 = **4 students**

---

### Connection to Day 4

On Day 4 you will learn **Complement (A')** and **Set Difference (A − B)** — which together with union and intersection complete the full toolkit of set operations. You will also prove **De Morgan's Laws**, which reveal a beautiful symmetry between complement, union, and intersection.


