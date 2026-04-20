# Day 4 — Complement & Set Difference

---

### Recap from Day 3

Before starting, make sure you are comfortable with:

- `A ∪ B` — union: everything in A **or** B (or both)
- `A ∩ B` — intersection: only what is in **both** A and B
- Disjoint sets: `A ∩ B = ∅` — no shared elements
- Commutative, associative, distributive, and identity laws
- `A ∩ B ⊆ A ⊆ A ∪ B` — the size ordering of operations

---

### Concept 1 — The Universal Set (U)

Before we can talk about complements, we need one new idea: the **universal set**.

The **universal set** `U` is the master collection — the set of **all possible elements** relevant to a given problem. Everything we discuss lives inside U.

```
U  =  the "world" that all our sets are drawn from
```

### Examples

| Context | Universal set U |
|---|---|
| Discussing digits | `U = {0, 1, 2, 3, 4, 5, 6, 7, 8, 9}` |
| Discussing letters | `U = {a, b, c, ..., z}` |
| Discussing integers 1–10 | `U = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}` |
| Discussing students in a school | `U = {all students in the school}` |

### Why it matters

The complement of a set depends entirely on what U is. Change U, and the complement changes. Always read a problem carefully to identify U before finding any complement.

---

### Concept 2 — Complement of a Set (A')

The **complement** of set A, written `A'` (read: *"A prime"* or *"A complement"*), is the set of all elements in U that are **not** in A.

```
A'  =  { x | x ∈ U  and  x ∉ A }
```

In other words: everything in the universal set that A left out.

### Step-by-step example

Let `U = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}` and `A = {2, 4, 6, 8, 10}`

- Go through every element of U.
- If it is **not** in A, it belongs to A'.

```
A'  =  {1, 3, 5, 7, 9}
```

A contains the even numbers, so A' contains the odd numbers.

### Venn diagram — complement

```
  ┌─────────────────────────────────────┐
  │               U                     │
  │                                     │
  │    ╔══════════════╗                 │
  │    ║              ║                 │
  │    ║      A       ║                 │
  │    ║              ║                 │
  │    ╚══════════════╝                 │
  │                                     │
  │  ← A' is everything OUTSIDE the     │
  │    circle, but still inside U       │
  └─────────────────────────────────────┘

  A  = shaded circle (inner region)
  A' = shaded region outside the circle, inside U
```

### Key properties of complement

```
(A')'  =  A                  Double complement returns the original set
A ∪ A' =  U                  A set and its complement together make U
A ∩ A' =  ∅                  A set and its complement share nothing
U'     =  ∅                  The complement of U is empty
∅'     =  U                  The complement of the empty set is U
```

### Critical warning ⚠️

The complement **always depends on U**. The same set A has a different complement for every different U.

Example:
- If `U = {1,2,3,4,5}` and `A = {1,2}`, then `A' = {3,4,5}`
- If `U = {1,2,3,4,5,6,7}` and `A = {1,2}`, then `A' = {3,4,5,6,7}`

Never find a complement without first identifying U.

---

### Concept 3 — Set Difference (A − B)

The **set difference** A minus B, written `A − B` (also written `A \ B`), is the set of all elements that are in A but **not** in B.

```
A − B  =  { x | x ∈ A  and  x ∉ B }
```

Read as: *"A minus B"* or *"A less B."*

Think of it as: start with A, then **remove** any element that also appears in B.

### Step-by-step example

Let `A = {1, 2, 3, 4, 5}` and `B = {3, 4, 5, 6, 7}`

**Finding A − B:**
- 1: in A, not in B → **keep**
- 2: in A, not in B → **keep**
- 3: in A, but also in B → **remove**
- 4: in A, but also in B → **remove**
- 5: in A, but also in B → **remove**

```
A − B  =  {1, 2}
```

**Finding B − A:**
- 3: in B, also in A → **remove**
- 4: in B, also in A → **remove**
- 5: in B, also in A → **remove**
- 6: in B, not in A → **keep**
- 7: in B, not in A → **keep**

```
B − A  =  {6, 7}
```

### Key observation

`A − B ≠ B − A` in general. Set difference is **not commutative**.

### Venn diagram — set difference

```
        A                B
   ___________      ___________
  /           \    /           \
 / ░░░░░░░░░░░ \  /             \
|░░░░░░░░  ____| |____           |
|░░░░░░░░ |    | |    |          |
 \░░░░░░░░|___/ \ \___|          /
  \░░░░░░░/      \              /
   \_______/      \____________/

  A − B  =  shade the LEFT part of A only
             (the part of A that does NOT overlap with B)
```

### Relationship between set difference and complement

If you have a universal set U, then:

