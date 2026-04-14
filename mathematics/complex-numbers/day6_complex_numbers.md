## Day 6 — Polar Form & Euler's Formula

---

### *"The most beautiful equation in mathematics — and why it makes everything easier"*

---

### Learning Objectives

By the end of Day 6, you will be able to:

- Write any complex number in **polar form** r(cosθ + i sinθ)
- Write any complex number in **exponential form** re^(iθ) using Euler's formula
- Convert fluently **between** Cartesian, polar, and exponential forms
- Multiply and divide complex numbers using **polar/exponential form**
- Understand why multiplication by a complex number causes **rotation and scaling**
- Appreciate **Euler's identity** — the most famous equation in all of mathematics

---

### Part 1 — Bringing Together Days 3 and 5

On Day 5 you learned that every complex number z = a + bi can be described by:
- Its **modulus** r = |z| — the distance from the origin
- Its **argument** θ = arg(z) — the angle from the positive real axis

You also discovered the conversion formulas:

$$a = r\cos\theta \qquad b = r\sin\theta$$

Substituting these into z = a + bi gives something remarkable:

$$z = r\cos\theta + ir\sin\theta$$

$$\boxed{z = r(\cos\theta + i\sin\theta)}$$

This is **polar form**. Every complex number has one. Today you will learn to use it — and meet the even more powerful exponential form hiding just behind it.

---

### Part 2 — Polar Form in Detail

### The Standard Notation

$$\boxed{z = r(\cos\theta + i\sin\theta)}$$

Where:
- **r = |z|** is the modulus — always $r \geq 0$
- **θ = arg(z)** is the principal argument — always $-\pi < \theta \leq \pi$
- The expression $(\cos\theta + i\sin\theta)$ is sometimes abbreviated **cis θ**

So polar form can also be written compactly as:

$$z = r \operatorname{cis}\theta$$

---

### Converting Cartesian → Polar Form

**Step-by-step:**
1. Calculate the modulus: $r = \sqrt{a^2 + b^2}$
2. Find the argument: $\theta = \arg(z)$ (using the quadrant method from Day 5)
3. Write: $z = r(\cos\theta + i\sin\theta)$

---

### Worked Example 1 — First Quadrant

$$\text{Write } z = 1 + i \text{ in polar form}$$

**Step 1 — Modulus:**
$$r = \sqrt{1^2 + 1^2} = \sqrt{2}$$

**Step 2 — Argument** (1st quadrant, a > 0, b > 0):
$$\theta = \arctan\!\left(\frac{1}{1}\right) = \frac{\pi}{4}$$

**Step 3 — Polar form:**
$$z = \sqrt{2}\!\left(\cos\frac{\pi}{4} + i\sin\frac{\pi}{4}\right)$$

**Answer:** $z = \sqrt{2}\operatorname{cis}\dfrac{\pi}{4}$ ✓

---

### Worked Example 2 — Second Quadrant

$$\text{Write } z = -\sqrt{3} + i \text{ in polar form}$$

**Step 1 — Modulus:**
$$r = \sqrt{(-\sqrt{3})^2 + 1^2} = \sqrt{3 + 1} = 2$$

**Step 2 — Argument** (2nd quadrant, a < 0, b > 0):
$$\alpha = \arctan\!\left(\frac{1}{\sqrt{3}}\right) = \frac{\pi}{6}$$
$$\theta = \pi - \frac{\pi}{6} = \frac{5\pi}{6}$$

**Step 3 — Polar form:**
$$z = 2\!\left(\cos\frac{5\pi}{6} + i\sin\frac{5\pi}{6}\right)$$

---

### Worked Example 3 — Third Quadrant

$$\text{Write } z = -1 - i \text{ in polar form}$$

**Step 1 — Modulus:**
$$r = \sqrt{1 + 1} = \sqrt{2}$$

