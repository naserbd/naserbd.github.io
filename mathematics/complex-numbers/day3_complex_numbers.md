## Day 3 — Multiplying Complex Numbers

---

### *"Where imaginary becomes real — the magic of i² = −1"*

---

### Learning Objectives

By the end of Day 3, you will be able to:

- Multiply a complex number by a **real number**
- Multiply a complex number by a **purely imaginary number**
- Multiply **two complex numbers** together using FOIL
- Apply the rule **i² = −1** to simplify results
- Write every answer in **standard form** (a + bi)
- Recognise the elegant formula for complex multiplication

---

### Part 1 — Why Multiplication Is Special

Addition and subtraction of complex numbers were straightforward — just combine like parts. Multiplication is where things get **genuinely interesting**.

The key ingredient that makes complex multiplication unique is the single rule you learned on Day 1:

$$\boxed{i^2 = -1}$$

When you multiply two complex numbers, you will always produce an **i²** term. That term then transforms from imaginary into **real** using this rule. An imaginary quantity literally becomes real — and that is what makes complex numbers so powerful.

---

### Part 2 — Multiplying by a Real Number

This is the simplest case. When multiplying a complex number by a real number **k**, simply distribute k to both parts.

### The Rule

$$\boxed{k(a + bi) = ka + kbi}$$

### Worked Example 1

$$3(2 + 5i)$$

**Distribute the 3:**
$$= 3 \times 2 + 3 \times 5i = 6 + 15i$$

**Answer: 6 + 15i** ✓

---

### Worked Example 2

$$-2(4 - 3i)$$

**Distribute the −2 carefully:**
$$= (-2)(4) + (-2)(-3i) = -8 + 6i$$

**Answer: −8 + 6i** ✓

> ⚠️ **Watch the signs:** −2 × −3i = +6i. A negative times a negative is positive — the same rule as always.

---

### Part 3 — Multiplying by a Purely Imaginary Number

When multiplying by a term like **ci** (a purely imaginary number), distribute as normal — then simplify any **i²** that appears.

### Worked Example 3

$$3i(2 + 4i)$$

**Step 1:** Distribute 3i:
$$= 3i \times 2 + 3i \times 4i$$
$$= 6i + 12i^2$$

**Step 2:** Replace i² with −1:
$$= 6i + 12(-1)$$
$$= 6i - 12$$

**Step 3:** Write in standard form (real part first):
$$= -12 + 6i$$

**Answer: −12 + 6i** ✓

> 💡 **Key moment:** The term 12i² looked imaginary — but after replacing i² = −1, it became the real number −12. This is the transformation that makes complex multiplication so elegant.

---

### Part 4 — Multiplying Two Complex Numbers (FOIL)

This is the main event. To multiply two complex numbers, treat them exactly like two **algebraic binomials** and expand using **FOIL**:

- **F**irst terms
- **O**uter terms
- **I**nner terms
- **L**ast terms

Then apply i² = −1 to simplify.

### The Formula

$$\boxed{(a + bi)(c + di) = (ac - bd) + (ad + bc)i}$$

You do **not** need to memorise this formula — if you can do FOIL, you can always derive it. But it is worth recognising.

---

### Worked Example 4 — Step by Step FOIL

$$\text{Calculate } (2 + 3i)(1 + 4i)$$

**Step 1 — FOIL expansion:**

| Term | Calculation | Result |
|------|-------------|--------|
| First: 2 × 1 | | 2 |
| Outer: 2 × 4i | | 8i |
| Inner: 3i × 1 | | 3i |
| Last: 3i × 4i | = 12i² | 12i² |

**Step 2 — Collect terms:**
$$= 2 + 8i + 3i + 12i^2$$

**Step 3 — Replace i² = −1:**
$$= 2 + 8i + 3i + 12(-1)$$
$$= 2 + 11i - 12$$

**Step 4 — Combine real parts:**
$$= (2 - 12) + 11i$$
$$= -10 + 11i$$

**Answer: −10 + 11i** ✓

---

### Worked Example 5 — Negative Imaginary Parts

$$\text{Calculate } (3 - 2i)(4 + i)$$

**Step 1 — FOIL:**
$$= (3)(4) + (3)(i) + (-2i)(4) + (-2i)(i)$$
$$= 12 + 3i - 8i - 2i^2$$

**Step 2 — Replace i² = −1:**
$$= 12 + 3i - 8i - 2(-1)$$
$$= 12 + 3i - 8i + 2$$

