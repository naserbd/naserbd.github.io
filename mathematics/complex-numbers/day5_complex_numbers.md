## Day 5 — The Argand Diagram

---

### *"Giving complex numbers a home — the beautiful geometry of the complex plane"*

---

### Learning Objectives

By the end of Day 5, you will be able to:

- Plot any complex number on an **Argand diagram**
- Calculate the **modulus** of a complex number
- Calculate the **argument** of a complex number in both degrees and radians
- Interpret **addition** and **subtraction** geometrically as vector operations
- Understand what the conjugate looks like **visually**
- Describe **loci** of points on the Argand diagram using simple conditions

---

### Part 1 — From Algebra to Geometry

For four days you have worked with complex numbers purely algebraically — adding, subtracting, multiplying and dividing. Today everything gets a **visual form**.

The key insight is simple:

> A complex number **z = a + bi** can be plotted as the point **(a, b)** on a 2D coordinate plane.

This 2D plane has a special name:

$$\boxed{\text{The Argand Diagram (or the Complex Plane)}}$$

Named after the French mathematician **Jean-Robert Argand** (1768–1822), who published one of the first clear geometric interpretations of complex numbers.

### The Two Axes

| Axis | Direction | Represents |
|------|-----------|------------|
| Horizontal axis | Left ↔ Right | The **real part** (Re) |
| Vertical axis | Up ↕ Down | The **imaginary part** (Im) |

So the complex number **z = a + bi** is plotted at the coordinate **(a, b)** — exactly like a Cartesian point, where the x-coordinate is the real part and the y-coordinate is the imaginary part.

---

### Part 2 — Plotting Complex Numbers

### How to Plot z = a + bi

1. Draw a horizontal axis labelled **Re** (real axis)
2. Draw a vertical axis labelled **Im** (imaginary axis)
3. Move **a** units along the real axis (right if positive, left if negative)
4. Move **b** units up the imaginary axis (up if positive, down if negative)
5. Mark the point and label it

### Examples of Plotted Points

| Complex Number | Real Part (a) | Imaginary Part (b) | Location on Diagram |
|---------------|--------------|-------------------|---------------------|
| z = 3 + 4i | 3 | 4 | 3 right, 4 up |
| z = −2 + 3i | −2 | 3 | 2 left, 3 up |
| z = 4 − 2i | 4 | −2 | 4 right, 2 down |
| z = −3 − i | −3 | −1 | 3 left, 1 down |
| z = 5 | 5 | 0 | On the real axis |
| z = −4i | 0 | −4 | On the imaginary axis |
| z = 0 | 0 | 0 | The origin |

> 💡 **Key observations:**
> - All **real numbers** lie on the horizontal (real) axis
> - All **purely imaginary numbers** lie on the vertical (imaginary) axis
> - **General complex numbers** occupy the 2D plane off both axes

---

### Sketch of a Sample Argand Diagram

```
        Im
         |
     4 - |          • z = 4 + 4i
     3 - |    • z = 2 + 3i
     2 - |
     1 - |
         |
─────────+──────────────── Re
-3 -2 -1 | 1  2  3  4
    -1 - |
    -2 - |       • z = 3 − 2i
    -3 - |
         |
```

---

### Part 3 — The Modulus

### Definition

The **modulus** of a complex number z = a + bi is its **distance from the origin** on the Argand diagram. It is written as **|z|** and read as "mod z".

By Pythagoras' theorem applied to the right triangle formed by the real part, imaginary part, and the line from origin to the point:

$$\boxed{|z| = |a + bi| = \sqrt{a^2 + b^2}}$$

### Why Pythagoras?

If you draw the complex number z = a + bi on the Argand diagram:
- The horizontal leg of the right triangle has length **|a|**
- The vertical leg has length **|b|**
- The hypotenuse is the distance from origin to the point = **|z|**

By Pythagoras: $|z|^2 = a^2 + b^2$, so $|z| = \sqrt{a^2 + b^2}$

---

### Worked Examples — Modulus

**Example 1:** $z = 3 + 4i$

$$|z| = \sqrt{3^2 + 4^2} = \sqrt{9 + 16} = \sqrt{25} = 5$$

**Example 2:** $z = -5 + 12i$

$$|z| = \sqrt{(-5)^2 + 12^2} = \sqrt{25 + 144} = \sqrt{169} = 13$$

**Example 3:** $z = 1 - i$

$$|z| = \sqrt{1^2 + (-1)^2} = \sqrt{1 + 1} = \sqrt{2}$$