**Step 2 — Argument** (3rd quadrant, a < 0, b < 0):
$$\alpha = \arctan\!\left(\frac{1}{1}\right) = \frac{\pi}{4}$$
$$\theta = \frac{\pi}{4} - \pi = -\frac{3\pi}{4}$$

**Step 3 — Polar form:**
$$z = \sqrt{2}\!\left(\cos\!\left(-\frac{3\pi}{4}\right) + i\sin\!\left(-\frac{3\pi}{4}\right)\right)$$

---

### Worked Example 4 — Fourth Quadrant

$$\text{Write } z = 2 - 2\sqrt{3}i \text{ in polar form}$$

**Step 1 — Modulus:**
$$r = \sqrt{4 + 12} = \sqrt{16} = 4$$

**Step 2 — Argument** (4th quadrant, a > 0, b < 0):
$$\alpha = \arctan\!\left(\frac{2\sqrt{3}}{2}\right) = \arctan(\sqrt{3}) = \frac{\pi}{3}$$
$$\theta = -\frac{\pi}{3}$$

**Step 3 — Polar form:**
$$z = 4\!\left(\cos\!\left(-\frac{\pi}{3}\right) + i\sin\!\left(-\frac{\pi}{3}\right)\right)$$

---

### Converting Polar → Cartesian Form

Simply evaluate the cosine and sine values:

$$a = r\cos\theta \qquad b = r\sin\theta \qquad \Rightarrow \qquad z = a + bi$$

**Example:** $z = 3\!\left(\cos\dfrac{\pi}{6} + i\sin\dfrac{\pi}{6}\right)$

$$a = 3\cos\frac{\pi}{6} = 3 \times \frac{\sqrt{3}}{2} = \frac{3\sqrt{3}}{2}$$

$$b = 3\sin\frac{\pi}{6} = 3 \times \frac{1}{2} = \frac{3}{2}$$

$$z = \frac{3\sqrt{3}}{2} + \frac{3}{2}i$$

---

### Part 3 — Euler's Formula

### The Most Important Formula in Complex Analysis

In the 18th century, the Swiss mathematician **Leonhard Euler** discovered a breathtaking connection between the exponential function and trigonometry:

$$\boxed{e^{i\theta} = \cos\theta + i\sin\theta}$$

This is **Euler's formula**. It tells us that the complex exponential $e^{i\theta}$ traces a perfect circle of radius 1 in the complex plane as θ varies.

At first glance this seems impossible — how can raising e to an imaginary power give trigonometric functions? The connection comes through **power series** (studied at A-level and university), where the series for $e^x$, $\cos x$, and $\sin x$ combine perfectly when x is replaced by iθ.

---

### Why Euler's Formula Makes Sense — The Power Series Approach

Recall the Taylor series expansions:

$$e^x = 1 + x + \frac{x^2}{2!} + \frac{x^3}{3!} + \frac{x^4}{4!} + \cdots$$

$$\cos\theta = 1 - \frac{\theta^2}{2!} + \frac{\theta^4}{4!} - \frac{\theta^6}{6!} + \cdots$$

$$\sin\theta = \theta - \frac{\theta^3}{3!} + \frac{\theta^5}{5!} - \frac{\theta^7}{7!} + \cdots$$

Substituting $x = i\theta$ into the exponential series:

$$e^{i\theta} = 1 + i\theta + \frac{(i\theta)^2}{2!} + \frac{(i\theta)^3}{3!} + \frac{(i\theta)^4}{4!} + \cdots$$

$$= 1 + i\theta - \frac{\theta^2}{2!} - \frac{i\theta^3}{3!} + \frac{\theta^4}{4!} + \frac{i\theta^5}{5!} - \cdots$$

$$= \underbrace{\left(1 - \frac{\theta^2}{2!} + \frac{\theta^4}{4!} - \cdots\right)}_{\cos\theta} + i\underbrace{\left(\theta - \frac{\theta^3}{3!} + \frac{\theta^5}{5!} - \cdots\right)}_{\sin\theta}$$

