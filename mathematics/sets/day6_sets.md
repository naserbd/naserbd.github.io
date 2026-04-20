# Day 6 — Cartesian Product & Relations

---

### Recap from Day 5

Before starting, make sure you are comfortable with:

- `|A ∪ B| = |A| + |B| − |A ∩ B|` — two-set inclusion-exclusion
- `|A ∪ B ∪ C|` — three-set inclusion-exclusion formula
- `|A'| = |U| − |A|` — cardinality of complement
- `|A − B| = |A| − |A ∩ B|` — cardinality of set difference
- `|A △ B| = |A| + |B| − 2|A ∩ B|` — cardinality of symmetric difference
- The 8-region three-set Venn diagram and how to fill it inside-out

---

### Concept 1 — Ordered Pairs

Before we can define the Cartesian product, we need to understand **ordered pairs**.

An **ordered pair** is a pair of objects written in a specific order inside parentheses:

```
(a, b)
```

The first element `a` is called the **first component** and `b` is the **second component**.

### Order matters — this is the critical difference from sets

In a **set**, order does not matter: `{1, 2} = {2, 1}`

In an **ordered pair**, order matters completely: `(1, 2) ≠ (2, 1)`

Two ordered pairs `(a, b)` and `(c, d)` are equal **if and only if**:
```
a = c   AND   b = d   (both components match in position)
```

### Examples

| Statement | True or False? | Reason |
|---|---|---|
| `(3, 5) = (3, 5)` | ✅ True | Both components match |
| `(3, 5) = (5, 3)` | ❌ False | First components differ |
| `(2, 2) = (2, 2)` | ✅ True | Identical pairs |
| `(a, b) = (b, a)` | Only if `a = b` | Components must match positionally |

### Real-world connection

A GPS coordinate like (−27.47, 153.02) is an ordered pair — latitude first, then longitude.
Swapping them to (153.02, −27.47) points to a completely different location on Earth.

---

### Concept 2 — The Cartesian Product (A × B)

The **Cartesian product** of sets A and B, written `A × B` (read: *"A cross B"*), is the set of **all possible ordered pairs** where the first element comes from A and the second comes from B.

```
A × B  =  { (a, b) | a ∈ A  and  b ∈ B }
```

### Step-by-step example 1

Let `A = {1, 2, 3}` and `B = {x, y}`

List every possible (A-element, B-element) combination:

```
A × B  =  { (1,x), (1,y), (2,x), (2,y), (3,x), (3,y) }
```

Systematic method — build row by row:
- First element = 1: (1,x), (1,y)
- First element = 2: (2,x), (2,y)
- First element = 3: (3,x), (3,y)

### Step-by-step example 2

Let `P = {a, b}` and `Q = {1, 2, 3}`

```
P × Q  =  { (a,1), (a,2), (a,3), (b,1), (b,2), (b,3) }
```

### The grid (table) method

The most reliable way to list all pairs is to draw a table:

For `A = {1, 2, 3}` and `B = {x, y}`:

```
        B: x        B: y
A: 1  | (1, x)  |  (1, y)  |
A: 2  | (2, x)  |  (2, y)  |
A: 3  | (3, x)  |  (3, y)  |
```

Each cell in the table is one ordered pair. The total number of cells = `|A| × |B|`.

---

### Concept 3 — Cardinality of the Cartesian Product

```
|A × B|  =  |A|  ×  |B|
```

### Why?

For each of the `|A|` elements in A, you can pair it with any of the `|B|` elements in B. That gives `|A| × |B|` total combinations.

### Examples

| A | B | \|A\| | \|B\| | \|A × B\| |
|---|---|---|---|---|
| `{1, 2, 3}` | `{x, y}` | 3 | 2 | 6 |
| `{a, b}` | `{1, 2, 3}` | 2 | 3 | 6 |
| `{p, q, r, s}` | `{0, 1}` | 4 | 2 | 8 |
| `∅` | `{1, 2, 3}` | 0 | 3 | 0 |
| `{a}` | `{a}` | 1 | 1 | 1 |

### Important note — order matters for the product

`A × B ≠ B × A` in general (unless A = B).

- `A × B` has pairs (a, b) — A-element first
- `B × A` has pairs (b, a) — B-element first

However, `|A × B| = |B × A|` — the cardinalities are always equal.

---

### Concept 4 — Cartesian Product is Not Commutative or Associative

### Not commutative

```
A × B  ≠  B × A   (in general)
```

**Example:** `A = {1, 2}`, `B = {p, q}`

- `A × B = {(1,p), (1,q), (2,p), (2,q)}`
- `B × A = {(p,1), (p,2), (q,1), (q,2)}`

These are completely different sets of pairs.