```
A − B  =  A ∩ B'
```

This is very useful — it lets you convert a set difference into an intersection problem.

**Proof:**
- `x ∈ A − B` means x ∈ A and x ∉ B
- x ∉ B means x ∈ B' (by definition of complement)
- So x ∈ A and x ∈ B', which means x ∈ A ∩ B'
- Therefore `A − B = A ∩ B'` ∎

---

### Concept 4 — Symmetric Difference (A △ B)

The **symmetric difference** of A and B, written `A △ B`, is the set of elements that are in A or B, but **not in both**.

```
A △ B  =  { x | x ∈ A  OR  x ∈ B,  but  x ∉ A ∩ B }
```

Think of it as the union **minus** the intersection — everything except the middle overlap.

### Alternative formula

```
A △ B  =  (A − B) ∪ (B − A)  =  (A ∪ B) − (A ∩ B)
```

### Step-by-step example

Let `A = {1, 2, 3, 4}` and `B = {3, 4, 5, 6}`

- `A − B = {1, 2}` (in A only)
- `B − A = {5, 6}` (in B only)
- `A △ B = {1, 2} ∪ {5, 6} = {1, 2, 5, 6}`

Alternatively: `A ∪ B = {1,2,3,4,5,6}`, `A ∩ B = {3,4}`, so `A △ B = {1,2,5,6}` ✓

### Venn diagram — symmetric difference

```
        A                B
   ___________      ___________
  /░░░░░░░░░░░\    /░░░░░░░░░░░\
 /░░░░░░░░░░░░ \  / ░░░░░░░░░░░ \
|░░░░░░  ______| |______  ░░░░░░|
|░░░░░░ |      | |      | ░░░░░░|
 \░░░░░░|_____/ \ \_____| ░░░░░/
  \░░░░░░░░░░/   \░░░░░░░░░░░/
   \_________/    \_________/

  A △ B = shade the LEFT and RIGHT parts only
          (NOT the middle overlap)
```

---

### Concept 5 — De Morgan's Laws

De Morgan's Laws are two of the most powerful and elegant results in set theory. They describe how complement interacts with union and intersection.

### First De Morgan's Law

```
(A ∪ B)'  =  A' ∩ B'
```

*"The complement of a union equals the intersection of the complements."*

### Second De Morgan's Law

```
(A ∩ B)'  =  A' ∪ B'
```

*"The complement of an intersection equals the union of the complements."*

### Memory trick

When you move the complement **inside**, the operation **flips**:
- Union `∪` becomes Intersection `∩`
- Intersection `∩` becomes Union `∪`

It works exactly like the logical NOT rule in Boolean algebra:
```
NOT (A OR B)   =   (NOT A) AND (NOT B)
NOT (A AND B)  =   (NOT A) OR  (NOT B)
```

---

### Concept 6 — Proving De Morgan's Laws

### Proof of (A ∪ B)' = A' ∩ B'

We prove both inclusions.

**Part 1: Show `(A ∪ B)' ⊆ A' ∩ B'`**

Let `x ∈ (A ∪ B)'`  
→ x ∉ A ∪ B (by definition of complement)  
→ x ∉ A AND x ∉ B (if x were in either, it would be in the union)  
→ x ∈ A' AND x ∈ B' (by definition of complement)  
→ x ∈ A' ∩ B'  
∴ `(A ∪ B)' ⊆ A' ∩ B'` ✓

**Part 2: Show `A' ∩ B' ⊆ (A ∪ B)'`**