$$= \cos\theta + i\sin\theta \qquad \checkmark$$

The real and imaginary parts separate perfectly into cosine and sine!

---

### Exponential Form of a Complex Number

Using Euler's formula, polar form $r(\cos\theta + i\sin\theta)$ becomes:

$$\boxed{z = re^{i\theta}}$$

This is the **exponential form** (also called **Euler form**) of a complex number. It is the most compact and powerful way to write a complex number.

| Form | Expression | Best used for |
|------|-----------|---------------|
| Cartesian | $z = a + bi$ | Addition, subtraction |
| Polar | $z = r(\cos\theta + i\sin\theta)$ | Visualisation, rotation |
| Exponential | $z = re^{i\theta}$ | Multiplication, division, powers |

---

### Converting to Exponential Form

The method is identical to polar form — find r and θ, then write $re^{i\theta}$.

**Example:** Write $z = -2 + 2i$ in exponential form.

$$r = \sqrt{4+4} = 2\sqrt{2}, \qquad \theta = \pi - \frac{\pi}{4} = \frac{3\pi}{4}$$

$$z = 2\sqrt{2}\,e^{i\cdot\frac{3\pi}{4}}$$

---

### Part 4 — Euler's Identity

Setting $\theta = \pi$ in Euler's formula:

$$e^{i\pi} = \cos\pi + i\sin\pi = -1 + 0 = -1$$

Therefore:

$$\boxed{e^{i\pi} + 1 = 0}$$

This is **Euler's Identity** — consistently voted the most beautiful equation in mathematics. In a single line it unites:

| Symbol | What it represents |
|--------|--------------------|
| **e** | The base of natural logarithms — the heart of calculus |
| **i** | The imaginary unit — the foundation of complex numbers |
| **π** | The ratio of circumference to diameter — the soul of geometry |
| **1** | The multiplicative identity |
| **0** | The additive identity |

Five of the most fundamental constants in all of mathematics, connected by the simplest possible relationship.

> 💬 The physicist Richard Feynman called it *"the most remarkable formula in mathematics"*. The mathematician Carl Friedrich Gauss reportedly said that anyone to whom this formula is not immediately apparent has never been a first-rate mathematician.

---

### Part 5 — Multiplying in Polar/Exponential Form

This is where polar form reveals its true power. Multiplication in Cartesian form requires FOIL. In exponential form, it is a single line.

### Multiplication Rule

For $z_1 = r_1 e^{i\theta_1}$ and $z_2 = r_2 e^{i\theta_2}$:

$$\boxed{z_1 \cdot z_2 = r_1 r_2\, e^{i(\theta_1 + \theta_2)}}$$

In polar form:

$$\boxed{z_1 \cdot z_2 = r_1 r_2 \big(\cos(\theta_1+\theta_2) + i\sin(\theta_1+\theta_2)\big)}$$

**The rule in words:**
> To multiply two complex numbers — **multiply their moduli** and **add their arguments**.

This has a beautiful geometric meaning: multiplication **scales** by $r_1 r_2$ and **rotates** by $\theta_1 + \theta_2$.

---

### Worked Example 5 — Multiplication in Polar Form

Let $z_1 = 3\!\left(\cos\dfrac{\pi}{6} + i\sin\dfrac{\pi}{6}\right)$ and $z_2 = 2\!\left(\cos\dfrac{\pi}{3} + i\sin\dfrac{\pi}{3}\right)$

$$z_1 z_2 = (3 \times 2)\!\left(\cos\!\left(\frac{\pi}{6}+\frac{\pi}{3}\right) + i\sin\!\left(\frac{\pi}{6}+\frac{\pi}{3}\right)\right)$$

$$= 6\!\left(\cos\frac{\pi}{2} + i\sin\frac{\pi}{2}\right) = 6(0 + i) = 6i$$

**Answer: 6i** ✓

