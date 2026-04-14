## Day 6: Deep Dive — Properties & Real-World Connections

---

### Quick recap from Days 1 through 5

We have now built the complete Real Number system from the ground up:

$$\mathbb{N} \subset \mathbb{W} \subset \mathbb{Z} \subset \mathbb{Q} \subset \mathbb{R}$$

| Set | Symbol | Key feature |
|-----|--------|-------------|
| Natural Numbers | ℕ | Counting numbers: 1, 2, 3, ... |
| Whole Numbers | 𝕎 | Added zero |
| Integers | ℤ | Added negatives |
| Rational Numbers | ℚ | Added fractions and repeating/terminating decimals |
| Irrational Numbers | — | Non-terminating, non-repeating decimals |
| Real Numbers | ℝ | Everything above combined — every point on the number line |

Today we go deeper. We are not adding any new sets — instead, we are going to understand **how real numbers behave**. What rules govern them? Why do they work the way they do? And where do they actually show up in the real world?

This is the day where mathematics stops feeling like abstract symbols and starts feeling like a language that describes reality.

---

### The properties of real numbers

Every operation you have ever performed on numbers — adding, multiplying, rearranging — follows specific rules. These rules are called **properties**, and they hold true for all real numbers without exception.

There are six core properties. Let's go through each one carefully.

---

### Property 1 — Closure

**What it means:** When you perform an operation on two real numbers, the result is always also a real number. The answer never "escapes" the set.

**For addition:**

$$a + b \in \mathbb{R} \quad \text{for all } a, b \in \mathbb{R}$$

Example: 3 + π = some real number. You will never add two real numbers and get something that is not real.

**For multiplication:**

$$a \times b \in \mathbb{R} \quad \text{for all } a, b \in \mathbb{R}$$

Example: √2 × √3 = √6, which is still a real number.

> **Interesting edge case:** ℕ is closed under addition (3 + 5 = 8, still natural) but NOT under subtraction (3 − 5 = −2, not natural). This is exactly why we had to expand to ℤ on Day 2. Each time we expanded our number system, it was to restore closure under a new operation.

---

### Property 2 — Commutativity

**What it means:** The order in which you add or multiply two numbers does not matter. You get the same answer either way.

**For addition:**

$$a + b = b + a$$

Example: 4 + 7 = 7 + 4 = 11

**For multiplication:**

$$a \times b = b \times a$$

Example: 3 × 5 = 5 × 3 = 15

> **Warning — subtraction and division are NOT commutative:**
>
> $$8 - 3 \neq 3 - 8 \quad \text{because} \quad 5 \neq -5$$
>
> $$12 \div 4 \neq 4 \div 12 \quad \text{because} \quad 3 \neq \frac{1}{3}$$
>
> Commutativity only applies to addition and multiplication.

---

### Property 3 — Associativity

**What it means:** When adding or multiplying three or more numbers, the way you group them does not matter. You can move the brackets and get the same answer.

**For addition:**

$$(a + b) + c = a + (b + c)$$

Example: (2 + 3) + 4 = 5 + 4 = **9** and 2 + (3 + 4) = 2 + 7 = **9** ✅

**For multiplication:**

$$(a \times b) \times c = a \times (b \times c)$$

Example: (2 × 3) × 4 = 6 × 4 = **24** and 2 × (3 × 4) = 2 × 12 = **24** ✅

> **Warning — subtraction and division are NOT associative:**
>
> $$(8 - 3) - 2 = 5 - 2 = 3$$
> $$8 - (3 - 2) = 8 - 1 = 7$$
>
> The brackets matter for subtraction and division. Only addition and multiplication are associative.

---

### Property 4 — Distributivity

**What it means:** Multiplication distributes over addition and subtraction. You can either add first then multiply, or multiply each term separately then add — you get the same result.

$$a \times (b + c) = (a \times b) + (a \times c)$$

Example:

$$3 \times (4 + 5) = 3 \times 9 = 27$$

$$3 \times 4 + 3 \times 5 = 12 + 15 = 27 \quad \checkmark$$

This property is the foundation of algebra. Every time you expand brackets in an equation, you are using distributivity.

**It also works with subtraction:**

$$a \times (b - c) = (a \times b) - (a \times c)$$

Example:

$$5 \times (10 - 3) = 5 \times 7 = 35$$

$$5 \times 10 - 5 \times 3 = 50 - 15 = 35 \quad \checkmark$$

---

### Property 5 — Identity elements

**What it means:** There is a special number for addition and a special number for multiplication that leave any number unchanged when you use them.

**Additive identity — zero:**

$$a + 0 = a \quad \text{for all } a \in \mathbb{R}$$

Adding zero to any number does nothing. Zero is the identity for addition.

Example: 7 + 0 = 7, −π + 0 = −π, √2 + 0 = √2

**Multiplicative identity — one:**

$$a \times 1 = a \quad \text{for all } a \in \mathbb{R}$$

Multiplying any number by 1 does nothing. One is the identity for multiplication.