**Example 4:** $z = -3$

$$|z| = \sqrt{(-3)^2 + 0^2} = \sqrt{9} = 3$$

> 💡 For a real number, the modulus is simply its absolute value — exactly as expected.

---

### Key Properties of the Modulus

$$\boxed{|z| \geq 0} \qquad \text{(always non-negative)}$$

$$\boxed{|z| = 0 \iff z = 0} \qquad \text{(only zero has modulus zero)}$$

$$\boxed{|z| = |\bar{z}|} \qquad \text{(a number and its conjugate have the same modulus)}$$

$$\boxed{|z_1 z_2| = |z_1||z_2|} \qquad \text{(modulus of a product = product of moduli)}$$

$$\boxed{\left|\frac{z_1}{z_2}\right| = \frac{|z_1|}{|z_2|}} \qquad \text{(modulus of a quotient = quotient of moduli)}$$

$$\boxed{z \cdot \bar{z} = |z|^2} \qquad \text{(connects conjugate to modulus — from Day 4!)}$$

---

### Part 4 — The Argument

### Definition

The **argument** of a complex number z = a + bi is the **angle** that the line from the origin to z makes with the **positive real axis**. It is written as **arg(z)** and measured **anticlockwise** from the positive real axis.

$$\boxed{\arg(z) = \theta \quad \text{where} \quad \tan\theta = \frac{b}{a}}$$

> ⚠️ You cannot simply write $\theta = \arctan\!\left(\dfrac{b}{a}\right)$ without thinking about **which quadrant** z is in. The arctangent function only gives angles in the range $\left(-\dfrac{\pi}{2},\, \dfrac{\pi}{2}\right)$, but the argument can be in any quadrant. Always draw a diagram first!

### Principal Argument

The **principal argument** is the unique value of the argument in the range:

$$\boxed{-\pi < \arg(z) \leq \pi} \quad \text{(in radians)} \qquad \text{or} \qquad -180° < \arg(z) \leq 180° \quad \text{(in degrees)}$$

---

### Finding the Argument — Step by Step

1. Draw z on the Argand diagram
2. Identify which **quadrant** z is in
3. Find the **reference angle** $\alpha = \arctan\!\left(\dfrac{|b|}{|a|}\right)$ (always positive, always acute)
4. Adjust for the correct quadrant:

| Quadrant | Real part | Imaginary part | Argument θ |
|----------|-----------|----------------|------------|
| 1st (top-right) | a > 0 | b > 0 | $\theta = +\alpha$ |
| 2nd (top-left) | a < 0 | b > 0 | $\theta = \pi - \alpha$ |
| 3rd (bottom-left) | a < 0 | b < 0 | $\theta = -(\pi - \alpha) = \alpha - \pi$ |
| 4th (bottom-right) | a > 0 | b < 0 | $\theta = -\alpha$ |

---

### Worked Examples — Argument

**Example 1:** $z = 1 + i$ (1st quadrant)

$$\alpha = \arctan\!\left(\frac{1}{1}\right) = \arctan(1) = 45° = \frac{\pi}{4}$$

$$\arg(z) = +\frac{\pi}{4}$$

---

**Example 2:** $z = -1 + i$ (2nd quadrant)

$$\alpha = \arctan\!\left(\frac{1}{1}\right) = \frac{\pi}{4}$$

$$\arg(z) = \pi - \frac{\pi}{4} = \frac{3\pi}{4}$$

---

**Example 3:** $z = -\sqrt{3} - i$ (3rd quadrant)

$$\alpha = \arctan\!\left(\frac{1}{\sqrt{3}}\right) = \frac{\pi}{6}$$

$$\arg(z) = \frac{\pi}{6} - \pi = -\frac{5\pi}{6}$$

---

**Example 4:** $z = 1 - \sqrt{3}i$ (4th quadrant)

$$\alpha = \arctan\!\left(\frac{\sqrt{3}}{1}\right) = \frac{\pi}{3}$$

$$\arg(z) = -\frac{\pi}{3}$$

---

**Example 5 — Special cases on the axes:**

| z | Argument |
|---|----------|
| z = 5 (positive real) | arg(z) = 0 |
| z = −3 (negative real) | arg(z) = π |
| z = 2i (positive imaginary) | arg(z) = π/2 |
| z = −4i (negative imaginary) | arg(z) = −π/2 |

---

### Part 5 — Modulus and Argument Together