> ✨ Compare how quick this was versus expanding with FOIL in Cartesian form!

---

### Worked Example 6 — Multiplication in Exponential Form

$$z_1 = 4e^{i\pi/4}, \qquad z_2 = 3e^{i\pi/3}$$

$$z_1 z_2 = (4 \times 3)\,e^{i(\pi/4 + \pi/3)} = 12\,e^{i \cdot 7\pi/12}$$

**Answer:** $12e^{i\cdot 7\pi/12}$ ✓

---

### Part 6 — Dividing in Polar/Exponential Form

Division is equally elegant.

### Division Rule

$$\boxed{\frac{z_1}{z_2} = \frac{r_1}{r_2}\,e^{i(\theta_1 - \theta_2)}}$$

In polar form:

$$\boxed{\frac{z_1}{z_2} = \frac{r_1}{r_2}\big(\cos(\theta_1-\theta_2) + i\sin(\theta_1-\theta_2)\big)}$$

**The rule in words:**
> To divide two complex numbers — **divide their moduli** and **subtract their arguments**.

---

### Worked Example 7 — Division in Polar Form

$$\frac{z_1}{z_2} \text{ where } z_1 = 6\!\left(\cos\frac{3\pi}{4} + i\sin\frac{3\pi}{4}\right), \quad z_2 = 2\!\left(\cos\frac{\pi}{4} + i\sin\frac{\pi}{4}\right)$$

$$= \frac{6}{2}\!\left(\cos\!\left(\frac{3\pi}{4}-\frac{\pi}{4}\right) + i\sin\!\left(\frac{3\pi}{4}-\frac{\pi}{4}\right)\right)$$

$$= 3\!\left(\cos\frac{\pi}{2} + i\sin\frac{\pi}{2}\right) = 3(0 + i) = 3i$$

**Answer: 3i** ✓

---

### Part 7 — Geometric Meaning of Multiplication

This is one of the deepest insights in all of complex number theory.

### Multiplying by i — Rotation by 90°

Consider any complex number z. What happens when we multiply by i?

$$i = 1 \cdot e^{i\pi/2}$$

So multiplying by i means: modulus stays the same (×1), argument increases by $\dfrac{\pi}{2}$ (90°).

> **Multiplying by i rotates any complex number by exactly 90° anticlockwise.**

**Verification:**
- $1 \xrightarrow{\times i} i \xrightarrow{\times i} -1 \xrightarrow{\times i} -i \xrightarrow{\times i} 1$
- Arguments: $0 \to \frac{\pi}{2} \to \pi \to -\frac{\pi}{2} \to 0$ ✓ (each step +90°)

---

### Multiplying by −1 — Rotation by 180°

$$-1 = 1 \cdot e^{i\pi}$$

Multiplying by −1 rotates by 180° — this is why a negative times a negative is positive! Rotating 180° twice returns to the start.

---

### General Multiplication

$$z_1 = r_1 e^{i\theta_1} \quad \text{acts on} \quad z_2 = r_2 e^{i\theta_2}$$

The result $z_1 z_2 = r_1 r_2\,e^{i(\theta_1+\theta_2)}$ can be read as:

> $z_1$ **scales** $z_2$ by factor $r_1$ and **rotates** $z_2$ by angle $\theta_1$.

This geometric interpretation is the foundation of applications in physics, engineering and computer graphics.

---

### Part 8 — Key Trigonometric Values to Know

When working in polar form, these exact values come up constantly:

| θ (radians) | θ (degrees) | cos θ | sin θ |
|-------------|-------------|-------|-------|
| 0 | 0° | 1 | 0 |
| π/6 | 30° | $\frac{\sqrt{3}}{2}$ | $\frac{1}{2}$ |
| π/4 | 45° | $\frac{\sqrt{2}}{2}$ | $\frac{\sqrt{2}}{2}$ |
| π/3 | 60° | $\frac{1}{2}$ | $\frac{\sqrt{3}}{2}$ |
| π/2 | 90° | 0 | 1 |
| π | 180° | −1 | 0 |
| −π/2 | −90° | 0 | −1 |

