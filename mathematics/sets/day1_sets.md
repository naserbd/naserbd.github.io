# Day 1 — What Is a Set?

---

### Concept 1 — What is a set?

A **set** is a well-defined collection of distinct objects. The objects inside a set are called **elements** (or members).

### Three rules a set must follow

| Rule | Meaning |
|---|---|
| Well-defined | There must be no doubt whether an object belongs or not |
| Distinct | No element appears more than once |
| No order | {1, 2, 3} and {3, 1, 2} are the same set |

### Real-life examples

- Your school bag = `{book, pencil, ruler, lunch box}`
- Days of the week = `{Mon, Tue, Wed, Thu, Fri, Sat, Sun}`
- Even numbers less than 10 = `{2, 4, 6, 8}`

> We always write sets using `{ }` curly braces. This is the universal convention in mathematics.

---

### Concept 2 — The ∈ symbol (membership)

These two symbols are the most fundamental in set theory:

```
∈   means   "is an element of"
∉   means   "is NOT an element of"
```

### Example

Let `A = {cat, dog, rabbit, hamster}`

- `dog ∈ A` → TRUE — "dog is an element of A"
- `elephant ∉ A` → TRUE — "elephant is not an element of A"
- `cat ∉ A` → FALSE — cat IS in A, so this statement is wrong

### Practice

Given `B = {1, 3, 5, 7, 9}`, decide which of the following are true:

1. `2 ∈ B` → **False** (2 is not in B)
2. `5 ∈ B` → **True**
3. `9 ∉ B` → **False** (9 IS in B)
4. `4 ∉ B` → **True**

---

### Concept 3 — Roster notation

In **roster notation**, you list all the elements of a set, separated by commas, inside curly braces.

```
A = { element1, element2, element3, ... }
```

### Examples

| Description | Roster form |
|---|---|
| Vowels in English | `V = {a, e, i, o, u}` |
| Factors of 12 | `F = {1, 2, 3, 4, 6, 12}` |
| Months starting with J | `M = {January, June, July}` |
| Natural numbers (infinite) | `N = {1, 2, 3, 4, 5, ...}` |

The three dots `...` are called an **ellipsis**. They mean "the pattern continues forever."

### Common mistake to avoid

Writing `{1, 1, 2, 3}` is **not** a valid set — elements must be distinct.  
The correct set is `{1, 2, 3}`.

---

### Concept 4 — Set-builder notation

In **set-builder notation**, instead of listing every element, you describe the *rule* that an element must satisfy to belong to the set.

```
A = { x | condition on x }
```

Read the vertical bar `|` as *"such that"*.  
So the above reads: "A is the set of all x **such that** [some condition is true]."

### Roster vs Set-builder — side by side

| Roster form | Set-builder form |
|---|---|
| `A = {2, 4, 6, 8, 10}` | `A = {x \| x is even, x ≤ 10}` |
| `B = {1, 2, 3, 4, 5}` | `B = {x \| x ∈ ℕ, x ≤ 5}` |
| `C = {3, 6, 9, 12}` | `C = {x \| x is a multiple of 3, x ≤ 12}` |

### When to use each

- Use **roster** when the set is small and easy to list.
- Use **set-builder** when the set is large, infinite, or more naturally described by a rule — like "all real numbers between 0 and 1."

---

### Concept 5 — The empty set (∅)

The **empty set** (also called the null set) is a set that contains *no elements at all*.

```
Written as:  ∅   or   {}
```

### Examples of empty sets

- The set of months with 35 days → `∅` (no such month exists)
- The set of odd numbers divisible by 2 → `∅` (a number can't be both)
- The set of cats that speak English → `∅`

### Critical warning ⚠️

`∅` and `{∅}` are **NOT** the same thing!

| Symbol | Meaning | Cardinality |
|---|---|---|
| `∅` | The empty set — contains nothing | 0 elements |
| `{∅}` | A set *containing* the empty set | 1 element |

This is a very common exam trap. Read it carefully every time you see it.

> The empty set is extremely important in mathematics. Every set contains ∅ as a subset — you will learn why on Day 2.

---

### Concept 6 — Finite vs infinite sets

| | Finite set | Infinite set |
|---|---|---|
| Definition | Has a countable, fixed number of elements | Goes on forever — cannot be fully listed |
| Examples | `{Mon, Tue, Wed, Thu, Fri}` | `N = {1, 2, 3, 4, ...}` |
| | `{1, 2, 3, 4, 5}` | `Z = {..., -2, -1, 0, 1, 2, ...}` |
| | `∅` (0 elements — still finite!) | All real numbers between 0 and 1 |

### Cardinality

The **cardinality** of a set A, written `|A|`, is the number of elements it contains.

```
A = {a, e, i, o, u}   →   |A| = 5
B = ∅                 →   |B| = 0
N = {1, 2, 3, ...}    →   |N| = ∞
```

> Cardinality is explored in much more depth on Day 5, where some beautiful and surprising mathematics emerges.

---

### Concept 7 — Equal sets

Two sets are **equal** if and only if they contain exactly the same elements — regardless of order or repetition.

```
A = B  ⟺  every element of A is in B, AND every element of B is in A
```

### Examples

| Statement | Equal? | Reason |
|---|---|---|
| `{1, 2, 3} = {3, 2, 1}` | ✅ Yes | Order doesn't matter |
| `{a, a, b} = {a, b}` | ✅ Yes | Duplicates are ignored |
| `{1, 2, 3} ≠ {1, 2, 4}` | ❌ No | Different elements |
| `{1, 2} ≠ {1, 2, 3}` | ❌ No | Different cardinality |

---

### Day 1 — Symbols cheat sheet

| Symbol | Meaning |
|---|---|
| `{ }` | Curly braces — used to write a set |
| `∈` | Is an element of |
| `∉` | Is NOT an element of |
| `∅` | The empty set (no elements) |
| `\|A\|` | Cardinality — number of elements in A |
| `A = B` | Set equality — A and B have the same elements |

---

### Day 1 — Practice problems

Try these on your own before moving to Day 2.

**1.** Write the set of all letters in the word "MATHEMATICS" in roster form.

**2.** Let `P = {2, 4, 6, 8, 10}`. State whether each of the following is true or false:
   - a) `6 ∈ P`
   - b) `5 ∈ P`
   - c) `10 ∉ P`

**3.** Write the following set in set-builder notation: `{5, 10, 15, 20, 25}`

**4.** Find the cardinality of each set:
   - a) `A = {a, b, c, d, e}`
   - b) `B = {}`
   - c) `C = {1, 2, 3, ..., 100}`

**5.** Are these two sets equal? `X = {1, 3, 5}` and `Y = {5, 1, 3, 1}`. Justify your answer.

---

### Answers

1. `{M, A, T, H, E, I, C, S}` (8 distinct letters — duplicates removed)
2. a) True &nbsp; b) False &nbsp; c) False (10 IS in P)
3. `{x | x is a multiple of 5, 5 ≤ x ≤ 25}`
4. a) 5 &nbsp; b) 0 &nbsp; c) 100
5. Yes. `Y = {5, 1, 3}` after removing the duplicate 1. Both sets contain exactly {1, 3, 5}.

