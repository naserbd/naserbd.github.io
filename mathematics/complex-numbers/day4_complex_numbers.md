## Day 4 — Conjugates & Dividing Complex Numbers

---

### *"The cleverest trick in complex number arithmetic"*

---

### Learning Objectives

By the end of Day 4, you will be able to:

- Define the **complex conjugate** of any complex number
- State and use the key properties of conjugates
- Divide a complex number by a **real number**
- Divide a complex number by another **complex number**
- Use the conjugate method to **rationalise** the denominator
- Write every division result in **standard form** (a + bi)

---

### Part 1 — Revisiting Yesterday's Key Discovery

On Day 3, you discovered a remarkable special product:

$$(a + bi)(a - bi) = a^2 + b^2$$

Look at what makes this so special:
- The result is **always a real number**
- The result is **always positive** (since a² ≥ 0 and b² ≥ 0)
- The imaginary part has **completely vanished**

This is not a coincidence. The two numbers (a + bi) and (a − bi) are a special pair called **complex conjugates**, and their product being real is precisely what makes division possible.

Today, everything flows from this one idea.

---

### Part 2 — The Complex Conjugate

### Definition

The **complex conjugate** of a complex number z = a + bi is:

$$\boxed{\bar{z} = a - bi}$$

Read as **"z bar"**. To find the conjugate, you **flip the sign of the imaginary part only**. The real part stays exactly the same.

---

### Examples of Conjugates

| Complex Number z | Conjugate z̄ | What changed? |
|-----------------|-------------|---------------|
| 3 + 4i | 3 − 4i | +4i became −4i |
| 7 − 2i | 7 + 2i | −2i became +2i |
| −5 + 6i | −5 − 6i | +6i became −6i |
| −1 − 3i | −1 + 3i | −3i became +3i |
| 4 + 0i = 4 | 4 − 0i = 4 | Real numbers are their own conjugate! |
| 0 + 5i = 5i | 0 − 5i = −5i | Purely imaginary: just negate |

> ⚠️ **Common Mistake:** The conjugate of (3 − 4i) is (3 + 4i) — **not** (−3 + 4i). Only the sign of the imaginary part changes. The real part is **never** touched.

---

### Part 3 — Properties of the Conjugate

These properties are essential — learn them well.

### Property 1 — The Product of Conjugates

$$\boxed{z \cdot \bar{z} = a^2 + b^2}$$