Example: 7 × 1 = 7, −π × 1 = −π, √2 × 1 = √2

> Notice how important zero and one are. This is part of why we worked so hard on Day 1 and 2 to include them in our number system — they are not just numbers, they are the **anchor points** of arithmetic.

---

### Property 6 — Inverse elements

**What it means:** For every real number, there is another real number that "undoes" it — bringing you back to the identity element.

**Additive inverse — the negative:**

$$a + (-a) = 0 \quad \text{for all } a \in \mathbb{R}$$

Every number has an opposite. Add them together and you get zero.

Example: 5 + (−5) = 0, π + (−π) = 0, √3 + (−√3) = 0

**Multiplicative inverse — the reciprocal:**

$$a \times \frac{1}{a} = 1 \quad \text{for all } a \in \mathbb{R},\ a \neq 0$$

Every non-zero number has a reciprocal. Multiply them together and you get one.

Example: 4 × 1/4 = 1, π × 1/π = 1, √2 × 1/√2 = 1

> Why does zero have no multiplicative inverse? Because 1/0 is undefined — you cannot divide by zero. Zero is the only real number without a multiplicative inverse. This is a deep and important exception.

---

### All six properties at a glance

| Property | Addition | Multiplication |
|----------|----------|----------------|
| Closure | a + b ∈ ℝ | a × b ∈ ℝ |
| Commutativity | a + b = b + a | a × b = b × a |
| Associativity | (a+b)+c = a+(b+c) | (a×b)×c = a×(b×c) |
| Distributivity | a×(b+c) = a×b + a×c | (same property) |
| Identity | a + 0 = a | a × 1 = a |
| Inverse | a + (−a) = 0 | a × (1/a) = 1, a ≠ 0 |

---

### The density property

We touched on this briefly on Day 3, but now we can state it fully.

**The density property of ℝ:**

> Between any two distinct real numbers, there is always another real number.

This is true for rationals, and it is also true for the full set of real numbers.

Let's experience it. Start with 0.1 and 0.2. Can we find a number between them?

- 0.15 ✅

Can we find one between 0.1 and 0.15?

- 0.125 ✅

Between 0.1 and 0.125?

- 0.1125 ✅

No matter how many times we do this, we can always go deeper. There is no "next" real number. There is no real number so close to another that nothing fits between them.

This is fundamentally different from integers. Between 3 and 4 there is no integer. But between any two real numbers — no matter how close — there are infinitely many real numbers.

---

### The completeness property

This is the property that truly sets ℝ apart from ℚ.

**The completeness of ℝ:**

> The real number line has no holes or gaps. Every point on the line corresponds to exactly one real number.

The rational numbers ℚ, despite being dense, are actually full of holes. The point √2 exists on the number line — a ruler would land exactly on it — but √2 is not in ℚ. So the rational number line has a hole at every irrational location.

The real numbers fill every single one of those holes. ℝ is complete — there is no point on the number line that is missing a number.

Think of it this way:

- ℚ is like a net — tightly woven, covering most of the line, but with infinitely many tiny gaps
- ℝ is like a solid wall — every point covered, no gaps at all

This completeness is what makes ℝ the right foundation for calculus, physics, and all of higher mathematics.

---

### Real numbers in the real world

Let's connect everything we have learned to the world around us. Every measurement, every quantity, every piece of data you will ever encounter in science, finance, or daily life is a real number.

### Measurement

Every physical measurement is a real number:

- Distance: the length of a table might be 1.37 metres — a rational number
- Time: a race might be won in 9.58 seconds — rational
- Temperature: −17.3°C — rational
- Circumference of a circle with diameter 1 metre: exactly π metres — irrational

### Science and engineering

- The charge of an electron, the speed of light, gravitational constants — all real numbers
- Electrical engineers use √2 constantly: the peak voltage of a 240V power supply is 240√2 ≈ 339.4 volts
- Architects and designers use φ (the golden ratio ≈ 1.618) for proportions

### Finance

- Interest rates, prices, exchange rates — all rational numbers (written as decimals to 2 or more places)
- Compound interest over time involves powers that often produce irrational results

### Which type of number fits which situation?

| Real-world situation | Type of number | Why |
|---------------------|----------------|-----|
| Number of students in a class | ℕ | You count whole people |
| Temperature in winter | ℤ or ℚ | Can be negative or fractional |
| A test score like 7/10 | ℚ | It is a ratio |
| Diagonal of a 1×1 square | Irrational | = √2 |
| Circumference of any circle | Irrational (contains π) | π is irrational |
| Your bank balance | ℚ | Dollars and cents — always terminating |
| Probability of an event | ℚ | Always between 0 and 1, expressible as fraction |

---

### A sense of size — how big are these sets?

Here is something to stretch your thinking. We have five nested sets. How do they compare in size?

- ℕ is **infinite** — there are infinitely many natural numbers
- 𝕎 is also infinite — but only one member larger than ℕ
- ℤ is also infinite — same "size" of infinity as ℕ (mathematicians can prove this)
- ℚ is also infinite — and remarkably, the same "size" of infinity as ℤ and ℕ
- The irrationals are **a bigger kind of infinite** — there are vastly more irrationals than rationals
- ℝ is the same size as the irrationals — a fundamentally larger infinity than ℚ

