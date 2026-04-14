## Day 3: Fractions & Decimals — Rational Numbers

---

### Quick recap

Before we move forward, let's make sure Days 1 and 2 are locked in:

- **Natural Numbers (ℕ)** = { 1, 2, 3, 4, ... } — counting numbers starting at 1
- **Whole Numbers (𝕎)** = { 0, 1, 2, 3, ... } — natural numbers plus zero
- **Integers (ℤ)** = { ..., −2, −1, 0, 1, 2, ... } — whole numbers plus all the negatives
- **ℕ ⊂ 𝕎 ⊂ ℤ** — each set contains the previous one
- Our number line now goes in **both directions** from zero

Yesterday I left you with a question:

> *What kind of number lives between 0 and 1?*

Today we answer that. And the answer opens up an entirely new world of numbers.

---

### The gap problem

Look at our number line right now:

```
←──┬────┬────┬────┬────┬────┬────┬────┬──→
  −3   −2   −1    0    1    2    3    4
```

Between every pair of integers, there is a **gap**. A big, empty gap. And real life constantly forces us into those gaps.

Think about these situations:

- You eat **half** a pizza. How much did you eat? Not 0 pizzas. Not 1 pizza. Something in between.
- A race is won by a margin of **0.3 seconds**. That's not 0 seconds and not 1 second.
- You score **7 out of 10** on a test. That's a ratio — 7 divided by 10.

None of these can be expressed as integers. We need a new type of number — one that can live in the gaps.

---

### Meet the Rational Numbers

A **Rational Number** is any number that can be written as a fraction — that is, one integer divided by another integer, as long as the bottom number is not zero.

We write this definition formally as:

$$\mathbb{Q} = \left\{ \frac{p}{q} \mid p, q \in \mathbb{Z},\ q \neq 0 \right\}$$

Let's read that in plain English:

> ℚ is the set of all numbers that can be written as p divided by q, where p and q are both integers, and q is not zero.

The symbol **ℚ** stands for **Quotient** — because a fraction is the result of dividing (the mathematical word for division result is quotient).

### Why can't q be zero?

Because division by zero is undefined. Try it on your calculator — you'll get an error. Dividing by zero doesn't produce a number at all, so we must exclude it.

---

### Examples of rational numbers

Here are some rational numbers and why they qualify:

| Number | Written as p/q | p | q |
|--------|----------------|---|---|
| 1/2 | 1/2 | 1 | 2 |
| −3/4 | −3/4 | −3 | 4 |
| 5 | 5/1 | 5 | 1 |
| −7 | −7/1 | −7 | 1 |
| 0 | 0/1 | 0 | 1 |
| 0.25 | 1/4 | 1 | 4 |
| 0.333... | 1/3 | 1 | 3 |

Notice something very important in that table. The numbers 5, −7, and 0 are all in there. That means **every integer is also a rational number** — because any integer n can be written as n/1.

This extends our nesting doll chain:

$$\mathbb{N} \subset \mathbb{W} \subset \mathbb{Z} \subset \mathbb{Q}$$

---

### Fractions and decimals are the same thing

A fraction and a decimal are just **two different ways of writing the same number**. One is not more "mathematical" than the other — they are equal.

To convert a fraction to a decimal, you simply divide the top number by the bottom number:

$$\frac{1}{4} = 1 \div 4 = 0.25$$

$$\frac{1}{3} = 1 \div 3 = 0.333\ldots$$

$$\frac{3}{8} = 3 \div 8 = 0.375$$

$$\frac{7}{2} = 7 \div 2 = 3.5$$

Try these on your own before moving on:

- What is 1/5 as a decimal?
- What is 2/3 as a decimal?
- What is 5/4 as a decimal?

---

### Answers

| Fraction | Division | Decimal |
|----------|----------|---------|
| 1/5 | 1 ÷ 5 | **0.2** |
| 2/3 | 2 ÷ 3 | **0.666...** |
| 5/4 | 5 ÷ 4 | **1.25** |

---

### Two types of rational decimals

Here is something really important. When you convert a rational number to a decimal, one of exactly two things will happen:

### Type 1 — Terminating decimals

The decimal **stops**. It ends at a finite number of digits.

$$\frac{1}{4} = 0.25 \quad \text{(stops after 2 decimal places)}$$

$$\frac{3}{8} = 0.375 \quad \text{(stops after 3 decimal places)}$$

$$\frac{7}{2} = 3.5 \quad \text{(stops after 1 decimal place)}$$

These are called **terminating decimals**. The division finishes cleanly with no remainder.

### Type 2 — Repeating decimals

The decimal **never stops**, but a pattern of digits repeats forever.

$$\frac{1}{3} = 0.333\ldots$$

$$\frac{2}{3} = 0.666\ldots$$

$$\frac{1}{7} = 0.142857142857\ldots$$

$$\frac{5}{11} = 0.454545\ldots$$

These are called **repeating decimals**. We sometimes write them with a bar over the repeating part:

$$\frac{1}{3} = 0.\overline{3} \qquad \frac{5}{11} = 0.\overline{45}$$

> **Key fact:** Every rational number is either a terminating decimal or a repeating decimal. No exceptions. If you divide any integer by any non-zero integer, you will always get one of these two types.

---

### Why every integer is rational?

This is a point worth pausing on, because students sometimes find it surprising.

Take the integer **3**. Is it rational?