**Step 3 — Combine real and imaginary parts separately:**
$$= (12 + 2) + (3 - 8)i$$
$$= 14 - 5i$$

**Answer: 14 − 5i** ✓

---

### Worked Example 6 — Both Negative Imaginary Parts

$$\text{Calculate } (1 - 3i)(2 - 5i)$$

**Step 1 — FOIL:**
$$= (1)(2) + (1)(-5i) + (-3i)(2) + (-3i)(-5i)$$
$$= 2 - 5i - 6i + 15i^2$$

**Step 2 — Replace i² = −1:**
$$= 2 - 5i - 6i + 15(-1)$$
$$= 2 - 11i - 15$$

**Step 3 — Combine:**
$$= (2 - 15) + (-11)i$$
$$= -13 - 11i$$

**Answer: −13 − 11i** ✓

---

### Worked Example 7 — Using the Direct Formula

$$\text{Calculate } (5 + 2i)(3 - 4i)$$

Here a = 5, b = 2, c = 3, d = −4. Applying the formula (ac − bd) + (ad + bc)i:

$$\text{Real part: } ac - bd = (5)(3) - (2)(-4) = 15 + 8 = 23$$

$$\text{Imaginary part: } ad + bc = (5)(-4) + (2)(3) = -20 + 6 = -14$$

$$\text{Answer: } 23 - 14i \checkmark$$

> 💡 **Tip:** Always verify with FOIL if you use the formula, especially when signs are tricky.

---

### Part 5 — The Analogy: FOIL with a Twist

Think of multiplying complex numbers like multiplying two binomials in algebra — something you already know how to do:

$$(x + 3)(x + 4) = x^2 + 4x + 3x + 12 = x^2 + 7x + 12$$

Complex multiplication is **identical** — except when you reach the "Last" term, instead of getting something like 3 × 4 = 12, you get something like 3i × 4i = 12i². And that i² immediately becomes −1.

| Algebra | Complex Numbers |
|---------|----------------|
| (x + 3)(x + 4) | (2 + 3i)(1 + 4i) |
| x² + 4x + 3x + 12 | 2 + 8i + 3i + 12i² |
| = x² + 7x + 12 | = 2 + 11i + 12(−1) |
| No further simplification | = −10 + 11i |

The only new step is that **i² becomes −1** — everything else is standard algebra you already know.

---

### Part 6 — Special Products Worth Knowing

### Special Product 1 — Squaring a Complex Number

$$(a + bi)^2 = a^2 + 2abi + b^2i^2 = a^2 + 2abi - b^2 = (a^2 - b^2) + 2abi$$

**Example:** $(2 + 3i)^2$

$$= (2)^2 + 2(2)(3i) + (3i)^2$$
$$= 4 + 12i + 9i^2$$
$$= 4 + 12i - 9$$
$$= -5 + 12i$$

---

### Special Product 2 — A Complex Number Times Its Conjugate ⭐

This is the **most important** special product and sets up Day 4 perfectly.

The **conjugate** of (a + bi) is (a − bi). Watch what happens when you multiply them:

$$(a + bi)(a - bi)$$

**FOIL:**
$$= a^2 - abi + abi - b^2i^2$$
$$= a^2 - b^2i^2$$
$$= a^2 - b^2(-1)$$
$$= a^2 + b^2$$

$$\boxed{(a + bi)(a - bi) = a^2 + b^2}$$

> 🌟 **Remarkable result:** The two imaginary terms (+abi and −abi) cancel perfectly. The i² term becomes real. The final answer is **always a positive real number**. This extraordinary property is the foundation of complex division — coming up on Day 4!

**Example:** $(3 + 4i)(3 - 4i) = 3^2 + 4^2 = 9 + 16 = 25$

No complex working needed — just square and add!

---

### Special Product 3 — Multiplying Purely Imaginary Numbers

$$(bi)(di) = bdi^2 = bd(-1) = -bd$$

Two purely imaginary numbers multiply to give a **real number**.

**Example:** $(5i)(3i) = 15i^2 = 15(-1) = -15$

---

### Part 7 — Key Rules to Memorise

$$\boxed{i^2 = -1} \qquad \text{(apply this every single time you see } i^2 \text{)}$$

$$\boxed{k(a + bi) = ka + kbi} \qquad \text{(real number × complex number)}$$