You do not need to prove any of this. But hold onto the idea: not all infinities are the same size. The real numbers represent a richer, denser infinity than the rationals alone.

---

### Summary of what we learned

| Concept | Key point |
|---------|-----------|
| Closure | Operations on real numbers always produce real numbers |
| Commutativity | a + b = b + a and a × b = b × a (not for − or ÷) |
| Associativity | (a+b)+c = a+(b+c) and (a×b)×c = a×(b×c) (not for − or ÷) |
| Distributivity | a×(b+c) = a×b + a×c — the foundation of algebra |
| Identity | 0 for addition, 1 for multiplication |
| Inverse | −a for addition, 1/a for multiplication (a ≠ 0) |
| Density | Between any two reals, there is always another real |
| Completeness | ℝ has no gaps — every point on the line is a real number |
| Real world | Every physical measurement is a real number |

---

### Common mistakes — don't fall for these!

**Mistake 1:** "Subtraction is commutative because addition is."
→ No. a − b ≠ b − a in general. 10 − 3 = 7 but 3 − 10 = −7. Only addition and multiplication are commutative.

**Mistake 2:** "The additive inverse of −7 is 7, but negative numbers don't have inverses."
→ Every real number has an additive inverse. The inverse of −7 is +7 because −7 + 7 = 0. The inverse of a negative is a positive, and vice versa.

**Mistake 3:** "Zero has a multiplicative inverse — it's just zero itself."
→ No. 0 × 0 = 0, not 1. Zero has no multiplicative inverse. Division by zero is undefined.

**Mistake 4:** "The density property means there is a 'next' real number after any given one."
→ The opposite is true. Density means there is NO next real number — you can always find another one in between.

**Mistake 5:** "ℝ and ℚ are the same size because both are infinite."
→ Not all infinities are equal. ℝ is a provably larger infinity than ℚ. The irrationals make it so.

---

### Try yourself

Try these before checking the answers:

1. Which property justifies: 3 × (2 + 7) = 3 × 2 + 3 × 7?
2. What is the additive inverse of −√5?
3. What is the multiplicative inverse of 2/3?
4. Is ℕ closed under subtraction? Give an example to support your answer.
5. Find a real number between 0.999 and 1.
6. Which property states that (5 + 3) + 8 = 5 + (3 + 8)?
7. Why does zero have no multiplicative inverse?
8. Name one real-world measurement that would definitely be irrational.

---

### Answers

| # | Question | Answer |
|---|----------|--------|
| 1 | 3×(2+7) = 3×2 + 3×7 | **Distributive property** |
| 2 | Additive inverse of −√5 | **√5** (because −√5 + √5 = 0) |
| 3 | Multiplicative inverse of 2/3 | **3/2** (because 2/3 × 3/2 = 1) |
| 4 | Is ℕ closed under subtraction? | **No** — e.g. 3 − 5 = −2, which is not in ℕ |
| 5 | Between 0.999 and 1 | Many valid answers, e.g. **0.9995** or **0.9999** |
| 6 | (5+3)+8 = 5+(3+8) | **Associative property of addition** |
| 7 | Why no multiplicative inverse for 0? | Because 1/0 is **undefined** — division by zero has no answer |
| 8 | Irrational real-world measurement | **Circumference of any circle** (contains π), or **diagonal of a unit square** (= √2) |

---

### Homework

Write a **one-page summary** in your own words describing each number type from Days 1 through 5. Include:

- The name and symbol of each set
- Three examples of numbers in that set
- One real-world situation where that type of number appears

Then answer this reflection question:

> *Which of the six properties do you use most often in everyday arithmetic without realising it? Give a specific example from your own life.*

Bring any remaining questions to class tomorrow — Day 7 is our final review and assessment day, and it is your last chance to clear up anything before we close the week.

---

### Something to think about...

We have now covered the entire Real Number system — its structure, its properties, and its connection to the world. Tomorrow is Day 7: review, consolidation, and your final assessment.

But here is one last thought to carry into tomorrow.

Every number system we built this week started with a question that the previous system could not answer:

- ℕ couldn't handle zero → we built 𝕎
- 𝕎 couldn't handle negatives → we built ℤ
- ℤ couldn't handle fractions → we built ℚ
- ℚ couldn't handle √2 or π → we built ℝ

So the natural question is: what can ℝ not handle?

We saw it on Day 5 — try √−1 on your calculator and it says ERROR. Real numbers cannot answer that question.

The mathematicians who came after did exactly what we did all week — they asked the question, refused to accept "impossible" as an answer, and built a new number system to handle it. They called it the **Complex Numbers**, and it uses a brand new kind of number called **i**, where:

$$i = \sqrt{-1}$$

That is a story for another course. But you now know exactly how it will begin — with a gap, a question, and the courage to build something new.