**Exception:** `A × B = B × A` if and only if `A = B` or at least one of them is `∅`.

### Not associative

```
(A × B) × C  ≠  A × (B × C)   (in general)
```

- `(A × B) × C` produces pairs of the form `((a, b), c)`
- `A × (B × C)` produces pairs of the form `(a, (b, c))`

These are structurally different objects.

---

### Concept 5 — Cartesian Product with More Than Two Sets

The Cartesian product extends naturally to three or more sets:

```
A × B × C  =  { (a, b, c) | a ∈ A, b ∈ B, c ∈ C }
```

These are called **ordered triples**. More generally, with n sets you get **ordered n-tuples**.

```
|A × B × C|  =  |A| × |B| × |C|
```

### Example

Let `A = {0, 1}`, `B = {0, 1}`, `C = {0, 1}`

```
A × B × C  =  { (0,0,0), (0,0,1), (0,1,0), (0,1,1),
                (1,0,0), (1,0,1), (1,1,0), (1,1,1) }
```

`|A × B × C| = 2 × 2 × 2 = 8`

This is exactly the set of all 3-bit binary strings — a beautiful connection to computer science.

### Special case — A × A

When both sets are the same, we write:

```
A × A  =  A²      (read: "A squared")
A × A × A  =  A³
```

The most famous example: `ℝ × ℝ = ℝ²` is the **coordinate plane** (all (x, y) points). `ℝ³` is three-dimensional space.

---

### Concept 6 — Connection to Coordinate Geometry

The **Cartesian plane** (the xy-coordinate system you use in algebra and geometry) is literally the Cartesian product `ℝ × ℝ`.

```
ℝ × ℝ  =  { (x, y) | x ∈ ℝ and y ∈ ℝ }
```

Every point on the coordinate plane is an ordered pair from `ℝ × ℝ`. This is why it is called the **Cartesian** plane — it was invented by René Descartes, the same mathematician whose name we use for the Cartesian product.

### Finite grids as Cartesian products

If `X = {1, 2, 3}` and `Y = {1, 2, 3}`, then `X × Y` is a 3×3 grid of 9 points:

```
Y
3 |  (1,3)  (2,3)  (3,3)
2 |  (1,2)  (2,2)  (3,2)
1 |  (1,1)  (2,1)  (3,1)
  +---------------------
     1      2      3     X
```

This grid structure is exactly what you use when plotting points in coordinate geometry.

---

### Concept 7 — Relations

A **relation** from set A to set B is any **subset** of `A × B`.

```
R  ⊆  A × B
```

In other words: a relation is a collection of selected ordered pairs from the Cartesian product. You choose which pairs to include — and that choice defines the relationship.

### Formal definition

If `(a, b) ∈ R`, we say **"a is related to b"** and write `a R b`.

### Step-by-step example

Let `A = {1, 2, 3}` and `B = {1, 2, 3, 4, 5, 6}`

Define R = "a divides b" (a is a factor of b):

- `1` divides: 1, 2, 3, 4, 5, 6 → pairs: (1,1),(1,2),(1,3),(1,4),(1,5),(1,6)
- `2` divides: 2, 4, 6 → pairs: (2,2),(2,4),(2,6)
- `3` divides: 3, 6 → pairs: (3,3),(3,6)

```
R  =  { (1,1),(1,2),(1,3),(1,4),(1,5),(1,6),(2,2),(2,4),(2,6),(3,3),(3,6) }
```

This is a valid relation because `R ⊆ A × B`.

### Domain and Range of a relation

| Term | Definition | Formula |
|---|---|---|
| **Domain** | The set of all first components used | `Dom(R) = { a | (a,b) ∈ R for some b }` |
| **Range** | The set of all second components used | `Ran(R) = { b | (a,b) ∈ R for some a }` |

**Example** using the "divides" relation above:

- `Dom(R) = {1, 2, 3}` (all first components)
- `Ran(R) = {1, 2, 3, 4, 5, 6}` (all second components)

### Another example

Let `A = {1, 2, 3, 4}`. Define R on A × A as: `R = {(a,b) | a < b}`

```
R  =  { (1,2),(1,3),(1,4),(2,3),(2,4),(3,4) }
```

- `Dom(R) = {1, 2, 3}` (4 is never the smaller element)
- `Ran(R) = {2, 3, 4}` (1 is never the larger element)

---

### Concept 8 — Representing Relations

There are three standard ways to represent a relation.

### Method 1 — Roster (list of pairs)

Simply list all ordered pairs in the relation:

```
R  =  { (1,2), (1,4), (2,3), (3,1) }
```

### Method 2 — Arrow diagram (mapping diagram)

Draw two ovals (one for A, one for B). Draw an arrow from `a` to `b` whenever `(a,b) ∈ R`.

