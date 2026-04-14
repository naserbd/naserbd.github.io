## Day 4: The Breakthrough — Irrational Numbers

---

### Quick recap from yesterday

Let's make sure Days 1 through 3 are solid before we go further:

- **Natural Numbers (ℕ)** = { 1, 2, 3, ... } — counting numbers
- **Whole Numbers (𝕎)** = { 0, 1, 2, 3, ... } — added zero
- **Integers (ℤ)** = { ..., −2, −1, 0, 1, 2, ... } — added the negatives
- **Rational Numbers (ℚ)** = any number expressible as p/q where p, q ∈ ℤ and q ≠ 0
- **ℕ ⊂ 𝕎 ⊂ ℤ ⊂ ℚ** — each set contains the previous one
- Every rational number is either a **terminating** or **repeating** decimal

Yesterday I left you with this question:

> *What if a decimal goes on forever with no repeating pattern at all? Is it rational?*

Today we answer that. And the answer will genuinely surprise you.

---

### Let's start with a simple question

I want you to grab a calculator. Type this:

$$\sqrt{4}$$

You get **2**. Clean. Simple. 2 is a rational number — it equals 2/1.

Now type this:

$$\sqrt{9}$$

You get **3**. Also clean. Also rational.

Now type this:

$$\sqrt{2}$$

You get something like:

$$1.41421356237309504880168872\ldots$$

Keep staring at those digits. Does a pattern repeat? Is there a cycle of numbers coming back around?

No. There isn't. The digits go on forever and **never repeat**. Not ever.

This is not a rounding issue. This is not a calculator limitation. This is a fundamental property of the number itself. And it means that **√2 cannot be written as a fraction**. It is not rational.

We call it an **Irrational Number**.

---

### What exactly is an irrational number?

An irrational number is any real number that **cannot** be expressed as p/q where p and q are integers and q ≠ 0.

In decimal form, irrational numbers have two defining characteristics:

1. The decimal goes on **forever** — it never terminates
2. The decimal has **no repeating pattern** — ever

This is the exact opposite of rational numbers. Recall:

| Type | Decimal behaviour | Example |
|------|-------------------|---------|
| Rational | Terminates OR repeats forever | 0.25, 0.333... |
| Irrational | Goes on forever, never repeats | 1.41421356... |

There is no overlap. A number is either one or the other — never both.

---

### The most famous irrational numbers

These numbers are so important they each have their own symbol:

### √2 — the first discovered irrational

$$\sqrt{2} = 1.41421356237309504880168872420969807856967187537694\ldots$$

This was the number that broke ancient Greek mathematics. The Pythagoreans — a group of mathematicians around 500 BC — believed that every number in existence could be written as a fraction. When one of them proved that √2 could not, it was considered so shocking that, according to legend, the person who proved it was thrown into the sea.

### π (pi) — the circle constant

$$\pi = 3.14159265358979323846264338327950288419716939937510\ldots$$

π is the ratio of a circle's circumference to its diameter. Every circle in the universe, no matter how big or small, has this exact ratio. And yet it cannot be written as a fraction. 22/7 is a common approximation but it is not equal to π — it is just close.

### e — Euler's number

$$e = 2.71828182845904523536028747135266249775724709369995\ldots$$

e is the base of natural logarithms and appears constantly in science, finance, and engineering. It is irrational — its digits go on forever without repeating.

### √3, √5, √7 — and most square roots

$$\sqrt{3} = 1.73205080757\ldots$$
$$\sqrt{5} = 2.23606797749\ldots$$
$$\sqrt{7} = 2.64575131106\ldots$$

In fact, the square root of any whole number that is not a perfect square is irrational. The perfect squares are 1, 4, 9, 16, 25, 36... — their square roots are the integers 1, 2, 3, 4, 5, 6... Everything else is irrational.

### φ (phi) — the golden ratio

$$\varphi = \frac{1 + \sqrt{5}}{2} = 1.61803398874989484820458683436563811772030917980576\ldots$$

The golden ratio appears in art, architecture, nature, and biology. It is irrational.

---

### Proof that √2 is irrational

This is one of the most beautiful proofs in all of mathematics. It uses a technique called **proof by contradiction** — we assume the opposite of what we want to prove, then show that assumption leads to a logical impossibility.

We want to prove: **√2 cannot be written as a fraction.**

**Step 1 — Assume the opposite.**

Suppose √2 *is* rational. Then we can write:

$$\sqrt{2} = \frac{p}{q}$$

where p and q are integers with no common factors (the fraction is fully reduced).

**Step 2 — Square both sides.**

$$2 = \frac{p^2}{q^2}$$

$$p^2 = 2q^2$$

This tells us p² is even (because it equals 2 times something).

**Step 3 — If p² is even, then p must be even.**

This is because if p were odd, p² would also be odd. Since p² is even, p must be even.

So we can write p = 2k for some integer k.

**Step 4 — Substitute back.**

$$(2k)^2 = 2q^2$$

$$4k^2 = 2q^2$$

$$q^2 = 2k^2$$

This tells us q² is even — which means q must also be even.

**Step 5 — The contradiction.**

We now have: p is even AND q is even.

But we said at the start that p and q have **no common factors**. Two even numbers always share the factor 2. This is a contradiction.

**Conclusion:**

Our original assumption — that √2 is rational — must be false. Therefore √2 is irrational. ∎

> You do not need to memorise every step of this proof. But you should understand the *idea*: we assumed it was a fraction, followed the logic, and arrived at an impossible situation. That impossibility proves the assumption was wrong.

---

### Irrational numbers on the number line

Even though irrational numbers cannot be written as fractions, they absolutely exist on the number line. They have precise locations — we just cannot express those locations as p/q.