Together, the modulus r and argument θ give the **polar coordinates** of a complex number — a bridge to Day 6's polar form.

Every complex number can be described in two equivalent ways:

$$z = a + bi \quad \Longleftrightarrow \quad (r,\, \theta) \quad \text{where } r = |z|,\; \theta = \arg(z)$$

And the conversion back from polar to Cartesian:

$$\boxed{a = r\cos\theta, \qquad b = r\sin\theta}$$

So:

$$z = r\cos\theta + ir\sin\theta = r(\cos\theta + i\sin\theta)$$

This is the doorway to **polar form** — which you'll fully explore on Day 6!

---

### Worked Example — Finding Modulus and Argument Together

$$z = -2 + 2i$$

**Modulus:**
$$|z| = \sqrt{(-2)^2 + 2^2} = \sqrt{4 + 4} = \sqrt{8} = 2\sqrt{2}$$

**Argument** (2nd quadrant since a < 0, b > 0):
$$\alpha = \arctan\!\left(\frac{2}{2}\right) = \arctan(1) = \frac{\pi}{4}$$
$$\arg(z) = \pi - \frac{\pi}{4} = \frac{3\pi}{4}$$

**Polar description:** $r = 2\sqrt{2}$, $\theta = \dfrac{3\pi}{4}$

**Verify back:** $a = 2\sqrt{2}\cos\!\left(\dfrac{3\pi}{4}\right) = 2\sqrt{2} \times \left(-\dfrac{\sqrt{2}}{2}\right) = -2$ ✓
$b = 2\sqrt{2}\sin\!\left(\dfrac{3\pi}{4}\right) = 2\sqrt{2} \times \dfrac{\sqrt{2}}{2} = 2$ ✓

---

### Part 6 — Geometric Meaning of Operations

### Addition as Vector Addition

On the Argand diagram, complex numbers behave exactly like **position vectors**. Adding two complex numbers is the same as placing vectors tip to tail:

$$z_1 = 3 + i, \quad z_2 = 1 + 3i$$
$$z_1 + z_2 = 4 + 4i$$

This is identical to adding vectors $\begin{pmatrix}3\\1\end{pmatrix} + \begin{pmatrix}1\\3\end{pmatrix} = \begin{pmatrix}4\\4\end{pmatrix}$

### Subtraction as a Vector Difference

$$z_1 - z_2 = (3 + i) - (1 + 3i) = 2 - 2i$$

Geometrically, $z_1 - z_2$ is the vector **from $z_2$ to $z_1$** on the Argand diagram.

> 💡 **Useful fact:** The **distance** between two complex numbers $z_1$ and $z_2$ on the Argand diagram is:
> $$|z_1 - z_2| = \sqrt{(a_1-a_2)^2 + (b_1-b_2)^2}$$
> This is simply the distance formula from coordinate geometry!

---

### The Conjugate as a Reflection

On the Argand diagram, the conjugate $\bar{z} = a - bi$ is the **reflection of z in the real axis**.

- $z = 3 + 4i$ sits 4 units **above** the real axis
- $\bar{z} = 3 - 4i$ sits 4 units **below** the real axis — its mirror image

This beautifully explains why $|z| = |\bar{z}|$ — reflections preserve distance from the origin.

---

### Multiplication — A Sneak Preview

Multiplying by a complex number **rotates and scales** the original number. Multiplying z by i, for example, rotates z by exactly 90° anticlockwise. You'll see the full story on Day 6 with polar form.

---

### Part 7 — Loci on the Argand Diagram

A **locus** is the set of all points satisfying a given condition. In the Argand diagram, loci produce geometric shapes — circles, lines, and more.

### Locus Type 1 — Circle: $|z - z_0| = r$

The condition $|z - z_0| = r$ means:

> "The distance from z to the fixed point $z_0$ equals r"

This is a **circle** with centre $z_0$ and radius r.

**Example:** $|z - (2 + 3i)| = 5$

This is a circle with centre $(2, 3)$ and radius $5$ on the Argand diagram.

**Special case:** $|z| = r$ is a circle centred at the **origin** with radius r.

---

### Locus Type 2 — Perpendicular Bisector: $|z - z_1| = |z - z_2|$

The condition $|z - z_1| = |z - z_2|$ means:

> "z is equidistant from the two fixed points $z_1$ and $z_2$"

This is the **perpendicular bisector** of the line segment joining $z_1$ and $z_2$.

**Example:** $|z - 3| = |z - i|$

This is the perpendicular bisector of the segment joining $(3, 0)$ and $(0, 1)$.