```
A          B
●1  ──────→ ●2
●1  ──────────→ ●4
●2  ───────────→ ●3
●3  ──────→ ●1
```

### Method 3 — Matrix representation

Create a matrix with rows for A and columns for B. Place `1` if `(a,b) ∈ R`, place `0` if not.

For `A = B = {1, 2, 3}` and `R = {(1,2),(1,3),(2,3),(3,1)}`:

```
      b=1   b=2   b=3
a=1 [  0     1     1  ]
a=2 [  0     0     1  ]
a=3 [  1     0     0  ]
```

---

### Day 6 — Key results summary

```
(a,b) = (c,d)   ⟺   a=c AND b=d         Ordered pair equality
A × B = {(a,b) | a∈A, b∈B}              Cartesian product definition
|A × B| = |A| × |B|                      Cardinality formula
A × B ≠ B × A   (in general)             Not commutative
A × ∅ = ∅                                Product with empty set
ℝ × ℝ = ℝ²  =  coordinate plane         Geometric connection
R ⊆ A × B                                A relation is a subset
Dom(R) = {a | (a,b)∈R}                  Domain of a relation
Ran(R) = {b | (a,b)∈R}                  Range of a relation
```

---

### Day 6 — Symbols and terms cheat sheet

| Symbol / Term | Meaning |
|---|---|
| `(a, b)` | Ordered pair — order matters |
| `A × B` | Cartesian product of A and B |
| `\|A × B\|` | Cardinality: `\|A\| × \|B\|` |
| `A²` | `A × A` — all ordered pairs from A with itself |
| `ℝ²` | The coordinate plane: `ℝ × ℝ` |
| `R ⊆ A × B` | R is a relation from A to B |
| `(a,b) ∈ R` | "a is related to b" — written `a R b` |
| `Dom(R)` | Domain — set of all first components in R |
| `Ran(R)` | Range — set of all second components in R |
| Ordered triple | Element of `A × B × C`: written `(a, b, c)` |

---

### Day 6 — Practice problems

### Basic

**1.** Let `A = {1, 2}` and `B = {a, b, c}`. Find:
   - a) `A × B`
   - b) `B × A`
   - c) `|A × B|`
   - d) Are `A × B` and `B × A` equal?

**2.** Let `P = {x, y}` and `Q = {x, y}`. Find `P × Q`. Is `P × Q = Q × P` here? Why?

**3.** If `|A| = 4` and `|B| = 6`, find:
   - a) `|A × B|`
   - b) `|B × A|`
   - c) `|A × A|`
   - d) `|A × B × A|`

**4.** Find the ordered pairs `(x, y)` such that `(2x − 1, y + 3) = (5, 7)`.

### Intermediate

**5.** Let `A = {1, 2, 3}` and `B = {2, 4, 6}`. List all elements of `A × B` and shade on a coordinate grid the points that form this set.

**6.** Let `A = {1, 2, 3, 4}`. Define the relation R on A as:
`R = {(a, b) | a + b = 5, a ∈ A, b ∈ A}`
   - a) List all elements of R.
   - b) Find Dom(R) and Ran(R).
   - c) Represent R as an arrow diagram.

**7.** Let `A = {2, 3, 4, 6}` and `B = {2, 3, 6, 9, 12}`. Define:
`R = {(a, b) | a divides b, a ∈ A, b ∈ B}`
   - a) List all elements of R.
   - b) Find Dom(R) and Ran(R).
   - c) Write the matrix representation of R.

**8.** A = {1, 2, 3} and B = {1, 4, 9}. Define R: "a² = b".
   - a) List all elements of R.
   - b) Is every element of A used? Is every element of B used?
   - c) What is Dom(R) and Ran(R)?

### Challenge

**9.** Prove that `A × (B ∪ C) = (A × B) ∪ (A × C)`.

**10.** Prove that `A × (B ∩ C) = (A × B) ∩ (A × C)`.

**11.** Let `|A × B| = 24` and `|A| + |B| = 10`. Find all possible values of `|A|` and `|B|`.

**12.** How many relations are possible from a set A with `|A| = 3` to a set B with `|B| = 2`?
*(Hint: a relation is any subset of A × B. How many subsets does A × B have?)*

---

### Answers

**1.**
- a) `A × B = {(1,a),(1,b),(1,c),(2,a),(2,b),(2,c)}`
- b) `B × A = {(a,1),(a,2),(b,1),(b,2),(c,1),(c,2)}`
- c) `|A × B| = 2 × 3 = 6`
- d) No. The pairs have components in opposite order — e.g. `(1,a) ≠ (a,1)`.