For example, √2 sits between 1 and 2 on the number line:

```
←──┬─────────┬────┬─────────┬──→
   1       √2≈1.414         2
             ↑
         between 1 and 2,
         closer to 1
```

And π sits between 3 and 4:

```
←──┬──────────────┬──────┬──→
   3           π≈3.14159  4
                  ↑
              between 3 and 4,
              very close to 3
```

These points exist. They are real. A ruler placed on a number line would land exactly on them. They simply cannot be captured by any fraction, no matter how precise.

---

### How many irrational numbers are there?

Here is something that will bend your mind a little.

We said rational numbers are **dense** — between any two rationals, there are infinitely many more rationals. You might think that would fill up the entire number line completely.

But it turns out the irrational numbers are actually **far more numerous** than the rational numbers. Mathematicians have proven that if you picked a random point on the number line, the probability of landing on a rational number is essentially zero. Almost every point on the number line is irrational.

The rational numbers are like scattered islands. The irrational numbers are the vast ocean between them.

> You do not need to prove this — just hold onto the idea. It becomes important on Day 5 when we build the complete Real Number system.

---

### Rational vs irrational — how to tell

Given a number, how do you decide if it is rational or irrational?

**It IS rational if:**

- It is an integer (e.g. −7, 0, 4)
- It is a fraction of integers (e.g. 3/5, −2/9)
- Its decimal terminates (e.g. 0.6, 1.375)
- Its decimal repeats (e.g. 0.333..., 0.142857142857...)

**It IS irrational if:**

- It is the square root of a non-perfect-square (e.g. √2, √3, √5, √7)
- It is π, e, or φ
- Its decimal goes on forever with no repeating pattern

**Tricky cases to watch out for:**

| Number | Rational or Irrational? | Why |
|--------|------------------------|-----|
| √9 | **Rational** | √9 = 3 = 3/1 |
| √2 | **Irrational** | Non-perfect-square root |
| 0.101001000100001... | **Irrational** | Non-terminating, non-repeating |
| 0.101010101... | **Rational** | Repeating pattern (10 repeats) |
| 22/7 | **Rational** | It is a fraction |
| π | **Irrational** | Cannot be written as any fraction |
| −√16 | **Rational** | −√16 = −4 = −4/1 |
| √2 × √2 | **Rational** | √2 × √2 = 2 = 2/1 |

---

### Summary of what we learned

| Concept | Definition / Rule |
|---|---|
| Irrational number | Cannot be written as p/q; decimal is non-terminating and non-repeating |
| √2 | The first proven irrational number; ≈ 1.41421356... |
| π | Ratio of circumference to diameter; ≈ 3.14159265... |
| e | Euler's number; ≈ 2.71828182... |
| Proof by contradiction | Assume the opposite, reach an impossibility, conclude the opposite is false |
| Irrational on number line | They exist at precise points — just not expressible as fractions |
| Subset chain so far | ℕ ⊂ 𝕎 ⊂ ℤ ⊂ ℚ, and irrationals sit *outside* ℚ |

---

### Common mistakes — don't fall for these!

**Mistake 1:** "22/7 = π"
→ 22/7 ≈ 3.142857142857... — this is a rational number that is *close to* π. They are not equal. π is irrational; 22/7 is rational.

**Mistake 2:** "Irrational means impossible or wrong."
→ Irrational simply means *not a ratio*. Irrational numbers are perfectly real and valid. They have exact locations on the number line.

**Mistake 3:** "√4 is irrational because square roots are always irrational."
→ Wrong. √4 = 2, which is a perfectly rational integer. Only square roots of non-perfect squares are irrational.

**Mistake 4:** "0.101001000100001... looks like it repeats."
→ Look carefully — the number of zeros increases each time (1 zero, then 2, then 3, then 4...). The pattern of *growth* is regular, but the decimal itself never repeats the same block. It is irrational.

**Mistake 5:** "π = 3.14"
→ 3.14 is a terminating decimal and therefore rational. It is an approximation of π, not π itself.

---

### Try yourself

Try these before checking the answers:

1. Is √25 rational or irrational?
2. Is √11 rational or irrational?
3. Write down two digits of π after the decimal point from memory.
4. What are the two properties that make a decimal irrational?
5. Is 0.727272... rational or irrational?
6. A student says "π ≈ 22/7 so π is rational." What is wrong with this statement?

---

### Answers

| # | Question | Answer |
|---|----------|--------|
| 1 | √25 rational or irrational? | **Rational** — √25 = 5 |
| 2 | √11 rational or irrational? | **Irrational** — 11 is not a perfect square |
| 3 | Two digits of π after decimal | **3.14**... (3, 1, 4, 1, 5, 9, ...) |
| 4 | Two properties of irrational decimal | **Non-terminating** AND **non-repeating** |
| 5 | 0.727272... rational or irrational? | **Rational** — 0.72 repeats forever = 72/99 = 8/11 |
| 6 | π ≈ 22/7 so π is rational? | **Wrong** — an approximation is not equality. 22/7 ≠ π. π is irrational. |

---

### Homework

Use a calculator to find the decimal expansion of these square roots. For each one, decide: **rational or irrational?** Write one sentence justifying your answer.

1. √16
2. √5
3. √49
4. √8
5. √100

**Bonus:** Look up one more famous irrational number that we didn't mention in today's lesson. Write its symbol, its approximate decimal value, and where it appears in real life.

---

### Something to think about...

Today we met two separate groups of numbers — the rationals and the irrationals. They sit side by side on the number line, interleaved with each other, filling every possible point.

What if we put them both together? What do we get?

> *Is there a name for the set of ALL numbers on the number line — both rational and irrational combined?*