Let `x ∈ A' ∩ B'`  
→ x ∈ A' AND x ∈ B'  
→ x ∉ A AND x ∉ B  
→ x ∉ A ∪ B (x is in neither set, so it can't be in their union)  
→ x ∈ (A ∪ B)'  
∴ `A' ∩ B' ⊆ (A ∪ B)'` ✓

Since both inclusions hold: `(A ∪ B)' = A' ∩ B'` ∎

---

### Numerical verification of De Morgan's Laws

Let `U = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}`, `A = {1, 2, 3, 4}`, `B = {3, 4, 5, 6}`

**Verifying (A ∪ B)' = A' ∩ B':**

| Step | Calculation | Result |
|---|---|---|
| `A ∪ B` | Combine A and B | `{1, 2, 3, 4, 5, 6}` |
| `(A ∪ B)'` | Remove from U | `{7, 8, 9, 10}` |
| `A'` | Elements of U not in A | `{5, 6, 7, 8, 9, 10}` |
| `B'` | Elements of U not in B | `{1, 2, 7, 8, 9, 10}` |
| `A' ∩ B'` | Common elements | `{7, 8, 9, 10}` |

Both sides equal `{7, 8, 9, 10}` ✓

**Verifying (A ∩ B)' = A' ∪ B':**

| Step | Calculation | Result |
|---|---|---|
| `A ∩ B` | Common elements | `{3, 4}` |
| `(A ∩ B)'` | Remove from U | `{1, 2, 5, 6, 7, 8, 9, 10}` |
| `A'` | (from above) | `{5, 6, 7, 8, 9, 10}` |
| `B'` | (from above) | `{1, 2, 7, 8, 9, 10}` |
| `A' ∪ B'` | Combine complements | `{1, 2, 5, 6, 7, 8, 9, 10}` |

Both sides equal `{1, 2, 5, 6, 7, 8, 9, 10}` ✓

---

### Concept 7 — All four operations compared

Using `U = {1,2,3,4,5,6,7,8,9,10}`, `A = {1,2,3,4,5}`, `B = {4,5,6,7,8}`:

| Operation | Formula | Result | Venn region shaded |
|---|---|---|---|
| Union | `A ∪ B` | `{1,2,3,4,5,6,7,8}` | Both circles |
| Intersection | `A ∩ B` | `{4,5}` | Middle overlap only |
| Complement of A | `A'` | `{6,7,8,9,10}` | Outside A circle |
| Set difference | `A − B` | `{1,2,3}` | Left of A only |
| Set difference | `B − A` | `{6,7,8}` | Right of B only |
| Symmetric difference | `A △ B` | `{1,2,3,6,7,8}` | Both outer regions |
| De Morgan 1 | `(A ∪ B)'` | `{9,10}` | Outside both circles |
| De Morgan 2 | `(A ∩ B)'` | `{1,2,3,6,7,8,9,10}` | Everything except middle |

---

### Day 4 — Key results summary

```
A'       =  U − A                      Complement definition
(A')'    =  A                          Double complement
A ∪ A'   =  U                          Complement law
A ∩ A'   =  ∅                          Complement law
U'       =  ∅                          Complement of universal set
∅'       =  U                          Complement of empty set
A − B    =  A ∩ B'                     Set difference via complement
A △ B    =  (A − B) ∪ (B − A)          Symmetric difference
A △ B    =  (A ∪ B) − (A ∩ B)          Symmetric difference (alt.)
(A ∪ B)' =  A' ∩ B'                    De Morgan's First Law
(A ∩ B)' =  A' ∪ B'                    De Morgan's Second Law
```

---

### Day 4 — Symbols cheat sheet

| Symbol | Meaning |
|---|---|
| `U` | Universal set — the master set |
| `A'` or `Aᶜ` | Complement of A — everything in U not in A |
| `A − B` or `A \ B` | Set difference — elements in A but not in B |
| `A △ B` | Symmetric difference — in A or B, but not both |
| `(A ∪ B)'` | De Morgan 1 — equals A' ∩ B' |
| `(A ∩ B)'` | De Morgan 2 — equals A' ∪ B' |

---

### Day 4 — Practice problems

### Basic

**1.** Let `U = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}`, `A = {1, 3, 5, 7, 9}`, `B = {2, 3, 4, 5}`. Find:
   - a) `A'`
   - b) `B'`
   - c) `A − B`
   - d) `B − A`

**2.** Let `U = {a, b, c, d, e, f, g}`, `P = {a, c, e, g}`, `Q = {b, c, d, e}`. Find:
   - a) `P'`
   - b) `Q'`
   - c) `P △ Q`

**3.** For any set A, simplify:
   - a) `A ∪ A'`
   - b) `A ∩ A'`
   - c) `(A')'`

### Intermediate

**4.** Let `U = {1,2,...,10}`, `A = {2,4,6,8,10}`, `B = {1,2,3,4,5}`. Verify De Morgan's First Law:
`(A ∪ B)' = A' ∩ B'`
Show all steps clearly.

**5.** Let `U = {1,2,...,12}`, `A = {1,2,3,4,5,6}`, `B = {4,5,6,7,8,9}`. Find:
   - a) `A − B`
   - b) `B − A`
   - c) `A △ B`
   - d) Verify that `A △ B = (A ∪ B) − (A ∩ B)`

**6.** Express `A − B` using only the symbols `∩` and `'` (no minus sign).

**7.** If `A ⊆ B`, what is `A − B`? Justify your answer.

### Challenge

**8.** Prove De Morgan's Second Law: `(A ∩ B)' = A' ∪ B'`
Use the element-checking method (prove both inclusions).

**9.** Prove that `A △ B = (A ∪ B) − (A ∩ B)`.

**10.** Let `U = {1, 2, 3, ..., 20}`.
   - `A = {x | x is a multiple of 2}`
   - `B = {x | x is a multiple of 3}`
   - `C = {x | x is a multiple of 5}`

   Find:
   - a) `A'` — what kind of numbers are these?
   - b) `A ∩ B` — what is the pattern?
   - c) `(A ∪ B)'` — verify with De Morgan's Law
   - d) `A − C`