---

### Locus Type 3 — Half-Line: $\arg(z - z_0) = \theta$

The condition $\arg(z - z_0) = \theta$ means:

> "The angle from fixed point $z_0$ to z equals θ"

This is a **half-line** (ray) starting at $z_0$ (but not including $z_0$ itself) at angle θ from the positive real direction.

**Example:** $\arg(z - 1) = \dfrac{\pi}{4}$

This is a ray starting at the point $(1, 0)$, heading in the direction of 45° from the positive real axis.

---

### Part 8 — The Map Analogy Revisited

On Day 1, you imagined real numbers as East-West movement and imaginary numbers as North-South movement. Now you can make this precise:

| Map Concept | Argand Diagram Equivalent |
|-------------|--------------------------|
| Position on map | Complex number z = a + bi |
| Distance from town centre | Modulus \|z\| |
| Compass bearing (from East, anticlockwise) | Argument arg(z) |
| Walking East | Moving along positive real axis |
| Walking North | Moving along positive imaginary axis |
| Mirror image across East-West road | Complex conjugate z̄ |
| How far apart are two towns? | $\|z_1 - z_2\|$ |

---

### Part 9 — Key Rules to Memorise

$$\boxed{|z| = \sqrt{a^2 + b^2}} \qquad \text{(modulus = distance from origin)}$$

$$\boxed{\arg(z) = \theta \text{ where } \tan\theta = \frac{b}{a}, \quad -\pi < \theta \leq \pi} \qquad \text{(always check quadrant!)}$$

$$\boxed{a = r\cos\theta, \quad b = r\sin\theta} \qquad \text{(polar to Cartesian conversion)}$$

$$\boxed{|z_1 - z_2| = \text{distance between } z_1 \text{ and } z_2} \qquad \text{(distance formula)}$$

$$\boxed{|z - z_0| = r \implies \text{circle, centre } z_0 \text{, radius } r}$$

$$\boxed{|z - z_1| = |z - z_2| \implies \text{perpendicular bisector of } z_1z_2}$$

$$\boxed{\bar{z} \text{ is the reflection of } z \text{ in the real axis}}$$

---

### Part 10 — Common Mistakes to Avoid

| Mistake | Wrong | Correct |
|---------|-------|---------|
| Using arctan blindly | $\arg(-1+i) = \arctan(-1) = -\frac{\pi}{4}$ | Draw diagram first: answer is $\frac{3\pi}{4}$ |
| Squaring without root | $\|3+4i\| = 9 + 16 = 25$ | $= \sqrt{25} =$ **5** |
| Forgetting negative signs in modulus | $\|-3+4i\| = \sqrt{(-3)^2+4^2}$... stops at $\sqrt{-9+16}$ | $(-3)^2 = +9$, so $\sqrt{9+16} =$ **5** |
| Wrong range for argument | $\arg(-1) = 0$ | $\arg(-1) =$ **π** |
| Labelling axes wrongly | Calling Re axis vertical | Re is **horizontal**, Im is **vertical** |
| Including $z_0$ in half-line locus | Drawing filled dot at start | Half-line has an **open** point at $z_0$ |

---

### Practice Problems

Try these yourself before checking answers!

**Level 1 — Basic**

1. Plot these on an Argand diagram: $z_1 = 2+3i$, $z_2 = -1+2i$, $z_3 = 4-i$, $z_4 = -3-2i$
2. Find the modulus of: (a) $z = 5 + 12i$ (b) $z = -3 + 4i$ (c) $z = 2 - 2i$ (d) $z = -6$
3. Find the argument (in radians) of: (a) $z = 1$ (b) $z = i$ (c) $z = -1$ (d) $z = -i$

**Level 2 — Intermediate**

4. Find the modulus and argument of $z = -1 + \sqrt{3}i$
5. Find the modulus and argument of $z = \sqrt{3} - i$
6. If $z_1 = 3 + 4i$ and $z_2 = -1 + 2i$, find $|z_1 - z_2|$
7. Describe the locus of points satisfying $|z - 2 - i| = 3$
8. Show that $|z|^2 = z \cdot \bar{z}$ for $z = 3 + 4i$

**Level 3 — Challenge**

9. Find all complex numbers z such that $|z| = \arg(z) = \frac{\pi}{4}$ — express in the form a + bi
10. Describe the locus: $|z - 3| = |z + 1|$
11. If $|z - 1| = |z - i|$, show that $\text{Re}(z) = \text{Im}(z)$
12. A complex number z has modulus 2 and argument $\frac{2\pi}{3}$. Find z in the form a + bi, giving exact values.