**2.**
- `P × Q = {(x,x),(x,y),(y,x),(y,y)}`
- Yes, `P × Q = Q × P` here because P = Q. When the two sets are equal, the product is the same regardless of order.

**3.**
- a) `|A × B| = 4 × 6 = 24`
- b) `|B × A| = 6 × 4 = 24`
- c) `|A × A| = 4 × 4 = 16`
- d) `|A × B × A| = 4 × 6 × 4 = 96`

**4.**
Equate components:
- `2x − 1 = 5` → `2x = 6` → `x = 3`
- `y + 3 = 7` → `y = 4`
- Answer: `(x, y) = (3, 4)`

**5.**
```
A × B = {(1,2),(1,4),(1,6),(2,2),(2,4),(2,6),(3,2),(3,4),(3,6)}
```
On a coordinate grid, these are 9 points forming a 3×3 arrangement at x ∈ {1,2,3} and y ∈ {2,4,6}.

**6.**
- a) Pairs where a + b = 5: (1,4),(2,3),(3,2),(4,1) — all with both components in A.
  `R = {(1,4),(2,3),(3,2),(4,1)}`
- b) `Dom(R) = {1,2,3,4}`, `Ran(R) = {1,2,3,4}`
- c) Arrow diagram: 1→4, 2→3, 3→2, 4→1 (each element maps to its "partner" that sums to 5)

**7.**
Check each (a,b) pair:
- 2 divides: 2 ✓, 6 ✓, 12 ✓
- 3 divides: 3 ✓, 6 ✓, 9 ✓, 12 ✓
- 4 divides: 12 ✓
- 6 divides: 6 ✓, 12 ✓

- a) `R = {(2,2),(2,6),(2,12),(3,3),(3,6),(3,9),(3,12),(4,12),(6,6),(6,12)}`
- b) `Dom(R) = {2,3,4,6}`, `Ran(R) = {2,3,6,9,12}`
- c) Matrix (rows = A elements, columns = B elements, in order 2,3,6,9,12):

```
      2   3   6   9  12
  2 [ 1   0   1   0   1 ]
  3 [ 0   1   1   1   1 ]
  4 [ 0   0   0   0   1 ]
  6 [ 0   0   1   0   1 ]
```

**8.**
- a) 1²=1 ✓, 2²=4 ✓, 3²=9 ✓ → `R = {(1,1),(2,4),(3,9)}`
- b) Every element of A is used as a first component. Every element of B is used as a second component.
- c) `Dom(R) = {1,2,3} = A`, `Ran(R) = {1,4,9} = B`

**9.** Proof that `A × (B ∪ C) = (A × B) ∪ (A × C)`:

Let `(x,y) ∈ A × (B ∪ C)`  
→ x ∈ A and y ∈ B ∪ C  
→ x ∈ A and (y ∈ B or y ∈ C)  
→ (x ∈ A and y ∈ B) or (x ∈ A and y ∈ C)  
→ (x,y) ∈ A × B or (x,y) ∈ A × C  
→ (x,y) ∈ (A × B) ∪ (A × C)

Reverse direction follows the same steps in reverse. ∎

**10.** Proof that `A × (B ∩ C) = (A × B) ∩ (A × C)`:

Let `(x,y) ∈ A × (B ∩ C)`  
→ x ∈ A and y ∈ B ∩ C  
→ x ∈ A and (y ∈ B and y ∈ C)  
→ (x ∈ A and y ∈ B) and (x ∈ A and y ∈ C)  
→ (x,y) ∈ A × B and (x,y) ∈ A × C  
→ (x,y) ∈ (A × B) ∩ (A × C)

Reverse direction follows the same steps in reverse. ∎

**11.**
We need `|A| × |B| = 24` and `|A| + |B| = 10`.
Find factor pairs of 24 that sum to 10:
- 1 × 24 = 24, sum = 25 ✗
- 2 × 12 = 24, sum = 14 ✗
- 3 × 8 = 24, sum = 11 ✗
- **4 × 6 = 24, sum = 10 ✓**
- 6 × 4 = 24, sum = 10 ✓ (same pair, reversed)

The only solution is `|A| = 4, |B| = 6` or `|A| = 6, |B| = 4`.

**12.**
- `|A × B| = 3 × 2 = 6`
- A relation is any subset of A × B.
- Number of subsets of a 6-element set = `2⁶ = 64`
- Therefore, **64 relations** are possible from A to B.

---

### Connection to Day 7

On Day 7 — the final day — you will bring together **every concept from all six days** into a complete review. You will learn formal proof techniques, work through mixed problems spanning all topics, explore the common exam traps, and get a glimpse at what lies beyond: functions (which are special kinds of relations), infinite set theory, and university-level mathematics. Day 7 is where everything clicks into a single, unified picture.