---

### Answers

**1.**
- a) `A' = {2, 4, 6, 8, 10}` (even numbers — the non-odd elements of U)
- b) `B' = {1, 6, 7, 8, 9, 10}`
- c) `A − B = {1, 7, 9}` (elements of A not in B — remove 3 and 5)
- d) `B − A = {2, 4}` (elements of B not in A — remove 3 and 5)

**2.**
- a) `P' = {b, d, f}` (elements of U not in P)
- b) `Q' = {a, f, g}` (elements of U not in Q)
- c) `P − Q = {a, g}`, `Q − P = {b, d}`, so `P △ Q = {a, b, d, g}`

**3.**
- a) `A ∪ A' = U`
- b) `A ∩ A' = ∅`
- c) `(A')' = A`

**4.**
- `A ∪ B = {1,2,3,4,5,6,8,10}`
- `(A ∪ B)' = {7, 9}` ← Left side
- `A' = {1,3,5,7,9}`, `B' = {6,7,8,9,10}`
- `A' ∩ B' = {7, 9}` ← Right side
- Both equal `{7, 9}` ✓ De Morgan's First Law verified.

**5.**
- a) `A − B = {1, 2, 3}` (elements in A but not in B)
- b) `B − A = {7, 8, 9}` (elements in B but not in A)
- c) `A △ B = {1, 2, 3, 7, 8, 9}`
- d) `A ∪ B = {1,2,3,4,5,6,7,8,9}`, `A ∩ B = {4,5,6}`, `(A ∪ B) − (A ∩ B) = {1,2,3,7,8,9}` ✓

**6.** `A − B = A ∩ B'`
(Elements in A that are not in B means elements in A that are in B's complement.)

**7.** If `A ⊆ B`, then `A − B = ∅`.
- Every element of A is already in B, so there is nothing left after removing B's elements from A.

**8.** Proof of `(A ∩ B)' = A' ∪ B'`:

Part 1: Show `(A ∩ B)' ⊆ A' ∪ B'`

Let `x ∈ (A ∩ B)'`  
→ x ∉ A ∩ B  
→ NOT (x ∈ A AND x ∈ B)  
→ x ∉ A OR x ∉ B  
→ x ∈ A' OR x ∈ B'  
→ x ∈ A' ∪ B' ✓

Part 2: Show `A' ∪ B' ⊆ (A ∩ B)'`

Let `x ∈ A' ∪ B'`  
→ x ∈ A' OR x ∈ B'  
→ x ∉ A OR x ∉ B  
→ NOT (x ∈ A AND x ∈ B)  
→ x ∉ A ∩ B  
→ x ∈ (A ∩ B)' ✓

Since both inclusions hold: `(A ∩ B)' = A' ∪ B'` ∎

**9.** Proof that `A △ B = (A ∪ B) − (A ∩ B)`:

Let `x ∈ A △ B`  
→ x ∈ (A − B) ∪ (B − A) (by definition)  
→ (x ∈ A and x ∉ B) OR (x ∈ B and x ∉ A)  
→ x ∈ A ∪ B (x is in at least one)  
AND x ∉ A ∩ B (x is not in both simultaneously)  
→ x ∈ (A ∪ B) − (A ∩ B) ✓

The reverse direction follows the same steps in reverse. ∎

**10.**
- `A = {2,4,6,8,10,12,14,16,18,20}`, `B = {3,6,9,12,15,18}`, `C = {5,10,15,20}`
- a) `A' = {1,3,5,7,9,11,13,15,17,19}` — odd numbers
- b) `A ∩ B = {6,12,18}` — multiples of 6 (lcm of 2 and 3)
- c) `A ∪ B = {2,3,4,6,8,9,10,12,14,15,16,18,20}`, `(A ∪ B)' = {1,5,7,11,13,17,19}`. Via De Morgan: `A' ∩ B' = {1,5,7,11,13,17,19}` ✓
- d) `A − C = {2,4,6,8,12,14,16,18}` (remove multiples of 5 from A: remove 10 and 20)

---

### Connection to Day 5

On Day 5 you will learn **Cardinality and Counting** — including the powerful inclusion-exclusion formula:

```
|A ∪ B|  =  |A|  +  |B|  −  |A ∩ B|
```

Everything you learned today — especially complements and set differences — feeds directly into this formula and makes complex word problems straightforward to solve.