> 💡 **Memory trick:** For sin, the sequence $0°\to90°$ gives $0, \frac{1}{2}, \frac{\sqrt{2}}{2}, \frac{\sqrt{3}}{2}, 1$ — think of $\frac{\sqrt{0}}{2}, \frac{\sqrt{1}}{2}, \frac{\sqrt{2}}{2}, \frac{\sqrt{3}}{2}, \frac{\sqrt{4}}{2}$. For cos, the sequence runs in **reverse**.

---

### Part 9 — Key Rules to Memorise

$$\boxed{e^{i\theta} = \cos\theta + i\sin\theta} \qquad \text{(Euler's formula — learn this absolutely)}$$

$$\boxed{z = r(\cos\theta + i\sin\theta) = re^{i\theta}} \qquad \text{(polar and exponential forms)}$$

$$\boxed{z_1 z_2 = r_1 r_2\,e^{i(\theta_1+\theta_2)}} \qquad \text{(multiply moduli, ADD arguments)}$$

$$\boxed{\frac{z_1}{z_2} = \frac{r_1}{r_2}\,e^{i(\theta_1-\theta_2)}} \qquad \text{(divide moduli, SUBTRACT arguments)}$$

$$\boxed{e^{i\pi} + 1 = 0} \qquad \text{(Euler's identity)}$$

$$\boxed{\times i \Rightarrow \text{rotate anticlockwise by } 90°} \qquad \text{(geometric meaning of } i\text{)}$$

---

### Part 10 — Common Mistakes to Avoid

| Mistake | Wrong | Correct |
|---------|-------|---------|
| Multiplying arguments instead of adding | $z_1 z_2$ has argument $\theta_1 \times \theta_2$ | Argument is $\theta_1 + \theta_2$ |
| Adding moduli instead of multiplying | $|z_1 z_2| = r_1 + r_2$ | $|z_1 z_2| = r_1 \times r_2$ |
| Wrong sign in division | $\arg(z_1/z_2) = \theta_1 + \theta_2$ | $= \theta_1 - \theta_2$ |
| Forgetting r in polar form | $z = \cos\theta + i\sin\theta$ | $z = r(\cos\theta + i\sin\theta)$ |
| Argument outside principal range | $\theta = \frac{5\pi}{4}$ left as is | Adjust to $\theta = -\frac{3\pi}{4}$ (subtract $2\pi$) |
| Evaluating $e^{i\theta}$ as a real number | $e^{i\pi} = e^\pi \approx 23.1$ | $e^{i\pi} = -1$ (Euler's formula!) |

---

### Practice Problems

Try these yourself before checking answers!

**Level 1 — Basic**

1. Write in polar form: (a) $z = 2i$ (b) $z = -4$ (c) $z = 1 + i$ (d) $z = \sqrt{3} - i$
2. Write in Cartesian form: (a) $2(\cos\frac{\pi}{2} + i\sin\frac{\pi}{2})$ (b) $4(\cos\pi + i\sin\pi)$ (c) $3(\cos\frac{\pi}{6} + i\sin\frac{\pi}{6})$
3. Write in exponential form: (a) $z = 1$ (b) $z = i$ (c) $z = -1 + i$

**Level 2 — Intermediate**

4. Given $z_1 = 2(\cos\frac{\pi}{4} + i\sin\frac{\pi}{4})$ and $z_2 = 3(\cos\frac{\pi}{4} + i\sin\frac{\pi}{4})$, find $z_1 z_2$ in Cartesian form.
5. Given $z_1 = 6e^{i\pi/3}$ and $z_2 = 2e^{i\pi/6}$, find $\frac{z_1}{z_2}$ in polar and Cartesian form.
6. If $z = \sqrt{2}e^{i\pi/4}$, write $z^2$ in Cartesian form.
7. Show that multiplying $z = 3 + 4i$ by $i$ rotates it 90° anticlockwise by computing iz and verifying the argument increases by $\frac{\pi}{2}$.

**Level 3 — Challenge**

8. Find all complex numbers z such that $|z| = 2$ and $\arg(z^2) = \frac{\pi}{2}$
9. If $z = re^{i\theta}$, show that $\bar{z} = re^{-i\theta}$ — what does this say geometrically?
10. Use Euler's formula to prove that $\cos\theta = \dfrac{e^{i\theta}+e^{-i\theta}}{2}$ and $\sin\theta = \dfrac{e^{i\theta}-e^{-i\theta}}{2i}$
11. A complex number z has $|z| = 5$ and $|z - 4| = 3$. Find z in exponential form.
12. Simplify $\dfrac{(1+i)^6}{(\sqrt{3}+i)^3}$ by converting to exponential form first.

---

### Answers

**Level 1**

1. (a) $r=2, \theta=\frac{\pi}{2}$: $z = 2(\cos\frac{\pi}{2}+i\sin\frac{\pi}{2})$
   (b) $r=4, \theta=\pi$: $z = 4(\cos\pi+i\sin\pi)$
   (c) $r=\sqrt{2}, \theta=\frac{\pi}{4}$: $z = \sqrt{2}(\cos\frac{\pi}{4}+i\sin\frac{\pi}{4})$
   (d) $r=2, \theta=-\frac{\pi}{6}$: $z = 2(\cos(-\frac{\pi}{6})+i\sin(-\frac{\pi}{6}))$

2. (a) $a=2\cos\frac{\pi}{2}=0$, $b=2\sin\frac{\pi}{2}=2$: **2i**
   (b) $a=4\cos\pi=-4$, $b=4\sin\pi=0$: **−4**
   (c) $a=3\cdot\frac{\sqrt{3}}{2}=\frac{3\sqrt{3}}{2}$, $b=3\cdot\frac{1}{2}=\frac{3}{2}$: $\boldsymbol{\frac{3\sqrt{3}}{2}+\frac{3}{2}i}$

3. (a) $r=1, \theta=0$: **$e^{i\cdot 0} = e^0 = 1$** (b) $r=1, \theta=\frac{\pi}{2}$: **$e^{i\pi/2}$** (c) $r=\sqrt{2}, \theta=\frac{3\pi}{4}$: **$\sqrt{2}\,e^{i\cdot3\pi/4}$**

**Level 2**

4. $z_1 z_2$: moduli $2\times3=6$, arguments $\frac{\pi}{4}+\frac{\pi}{4}=\frac{\pi}{2}$; result $= 6(\cos\frac{\pi}{2}+i\sin\frac{\pi}{2}) = 6i$; Cartesian: **6i**

5. $\frac{z_1}{z_2}$: moduli $\frac{6}{2}=3$, arguments $\frac{\pi}{3}-\frac{\pi}{6}=\frac{\pi}{6}$; polar: $3(\cos\frac{\pi}{6}+i\sin\frac{\pi}{6})$; Cartesian: $3\cdot\frac{\sqrt{3}}{2}+3\cdot\frac{1}{2}i =$ **$\frac{3\sqrt{3}}{2}+\frac{3}{2}i$**

6. $z^2 = (\sqrt{2})^2 e^{i\cdot2\cdot\pi/4} = 2e^{i\pi/2} = 2(\cos\frac{\pi}{2}+i\sin\frac{\pi}{2}) =$ **$2i$**

7. $iz = i(3+4i) = 3i+4i^2 = -4+3i$; original: $|3+4i|=5$, $\arg(3+4i)=\arctan(\frac{4}{3})\approx0.927$; new: $|-4+3i|=5$ ✓ (same modulus), $\arg(-4+3i)=\pi-\arctan(\frac{3}{4})\approx\pi-0.644\approx2.498\approx0.927+\frac{\pi}{2}$ ✓ (argument increased by exactly $\frac{\pi}{2}$)

**Level 3**

8. $z^2 = r^2 e^{i\cdot2\theta}$; we need $r^2=4$ (so $r=2$ ✓ given) and $2\theta=\frac{\pi}{2}+2k\pi$, giving $\theta=\frac{\pi}{4}$ or $\theta=\frac{\pi}{4}+\pi=\frac{5\pi}{4}$ (adjust to $-\frac{3\pi}{4}$); answers: $2e^{i\pi/4} = \sqrt{2}+\sqrt{2}i$ and $2e^{-i3\pi/4} = -\sqrt{2}-\sqrt{2}i$

9. $z = re^{i\theta} = r(\cos\theta+i\sin\theta) = r\cos\theta+ir\sin\theta$; $\bar{z}=r\cos\theta-ir\sin\theta = r(\cos\theta-i\sin\theta) = r(\cos(-\theta)+i\sin(-\theta)) = re^{-i\theta}$ ✓; Geometrically: the conjugate has the **same modulus but negated argument** — confirming it is the reflection in the real axis (from Day 5).

10. From Euler: $e^{i\theta}=\cos\theta+i\sin\theta$ and $e^{-i\theta}=\cos\theta-i\sin\theta$; Adding: $e^{i\theta}+e^{-i\theta}=2\cos\theta$, so $\cos\theta=\frac{e^{i\theta}+e^{-i\theta}}{2}$ ✓; Subtracting: $e^{i\theta}-e^{-i\theta}=2i\sin\theta$, so $\sin\theta=\frac{e^{i\theta}-e^{-i\theta}}{2i}$ ✓

11. $|z|=5$ means z lies on circle radius 5 centred at origin; $|z-4|=3$ means z lies on circle radius 3 centred at 4; let $z=a+bi$: $a^2+b^2=25$ and $(a-4)^2+b^2=9$; subtract: $a^2-(a-4)^2=16$; expand: $8a-16=16$, so $a=4$; then $b^2=25-16=9$, $b=\pm3$; for $z=4+3i$: $r=5$, $\theta=\arctan(\frac{3}{4})$; for $z=4-3i$: $r=5$, $\theta=-\arctan(\frac{3}{4})$; answers: $5e^{i\arctan(3/4)}$ and $5e^{-i\arctan(3/4)}$

12. Convert each: $1+i=\sqrt{2}e^{i\pi/4}$, so $(1+i)^6=(\sqrt{2})^6 e^{i6\pi/4}=8e^{i3\pi/2}=8e^{-i\pi/2}$; $\sqrt{3}+i=2e^{i\pi/6}$, so $(\sqrt{3}+i)^3=8e^{i\pi/2}$; divide: $\frac{8e^{-i\pi/2}}{8e^{i\pi/2}}=e^{-i\pi}=\cos(-\pi)+i\sin(-\pi)=$ **$-1$**

---

### Day 6 Summary

| Concept | Key Takeaway |
|---------|-------------|
| Polar form | $z = r(\cos\theta + i\sin\theta)$, where $r = |z|$ and $\theta = \arg(z)$ |
| Euler's formula | $e^{i\theta} = \cos\theta + i\sin\theta$ — the bridge between exp and trig |
| Exponential form | $z = re^{i\theta}$ — most compact form |
| Multiplication | Multiply moduli, ADD arguments |
| Division | Divide moduli, SUBTRACT arguments |
| Euler's identity | $e^{i\pi}+1=0$ — five constants, one equation |
| Multiply by i | Rotates anticlockwise by 90° — always |
| Multiply by $re^{i\theta}$ | Scales by r AND rotates by θ |
| Cartesian best for | Addition and subtraction |
| Polar/exponential best for | Multiplication, division, powers, roots |