---

### Answers

**Level 1**

1. Plot the four points: (2,3), (−1,2), (4,−1), (−3,−2) on the Re-Im plane. *(Use squared paper if possible!)*
2. (a) $\sqrt{25+144} = \sqrt{169} =$ **13** (b) $\sqrt{9+16} = \sqrt{25} =$ **5** (c) $\sqrt{4+4} = \sqrt{8} = $ **$2\sqrt{2}$** (d) $\sqrt{36} =$ **6**
3. (a) $\arg(1) =$ **0** (b) $\arg(i) =$ **$\frac{\pi}{2}$** (c) $\arg(-1) =$ **$\pi$** (d) $\arg(-i) =$ **$-\frac{\pi}{2}$**

**Level 2**

4. $|-1+\sqrt{3}i| = \sqrt{1+3} = \sqrt{4} =$ **2**; 2nd quadrant: $\alpha = \arctan(\sqrt{3}/1) = \frac{\pi}{3}$, so $\arg = \pi - \frac{\pi}{3} =$ **$\frac{2\pi}{3}$**

5. $|\sqrt{3}-i| = \sqrt{3+1} = 2$; 4th quadrant: $\alpha = \arctan(1/\sqrt{3}) = \frac{\pi}{6}$, so $\arg =$ **$-\frac{\pi}{6}$**

6. $z_1 - z_2 = (3-(-1)) + (4-2)i = 4 + 2i$; $|4+2i| = \sqrt{16+4} = \sqrt{20} =$ **$2\sqrt{5}$**

7. Circle with **centre (2, 1)** and **radius 3** on the Argand diagram

8. $z \cdot \bar{z} = (3+4i)(3-4i) = 9+16 = 25$; $|z|^2 = (\sqrt{3^2+4^2})^2 = 25$ ✓

**Level 3**

9. We need $|z| = \frac{\pi}{4}$ and $\arg(z) = \frac{\pi}{4}$; so $r = \frac{\pi}{4}$, $\theta = \frac{\pi}{4}$; thus $a = \frac{\pi}{4}\cos\frac{\pi}{4} = \frac{\pi}{4} \cdot \frac{\sqrt{2}}{2} = \frac{\pi\sqrt{2}}{8}$, $b = \frac{\pi\sqrt{2}}{8}$; Answer: $z = \frac{\pi\sqrt{2}}{8} + \frac{\pi\sqrt{2}}{8}i$

10. $|z-3| = |z+1|$ means z is equidistant from $(3,0)$ and $(-1,0)$; this is the **perpendicular bisector** of the segment joining these points: the vertical line $\text{Re}(z) = 1$

11. $|z-1|^2 = |z-i|^2$; let $z = a+bi$: $(a-1)^2+b^2 = a^2+(b-1)^2$; expand: $a^2-2a+1+b^2 = a^2+b^2-2b+1$; simplify: $-2a = -2b$; therefore $a = b$, i.e. $\text{Re}(z) = \text{Im}(z)$ ✓

12. $a = 2\cos\frac{2\pi}{3} = 2 \times (-\frac{1}{2}) = -1$; $b = 2\sin\frac{2\pi}{3} = 2 \times \frac{\sqrt{3}}{2} = \sqrt{3}$; Answer: $z =$ **$-1 + \sqrt{3}i$**

---

### Day 5 Summary

| Concept | Key Takeaway |
|---------|-------------|
| Argand diagram | z = a+bi plotted at point (a, b); Re is horizontal, Im is vertical |
| Modulus \|z\| | Distance from origin: $\sqrt{a^2+b^2}$ |
| Argument arg(z) | Angle from positive real axis: $-\pi < \theta \leq \pi$ |
| Quadrant rule | Always draw diagram before computing argument |
| Polar form preview | $z = r(\cos\theta + i\sin\theta)$ with $a = r\cos\theta$, $b = r\sin\theta$ |
| Vector addition | Adding complex numbers = placing vectors tip to tail |
| Conjugate geometry | $\bar{z}$ is the reflection of z in the real axis |
| Distance formula | Distance between $z_1$ and $z_2$ = $\|z_1 - z_2\|$ |
| Circle locus | $\|z - z_0\| = r$ is a circle, centre $z_0$, radius r |
| Bisector locus | $\|z - z_1\| = \|z - z_2\|$ is the perpendicular bisector |