$$\boxed{(a + bi)(c + di) = (ac - bd) + (ad + bc)i} \qquad \text{(complex × complex)}$$

$$\boxed{(a + bi)(a - bi) = a^2 + b^2} \qquad \text{(conjugate pair — always real!)}$$

$$\text{Method: FOIL} \rightarrow \text{collect terms} \rightarrow \text{replace } i^2 = -1 \rightarrow \text{standard form}$$

---

### Part 8 — Common Mistakes to Avoid

| Mistake | Wrong | Correct |
|---------|-------|---------|
| Forgetting to apply i² = −1 | (2+3i)(1+4i) = 2+11i+12i² | = **−10 + 11i** |
| Treating i² as +1 | 12i² = 12 | = **−12** |
| Only multiplying first terms | (3+2i)(4+i) = 12 + 2i² | Use full **FOIL** |
| Forgetting real part from i² | 2+3i−12 → answer is 3i−10 | Real parts: 2+(−12) = **−10** |
| Sign error on last FOIL term | (1−3i)(2−5i): last = −15i² | last = +15i² → = **−15** |

---

### Practice Problems

Try these yourself before checking answers!

**Level 1 — Basic**

1. $4(3 + 2i)$
2. $-3(1 - 5i)$
3. $2i(3 + i)$
4. $i(4 - 6i)$

**Level 2 — Intermediate**

5. $(1 + 2i)(3 + 4i)$
6. $(5 + i)(2 - 3i)$
7. $(3 - 4i)(3 + 4i)$
8. $(2 + i)^2$

**Level 3 — Challenge**

9. $(1 + i)^3$ — Hint: find $(1+i)^2$ first, then multiply by $(1+i)$ again
10. $(2 + 3i)(2 - 3i)(1 + i)$
11. Show that $(a + bi)^2 + (a - bi)^2 = 2(a^2 - b^2)$
12. If $z = 1 + 2i$, find $z^2 - 2z + 5$

---

### Answers

**Level 1**

1. $4 \times 3 + 4 \times 2i =$ **12 + 8i**
2. $(-3)(1) + (-3)(-5i) =$ **−3 + 15i**
3. $2i \times 3 + 2i \times i = 6i + 2i^2 = 6i - 2 =$ **−2 + 6i**
4. $i \times 4 + i \times (-6i) = 4i - 6i^2 = 4i + 6 =$ **6 + 4i**

**Level 2**

5. FOIL: $3 + 4i + 6i + 8i^2 = 3 + 10i - 8 =$ **−5 + 10i**
6. FOIL: $10 - 15i + 2i - 3i^2 = 10 - 13i + 3 =$ **13 − 13i**
7. Conjugate pair: $3^2 + 4^2 = 9 + 16 =$ **25** (purely real!)
8. $(2+i)^2 = 4 + 4i + i^2 = 4 + 4i - 1 =$ **3 + 4i**

**Level 3**

9. $(1+i)^2 = 1 + 2i + i^2 = 1 + 2i - 1 = 2i$; then $2i(1+i) = 2i + 2i^2 = 2i - 2 =$ **−2 + 2i**
10. First: $(2+3i)(2-3i) = 4 + 9 = 13$; then $13(1+i) =$ **13 + 13i**
11. $(a+bi)^2 = a^2 - b^2 + 2abi$; $(a-bi)^2 = a^2 - b^2 - 2abi$; Sum $= 2(a^2 - b^2)$ ✓ (imaginary parts cancel)
12. $z^2 = (1+2i)^2 = 1 + 4i + 4i^2 = 1 + 4i - 4 = -3 + 4i$; $-2z = -2 - 4i$; Sum: $(-3+4i) + (-2-4i) + 5 = 0$ — the answer is **0**! This means z = 1+2i is a **root** of z² − 2z + 5 = 0.

---

### Day 3 Summary

| Concept | Key Takeaway |
|---------|-------------|
| Real × complex | Distribute to both parts: k(a+bi) = ka + kbi |
| Imaginary × complex | Distribute, then apply i² = −1 |
| Complex × complex | Use FOIL, then apply i² = −1 |
| The magic step | i² always becomes −1, turning imaginary into real |
| Conjugate product | (a+bi)(a−bi) = a² + b² — always a real number |
| Formula | (a+bi)(c+di) = (ac−bd) + (ad+bc)i |
| Method summary | FOIL → collect → replace i² = −1 → standard form |


