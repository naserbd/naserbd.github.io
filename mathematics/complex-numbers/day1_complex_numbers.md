## Day 1 — What Are Complex Numbers?

---

### *"The day mathematics refused to say 'impossible'"*

---

### Learning Objectives

By the end of Day 1, you will be able to:

- Explain **why** complex numbers were invented
- Understand what the imaginary unit **i** means
- Identify the **real** and **imaginary** parts of a complex number
- Write complex numbers in **standard form**
- Perform basic **checks** using the definition of i

---

### Part 1 — The Problem That Started It All

### The Equation Nobody Could Solve

Long ago, mathematicians could solve many equations. For example:

$$x^2 - 9 = 0 \quad \Rightarrow \quad x = 3 \text{ or } x = -3$$

Simple. But then came this innocent-looking equation:

$$x^2 + 1 = 0$$

Let's try to solve it step by step:

$$x^2 = -1$$

$$x = \sqrt{-1} \quad \text{???}$$

**The problem:** No real number, when squared, gives a negative result.

- Positive × Positive = **Positive** ✓
- Negative × Negative = **Positive** ✓
- Zero × Zero = **Zero** ✓
- **There is no real number where x² = −1** ✗

For centuries, mathematicians simply wrote *"no solution"* and moved on. Until they didn't.

---

### Part 2 — The Invention of i

### The Bold Decision

Around the 16th–17th century, mathematicians made a **revolutionary decision**:

> *"What if we simply* **define** *a new number that solves this?"*

They defined a brand new number called the **imaginary unit**, written as **i**, with this single rule:

$$\boxed{i^2 = -1}$$

Or equivalently:

$$i = \sqrt{-1}$$

This is the **entire foundation** of complex numbers. Everything else builds from this one definition.

---

### Powers of i — A Repeating Cycle

Once you define i, its powers create a beautiful cycle of just 4 values:

| Power | Working | Result |
|-------|---------|--------|
| i¹ | i | **i** |
| i² | i × i | **−1** |
| i³ | i² × i = −1 × i | **−i** |
| i⁴ | i² × i² = −1 × −1 | **1** |
| i⁵ | i⁴ × i = 1 × i | **i** (cycle restarts!) |

> **The cycle:** i → −1 → −i → 1 → i → −1 → −i → 1 → ...
>
> **Trick:** To find any power of i, divide the exponent by 4 and look at the remainder.
> - Remainder 0 → **1**
> - Remainder 1 → **i**
> - Remainder 2 → **−1**
> - Remainder 3 → **−i**

**Example:** What is i²³?
- 23 ÷ 4 = 5 remainder **3**
- Remainder 3 → answer is **−i** ✓

---

### Part 3 — The Standard Form of a Complex Number

### Building a Complex Number

Now that we have i, we can build complex numbers by combining a real number with an imaginary number:

$$\boxed{z = a + bi}$$

Where:
- **z** is the name we give to the complex number
- **a** is the **real part** — an ordinary real number
- **b** is the **imaginary part** — the coefficient in front of i
- **i** is the imaginary unit (i² = −1)

---

### Identifying Real and Imaginary Parts

| Complex Number z | Real Part Re(z) | Imaginary Part Im(z) |
|-----------------|-----------------|----------------------|
| 3 + 4i | 3 | 4 |
| 7 − 2i | 7 | −2 |
| −5 + i | −5 | 1 |
| 6 | 6 | 0 |
| −3i | 0 | −3 |
| 0 | 0 | 0 |

> **Common Mistake:** The imaginary part of 3 + 4i is **4**, not 4i. It is just the *coefficient* of i — a plain real number.

---

### Special Cases — The Number Line Inside the Plane

Complex numbers are a **superset** of all the numbers you already know:

- If **b = 0**: z = a + 0i = **a** → just a regular real number (e.g., 5, −3, π)
- If **a = 0**: z = 0 + bi = **bi** → a **purely imaginary** number (e.g., 2i, −7i)
- If **a = 0 and b = 0**: z = 0 → the number **zero**

So every real number IS a complex number — just with imaginary part = 0. Complex numbers contain all real numbers within them.

---

### Part 4 — The Analogy: A New Dimension

### Why "Imaginary" Is a Misleading Name

The word *"imaginary"* was meant as an insult — critics thought these numbers were made-up nonsense. The name stuck, but these numbers are absolutely real in their usefulness.