Yes — because you can write it as:

$$3 = \frac{3}{1}$$

That is p = 3 and q = 1. Both are integers, and q ≠ 0. So 3 is rational.

Take the integer **−8**. Is it rational?

$$-8 = \frac{-8}{1}$$

Yes. Rational.

Take **0**. Is it rational?

$$0 = \frac{0}{1}$$

Yes. Rational.

This is why ℤ ⊂ ℚ — every integer fits perfectly inside the rational numbers.

---

### Rational numbers are dense

Here is something beautiful about rational numbers that integers don't have.

Between any two integers, there are only finitely many integers. Between 2 and 5, for example, there are exactly two integers: 3 and 4.

But between any two rational numbers, there are **infinitely many** rational numbers. This property is called **density**.

Let's say I give you 1/2 and 3/4. Can you find a rational number between them?

Yes — take the average:

$$\frac{\frac{1}{2} + \frac{3}{4}}{2} = \frac{\frac{5}{4}}{2} = \frac{5}{8}$$

Now can you find one between 1/2 and 5/8? Yes. Between that result and 5/8? Yes. You can always go deeper. The rational numbers pack infinitely tightly between any two points.

This is why we say the rational numbers are **dense on the number line**.

---

### Placing rational numbers on the number line

Let's practice placing some rational numbers on the number line.

```
←──┬─────┬──┬──┬─────┬──┬──┬─────┬──→
  −1   −1/2  0  1/4  1/2  3/4   1
```

A few tips for placing fractions:

- **1/2** sits exactly halfway between 0 and 1
- **1/4** sits one quarter of the way between 0 and 1
- **3/4** sits three quarters of the way between 0 and 1
- **−1/2** sits exactly halfway between −1 and 0

The key skill is knowing **which two integers your fraction lives between**, then figuring out exactly where in that gap it falls.

For example, where does **7/3** go?

$$\frac{7}{3} = 2.333\ldots$$

So it lives between 2 and 3, closer to 2.

---

### The "between" challenge

Here is one of the best exercises for understanding rational numbers:

> Find 3 rational numbers between 1/2 and 3/4.

Method: convert to decimals first.

$$\frac{1}{2} = 0.5 \qquad \frac{3}{4} = 0.75$$

Now find any three decimals between 0.5 and 0.75:

- 0.6 = 3/5 ✅
- 0.7 = 7/10 ✅
- 0.625 = 5/8 ✅

All three are rational (they can be written as fractions), and all three sit between 1/2 and 3/4. There are infinitely many more — we just picked three.

---

### Summary of what we learned

| Concept | Definition / Rule |
|---|---|
| Rational Numbers (ℚ) | Any number expressible as p/q where p, q ∈ ℤ and q ≠ 0 |
| Terminating decimal | A decimal that ends: 0.25, 0.375, 3.5 |
| Repeating decimal | A decimal with a forever-repeating pattern: 0.333..., 0.4545... |
| Every integer is rational | Because n = n/1 for any integer n |
| Density | Between any two rationals, there are infinitely many more rationals |
| Subset chain | ℕ ⊂ 𝕎 ⊂ ℤ ⊂ ℚ |

---

### Common mistakes — don't fall for these!

**Mistake 1:** "0.333... is not a fraction because it never ends."
→ Wrong. 0.333... = 1/3 exactly. Repeating decimals are perfectly valid rational numbers.

**Mistake 2:** "Integers are not rational numbers."
→ Wrong. Every integer n can be written as n/1, so every integer is rational. ℤ ⊂ ℚ.

**Mistake 3:** "The bottom of a fraction can be zero."
→ Never. Division by zero is undefined. q = 0 is strictly forbidden in the definition of ℚ.

**Mistake 4:** "A longer decimal is more accurate."
→ 0.333... and 1/3 are not approximations of each other — they are the **exact same number**, just written differently.

---

### Try yourself

Try these before checking the answers:

1. Write 0.6 as a fraction in its simplest form.
2. Is −5/3 a rational number? Why?
3. Convert 5/8 to a decimal. Is it terminating or repeating?
4. Find one rational number between 1/3 and 1/2.
5. Is every rational number also an integer? Is every integer also a rational number?

---

### Answers

| # | Question | Answer |
|---|----------|--------|
| 1 | 0.6 as a fraction | **3/5** |
| 2 | Is −5/3 rational? | **Yes** — p = −5, q = 3, both integers, q ≠ 0 |
| 3 | 5/8 as a decimal | **0.625** — terminating |
| 4 | Between 1/3 and 1/2 | Many valid answers, e.g. **5/12**, or **0.4** = 2/5 |
| 5 | Rational vs integer? | ❌ Not every rational is an integer (e.g. 1/2). ✅ Every integer IS rational. |

---

### Homework

Convert these 5 fractions to decimals. For each one, state whether it is **terminating** or **repeating**:

1. 3/4
2. 1/6
3. 7/8
4. 2/9
5. 11/4

Then write **one sentence** answering this question: *What makes a number rational?*

---

### Something to think about...

We said that every rational number is either a terminating decimal or a repeating decimal. Terminating means it stops. Repeating means a pattern goes on forever.

But what if a decimal goes on forever... and has **no repeating pattern at all**? What if the digits just go on and on, completely randomly, never settling into a cycle?

Could such a number exist? And if it does — is it rational?

> *Hint: think about the number π = 3.14159265358979...*