This is always a **real, non-negative** number. It equals the square of the distance from the origin on the Argand diagram (you'll explore this on Day 5).

**Example:** $z = 3 + 4i$, $\bar{z} = 3 - 4i$

$$z \cdot \bar{z} = (3+4i)(3-4i) = 3^2 + 4^2 = 9 + 16 = 25$$

---

### Property 2 — The Sum of Conjugates

$$\boxed{z + \bar{z} = 2a}$$

Adding a complex number to its conjugate always gives **twice the real part** — a real number.

**Example:** $z = 5 + 3i$, $\bar{z} = 5 - 3i$

$$z + \bar{z} = (5 + 3i) + (5 - 3i) = 10 + 0i = 10 = 2(5)$$

---

### Property 3 — The Difference of Conjugates

$$\boxed{z - \bar{z} = 2bi}$$

Subtracting a conjugate from the original gives **twice the imaginary part** — a purely imaginary number.

**Example:** $z = 5 + 3i$, $\bar{z} = 5 - 3i$

$$z - \bar{z} = (5 + 3i) - (5 - 3i) = 0 + 6i = 6i = 2(3i)$$

---

### Property 4 — The Conjugate of a Conjugate

$$\boxed{\overline{(\bar{z})} = z}$$

Taking the conjugate twice returns you to the original number. Conjugation is its own inverse.

---

### Property 5 — Conjugate of a Sum and Product

$$\boxed{\overline{z_1 + z_2} = \bar{z_1} + \bar{z_2}}$$

$$\boxed{\overline{z_1 \cdot z_2} = \bar{z_1} \cdot \bar{z_2}}$$

The conjugate distributes over both addition and multiplication.

---

### Part 4 — Dividing by a Real Number

This is the easy case. When dividing a complex number by a **real number** k, simply divide both parts by k separately.

### The Rule

$$\boxed{\frac{a + bi}{k} = \frac{a}{k} + \frac{b}{k}i}$$

### Worked Example 1

$$\frac{6 + 10i}{2}$$

**Divide each part by 2:**

$$= \frac{6}{2} + \frac{10}{2}i = 3 + 5i$$

**Answer: 3 + 5i** ✓

---

### Worked Example 2

$$\frac{5 - 3i}{4}$$

**Divide each part by 4:**

$$= \frac{5}{4} - \frac{3}{4}i$$

**Answer:** $\dfrac{5}{4} - \dfrac{3}{4}i$ ✓

> 💡 Fractions in the answer are perfectly fine and correct — do not try to eliminate them unless told to.

---

### Part 5 — Dividing by a Complex Number

This is the heart of today's lesson. Dividing by a complex number requires a technique called **multiplying by the conjugate**.

### Why Can't We Just Divide Directly?

Consider:

$$\frac{1 + 2i}{3 + i}$$

If we tried to separate this fraction directly, we'd be left with an imaginary number in the denominator — which is **not** standard form. Standard form requires the denominator to be a real number.

### The Solution — Multiply by the Conjugate

To remove the complex number from the denominator, multiply **both numerator and denominator** by the conjugate of the denominator.

This is exactly like **rationalising the denominator** with surds:

$$\frac{1}{\sqrt{3}} = \frac{1}{\sqrt{3}} \times \frac{\sqrt{3}}{\sqrt{3}} = \frac{\sqrt{3}}{3}$$

With complex numbers:

$$\frac{a + bi}{c + di} = \frac{a + bi}{c + di} \times \frac{c - di}{c - di}$$

Since $\dfrac{c - di}{c - di} = 1$, we haven't changed the value — only the form.

### The Complete Method

$$\boxed{\frac{a + bi}{c + di} = \frac{(a + bi)(c - di)}{(c + di)(c - di)} = \frac{(a + bi)(c - di)}{c^2 + d^2}}$$

**Step-by-step:**
1. Write the division as a fraction
2. Identify the conjugate of the denominator
3. Multiply top AND bottom by the conjugate
4. Expand the numerator using FOIL
5. Simplify the denominator using $c^2 + d^2$ (no working needed!)
6. Separate into real and imaginary parts
7. Write in standard form a + bi

---

### Worked Example 3 — Full Step-by-Step Division

$$\text{Calculate } \frac{1 + 2i}{3 + i}$$

**Step 1:** Identify conjugate of denominator: conjugate of (3 + i) is **(3 − i)**

**Step 2:** Multiply top and bottom by (3 − i):

$$= \frac{(1 + 2i)(3 - i)}{(3 + i)(3 - i)}$$

**Step 3:** Expand the numerator using FOIL:

$$(1 + 2i)(3 - i) = 3 - i + 6i - 2i^2$$
$$= 3 + 5i - 2(-1)$$
$$= 3 + 5i + 2$$
$$= 5 + 5i$$

**Step 4:** Simplify the denominator:

$$(3 + i)(3 - i) = 3^2 + 1^2 = 9 + 1 = 10$$

**Step 5:** Combine:

$$= \frac{5 + 5i}{10}$$

**Step 6:** Divide each part by 10:

$$= \frac{5}{10} + \frac{5}{10}i = \frac{1}{2} + \frac{1}{2}i$$

**Answer:** $\dfrac{1}{2} + \dfrac{1}{2}i$ ✓

---

### Worked Example 4 — Division with Negative Parts

$$\text{Calculate } \frac{3 - 2i}{1 + 4i}$$

**Step 1:** Conjugate of denominator: **(1 − 4i)**

**Step 2:** Multiply:

$$= \frac{(3 - 2i)(1 - 4i)}{(1 + 4i)(1 - 4i)}$$

**Step 3:** Expand numerator:

$$(3 - 2i)(1 - 4i) = 3 - 12i - 2i + 8i^2$$
$$= 3 - 14i + 8(-1)$$
$$= 3 - 14i - 8$$
$$= -5 - 14i$$

**Step 4:** Simplify denominator:

$$(1 + 4i)(1 - 4i) = 1^2 + 4^2 = 1 + 16 = 17$$

**Step 5:** Combine and separate:

$$= \frac{-5 - 14i}{17} = -\frac{5}{17} - \frac{14}{17}i$$

**Answer:** $-\dfrac{5}{17} - \dfrac{14}{17}i$ ✓

---

### Worked Example 5 — Purely Imaginary Denominator

$$\text{Calculate } \frac{4 + 2i}{3i}$$

**Method A — Conjugate method:**

Conjugate of 3i = (0 + 3i) is (0 − 3i) = −3i

$$= \frac{(4 + 2i)(-3i)}{(3i)(-3i)} = \frac{-12i - 6i^2}{-9i^2} = \frac{-12i + 6}{9} = \frac{6}{9} - \frac{12}{9}i = \frac{2}{3} - \frac{4}{3}i$$

**Method B — Multiply numerator and denominator by i:**

$$= \frac{(4 + 2i) \times i}{3i \times i} = \frac{4i + 2i^2}{3i^2} = \frac{4i - 2}{-3} = \frac{-2 + 4i}{-3} = \frac{2}{3} - \frac{4}{3}i$$

Both methods give the same answer.

**Answer:** $\dfrac{2}{3} - \dfrac{4}{3}i$ ✓

---

### Worked Example 6 — Finding the Real and Imaginary Parts of a Quotient

$$\text{Find Re}\left(\frac{2+i}{1-i}\right) \text{ and } \text{Im}\left(\frac{2+i}{1-i}\right)$$

**Conjugate of denominator:** (1 + i)

$$\frac{(2+i)(1+i)}{(1-i)(1+i)} = \frac{2 + 2i + i + i^2}{1^2 + 1^2} = \frac{2 + 3i - 1}{2} = \frac{1 + 3i}{2} = \frac{1}{2} + \frac{3}{2}i$$

$$\text{Re} = \frac{1}{2}, \qquad \text{Im} = \frac{3}{2}$$

---

### Part 6 — The Analogy: Rationalising the Denominator

You have already used a very similar technique with **surds**:

$$\frac{5}{2 + \sqrt{3}} = \frac{5(2 - \sqrt{3})}{(2 + \sqrt{3})(2 - \sqrt{3})} = \frac{5(2 - \sqrt{3})}{4 - 3} = 5(2 - \sqrt{3})$$

The technique is **identical** in structure:

| Surds | Complex Numbers |
|-------|----------------|
| Denominator: $2 + \sqrt{3}$ | Denominator: $3 + 4i$ |
| Multiply by: $2 - \sqrt{3}$ | Multiply by: $3 - 4i$ |
| Result: $(2)^2 - (\sqrt{3})^2 = 1$ | Result: $3^2 + 4^2 = 25$ |
| Denominator becomes real | Denominator becomes real |

In both cases, the strategy is to **use a partner that eliminates the awkward part** — the surd or the imaginary number. With complex numbers, that partner is always the conjugate.

---

### Part 7 — The Division Formula

If you prefer a direct formula (though FOIL + conjugate is recommended for clarity):

$$\boxed{\frac{a + bi}{c + di} = \frac{ac + bd}{c^2 + d^2} + \frac{bc - ad}{c^2 + d^2}i}$$

**Verify with Example 3:** $\dfrac{1 + 2i}{3 + i}$ where a=1, b=2, c=3, d=1

$$\text{Real: } \frac{(1)(3) + (2)(1)}{3^2 + 1^2} = \frac{3 + 2}{10} = \frac{5}{10} = \frac{1}{2}$$

$$\text{Imaginary: } \frac{(2)(3) - (1)(1)}{3^2 + 1^2} = \frac{6 - 1}{10} = \frac{5}{10} = \frac{1}{2}$$

$$\text{Answer: } \frac{1}{2} + \frac{1}{2}i \checkmark$$

---

### Part 8 — Key Rules to Memorise

$$\boxed{\bar{z} = a - bi} \qquad \text{(flip the sign of the imaginary part only)}$$

$$\boxed{z \cdot \bar{z} = a^2 + b^2} \qquad \text{(always a real, non-negative number)}$$

$$\boxed{\frac{a + bi}{k} = \frac{a}{k} + \frac{b}{k}i} \qquad \text{(divide each part by the real number)}$$

$$\boxed{\frac{a + bi}{c + di} = \frac{(a + bi)(c - di)}{c^2 + d^2}} \qquad \text{(multiply by conjugate of denominator)}$$

$$\text{The denominator always simplifies to } c^2 + d^2 \text{ — a real number. No FOIL needed for denominator.}$$

---

### Part 9 — Common Mistakes to Avoid

| Mistake | Wrong | Correct |
|---------|-------|---------|
| Conjugating the wrong number | Conjugate of (3+4i) is (−3+4i) | Conjugate is **(3 − 4i)** |
| Only multiplying the numerator | $\frac{1+2i}{3+i} \times (3-i)$ | Must multiply **both** top and bottom |
| Using wrong sign in denominator formula | $c^2 - d^2$ | Denominator is always $c^2 + d^2$ |
| Forgetting i² = −1 in numerator FOIL | Leaving 2i² in answer | Replace: $2i^2 = -2$ |
| Not simplifying fully | $\frac{6 + 10i}{4}$ left as is | Simplify to $\frac{3}{2} + \frac{5}{2}i$ |
| Changing the real part in conjugate | Conjugate of (5+3i) is (−5−3i) | Conjugate is **(5 − 3i)** |

---

### Practice Problems

Try these yourself before checking answers!

**Level 1 — Basic**

1. Write the conjugate of each: (a) $2 + 7i$ (b) $-4 - i$ (c) $3$ (d) $-6i$
2. Calculate $z \cdot \bar{z}$ for $z = 3 + 5i$
3. $\dfrac{8 + 12i}{4}$
4. $\dfrac{6 - 9i}{3}$

**Level 2 — Intermediate**

5. $\dfrac{1}{2 + i}$
6. $\dfrac{3 + i}{1 - i}$
7. $\dfrac{2 + 3i}{4 - i}$
8. $\dfrac{5}{3i}$

**Level 3 — Challenge**

9. $\dfrac{(1 + i)^2}{1 - i}$ — Hint: expand the numerator first using Day 3 skills
10. $\dfrac{3 + 4i}{3 - 4i}$ — What do you notice about the modulus of this result?
11. If $z = \dfrac{1 + 2i}{3 - i}$, find $z + \bar{z}$ and $z \cdot \bar{z}$
12. Show that $\dfrac{z}{\bar{z}}$ always has modulus 1 for any non-zero complex number z (Hint: use $|z|^2 = z \cdot \bar{z}$ and the property $\overline{z_1 z_2} = \bar{z_1}\bar{z_2}$)

---

### Answers

**Level 1**

1. (a) $2 - 7i$ (b) $-4 + i$ (c) $3$ (d) $6i$
2. $z \cdot \bar{z} = 3^2 + 5^2 = 9 + 25 =$ **34**
3. $\dfrac{8}{4} + \dfrac{12}{4}i =$ **2 + 3i**
4. $\dfrac{6}{3} - \dfrac{9}{3}i =$ **2 − 3i**

**Level 2**

5. $\dfrac{1}{2+i} \times \dfrac{2-i}{2-i} = \dfrac{2-i}{4+1} = \dfrac{2-i}{5} =$ **$\dfrac{2}{5} - \dfrac{1}{5}i$**

6. $\dfrac{(3+i)(1+i)}{(1-i)(1+i)} = \dfrac{3+3i+i+i^2}{1+1} = \dfrac{3+4i-1}{2} = \dfrac{2+4i}{2} =$ **1 + 2i**

7. $\dfrac{(2+3i)(4+i)}{(4-i)(4+i)} = \dfrac{8+2i+12i+3i^2}{16+1} = \dfrac{8+14i-3}{17} = \dfrac{5+14i}{17} =$ **$\dfrac{5}{17} + \dfrac{14}{17}i$**

8. $\dfrac{5}{3i} \times \dfrac{-3i}{-3i} = \dfrac{-15i}{9} =$ **$-\dfrac{5}{3}i$** (or equivalently $0 - \dfrac{5}{3}i$)

**Level 3**

9. $(1+i)^2 = 1 + 2i + i^2 = 2i$; then $\dfrac{2i}{1-i} \times \dfrac{1+i}{1+i} = \dfrac{2i+2i^2}{1+1} = \dfrac{-2+2i}{2} =$ **−1 + i**

10. $\dfrac{(3+4i)(3+4i)}{(3-4i)(3+4i)} = \dfrac{9+24i+16i^2}{25} = \dfrac{9+24i-16}{25} = \dfrac{-7+24i}{25} = -\dfrac{7}{25}+\dfrac{24}{25}i$; Modulus $= \sqrt{\left(\dfrac{7}{25}\right)^2+\left(\dfrac{24}{25}\right)^2} = \sqrt{\dfrac{49+576}{625}} = \sqrt{\dfrac{625}{625}} = $ **1** — the modulus is always 1 when dividing conjugate pairs of equal modulus!

11. First find z: $\dfrac{(1+2i)(3+i)}{(3-i)(3+i)} = \dfrac{3+i+6i+2i^2}{9+1} = \dfrac{3+7i-2}{10} = \dfrac{1+7i}{10} = \dfrac{1}{10}+\dfrac{7}{10}i$; so $\bar{z} = \dfrac{1}{10}-\dfrac{7}{10}i$; $z+\bar{z} = \dfrac{2}{10} =$ **$\dfrac{1}{5}$**; $z \cdot \bar{z} = \left(\dfrac{1}{10}\right)^2+\left(\dfrac{7}{10}\right)^2 = \dfrac{1+49}{100} =$ **$\dfrac{1}{2}$**

12. $\left|\dfrac{z}{\bar{z}}\right| = \dfrac{|z|}{|\bar{z}|}$; since $|\bar{z}| = \sqrt{a^2+(-b)^2} = \sqrt{a^2+b^2} = |z|$, we get $\dfrac{|z|}{|z|} = $ **1** ✓ — dividing z by its conjugate always produces a number on the unit circle.

---

### Day 4 Summary

| Concept | Key Takeaway |
|---------|-------------|
| Conjugate definition | $\bar{z} = a - bi$ — flip sign of imaginary part only |
| Conjugate product | $z\bar{z} = a^2 + b^2$ — always real and non-negative |
| Conjugate sum | $z + \bar{z} = 2a$ — always real |
| Divide by real | Split into $\frac{a}{k} + \frac{b}{k}i$ |
| Divide by complex | Multiply top and bottom by conjugate of denominator |
| Denominator result | Always simplifies to $c^2 + d^2$ — real, no FOIL needed |
| Core strategy | Same as rationalising the denominator with surds |
| Goal | Get denominator real → write result in standard form |