**The 2D Map Analogy:**

Think of numbers like directions on a map:

- **Real numbers** only move you **East ↔ West** along a line
- **Imaginary numbers** add the ability to move **North ↕ South**
- **Complex numbers** give you **full 2D movement** on a plane

| Movement | Number Type | Example |
|----------|-------------|---------|
| East only | Positive real | +5 |
| West only | Negative real | −3 |
| North only | Positive imaginary | +4i |
| South only | Negative imaginary | −2i |
| Any direction | Complex | 3 + 4i |

> The number **3 + 4i** means: *"Go 3 units East and 4 units North."*
> This 2D plane of complex numbers is called the **Argand diagram** — you'll explore it fully on Day 5!

---

### Part 5 — Worked Examples

### Example 1 — Simplifying square roots of negatives

$$\sqrt{-9} = \sqrt{9 \times -1} = \sqrt{9} \times \sqrt{-1} = 3i$$

$$\sqrt{-25} = \sqrt{25} \times \sqrt{-1} = 5i$$

$$\sqrt{-7} = \sqrt{7} \times \sqrt{-1} = \sqrt{7} \cdot i$$

---

### Example 2 — Writing in standard form

**Write 4i + 3 in standard form:**
- Standard form is a + bi
- Answer: **3 + 4i** (real part first)

**Write −2 − √(−16) in standard form:**
- √(−16) = 4i
- Answer: **−2 − 4i**

---

### Example 3 — Are these complex numbers?

| Number | Is it complex? | Why? |
|--------|---------------|------|
| 7 | ✅ Yes | z = 7 + 0i |
| −3i | ✅ Yes | z = 0 + (−3)i |
| √2 | ✅ Yes | z = √2 + 0i |
| π | ✅ Yes | z = π + 0i |
| 2 + 3i | ✅ Yes | Already in standard form |

Every number you've ever used is a complex number. Complex numbers are the **complete number system**.

---

### Part 6 — Key Rules to Memorise

$$i^2 = -1 \qquad \text{(the master rule — everything follows from this)}$$

$$z = a + bi \qquad \text{(standard form)}$$

$$\text{Re}(z) = a \qquad \text{(real part)}$$

$$\text{Im}(z) = b \qquad \text{(imaginary part — just the coefficient, not "bi")}$$

$$\sqrt{-n} = \sqrt{n} \cdot i \qquad \text{for any } n > 0$$

---

### Practice Problems

Try these yourself before checking answers:

**Level 1 — Basic**
1. Write the real and imaginary parts of: z = 8 − 3i
2. Simplify: √(−36)
3. What is i⁶?
4. Is 5 a complex number? Explain.

**Level 2 — Intermediate**

5. Write in standard form: −√(−4) + 7
6. What is i¹⁰⁰?
7. Find a and b if z = (3−b) + (2a)i = 1 + 6i

**Level 3 — Challenge**

8. Show that (i²)² = 1. Does this mean i² = 1? Why or why not?
9. Simplify: i + i² + i³ + i⁴
10. If z = 0 + 0i, is z real, purely imaginary, or both?

---

### Answers

1. Re(z) = 8, Im(z) = −3
2. √(−36) = 6i
3. i⁶ → 6 ÷ 4 = remainder 2 → **−1**
4. Yes — it equals 5 + 0i
5. −2i + 7 = **7 − 2i**
6. i¹⁰⁰ → 100 ÷ 4 = remainder 0 → **1**
7. 3 − b = 1 → b = 2; and 2a = 6 → a = 3
8. (i²)² = (−1)² = 1 ✓. But i² = −1, not +1. Squaring i² gives +1 because (−1)² = 1 — no contradiction.
9. i + (−1) + (−i) + 1 = **0**
10. z = 0 is **both** — it's the only number that is simultaneously real (b = 0) and purely imaginary (a = 0)

---

### Day 1 Summary

| Concept | Key Takeaway |
|---------|-------------|
| Why i exists | To solve equations like x² = −1 |
| Definition | i² = −1 (this is all you need) |
| Standard form | z = a + bi |
| Real part | The 'a' — no i attached |
| Imaginary part | The 'b' — coefficient of i only |
| Powers of i | Cycle of 4: i, −1, −i, 1 |
| Big picture | Complex numbers contain ALL numbers |
