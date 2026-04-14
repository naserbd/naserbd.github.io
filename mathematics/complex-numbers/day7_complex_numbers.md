## Day 7 — De Moivre's Theorem, nth Roots & Real-World Applications

---

### *"The grand finale — power, elegance, and the world beyond the classroom"*

---

### Learning Objectives

By the end of Day 7, you will be able to:

- State and apply **De Moivre's theorem** to raise complex numbers to any integer power
- Find all **nth roots** of any complex number
- Recognise that nth roots are **equally spaced** on a circle in the Argand diagram
- Use De Moivre's theorem to derive **trigonometric identities**
- Appreciate where complex numbers appear in **real-world applications**
- Consolidate everything from Days 1–6 into a unified picture

---

### Part 1 — The Problem De Moivre Solved

By Day 6 you knew that multiplying two complex numbers in polar form means:

$$z_1 z_2 = r_1 r_2\,e^{i(\theta_1+\theta_2)}$$

Now ask: what if both numbers are the **same**? What is $z^n$?

$$z^2 = z \cdot z = r \cdot r\,e^{i(\theta+\theta)} = r^2 e^{i \cdot 2\theta}$$

$$z^3 = z^2 \cdot z = r^2 e^{i \cdot 2\theta} \cdot r\,e^{i\theta} = r^3 e^{i \cdot 3\theta}$$

The pattern is clear: every time you multiply by z, the modulus is multiplied by r and the argument increases by θ. After n multiplications:

$$\boxed{z^n = r^n e^{in\theta}}$$

In polar form this is:

$$\boxed{\left[r(\cos\theta + i\sin\theta)\right]^n = r^n(\cos n\theta + i\sin n\theta)}$$

This is **De Moivre's Theorem**, named after the French-British mathematician **Abraham de Moivre** (1667–1754).

---

### Part 2 — De Moivre's Theorem in Full

### The Theorem

For any complex number $z = r(\cos\theta + i\sin\theta)$ and any **integer** n:

$$\boxed{\left[r(\cos\theta + i\sin\theta)\right]^n = r^n(\cos n\theta + i\sin n\theta)}$$

Equivalently, for $z = re^{i\theta}$:

$$\boxed{z^n = r^n e^{in\theta}}$$

**The rule in words:**
> To raise a complex number to the power n — raise the modulus to the power n, and multiply the argument by n.

### Scope of the Theorem

| Value of n | Valid? | Example |
|-----------|--------|---------|
| Positive integer | ✅ Yes | $z^5$ |
| Zero | ✅ Yes | $z^0 = 1$ (any non-zero z) |
| Negative integer | ✅ Yes | $z^{-3} = \frac{1}{z^3}$ |
| Fraction (for roots) | ✅ Yes (with care) | $z^{1/n}$ gives nth roots |

---

### Part 3 — Applying De Moivre's Theorem to Powers

### Worked Example 1 — Positive Integer Power

$$\text{Find } (1 + i)^8$$

**Step 1 — Convert to polar form:**
$$r = \sqrt{1^2+1^2} = \sqrt{2}, \qquad \theta = \frac{\pi}{4}$$
$$1 + i = \sqrt{2}\!\left(\cos\frac{\pi}{4}+i\sin\frac{\pi}{4}\right)$$

**Step 2 — Apply De Moivre:**
$$(\sqrt{2})^8\!\left(\cos\!\left(8 \times \frac{\pi}{4}\right)+i\sin\!\left(8 \times \frac{\pi}{4}\right)\right)$$
$$= 2^4(\cos 2\pi + i\sin 2\pi)$$
$$= 16(1 + 0i) = 16$$

**Answer: $(1+i)^8 = 16$** ✓

> ✨ Try expanding $(1+i)^8$ by repeated FOIL — it would take dozens of steps. De Moivre gives the answer in three lines.

---

### Worked Example 2 — Large Power

$$\text{Find } \left(\sqrt{3}+i\right)^{10}$$

**Step 1 — Polar form:**
$$r = \sqrt{3+1} = 2, \qquad \theta = \arctan\!\left(\frac{1}{\sqrt{3}}\right) = \frac{\pi}{6}$$
$$\sqrt{3}+i = 2\!\left(\cos\frac{\pi}{6}+i\sin\frac{\pi}{6}\right)$$

**Step 2 — Apply De Moivre:**
$$2^{10}\!\left(\cos\frac{10\pi}{6}+i\sin\frac{10\pi}{6}\right)$$
$$= 1024\!\left(\cos\frac{5\pi}{3}+i\sin\frac{5\pi}{3}\right)$$

**Step 3 — Adjust argument to principal range** ($\frac{5\pi}{3} > \pi$, so subtract $2\pi$):
$$\frac{5\pi}{3} - 2\pi = -\frac{\pi}{3}$$

**Step 4 — Evaluate:**
$$= 1024\!\left(\cos\!\left(-\frac{\pi}{3}\right)+i\sin\!\left(-\frac{\pi}{3}\right)\right)$$
$$= 1024\!\left(\frac{1}{2} - \frac{\sqrt{3}}{2}i\right)$$
$$= 512 - 512\sqrt{3}i$$

**Answer:** $512 - 512\sqrt{3}i$ ✓

---

### Worked Example 3 — Negative Integer Power

$$\text{Find } (1+i)^{-4}$$

**Step 1 — Polar form:**
$$1+i = \sqrt{2}\!\left(\cos\frac{\pi}{4}+i\sin\frac{\pi}{4}\right)$$

**Step 2 — Apply De Moivre with n = −4:**
$$\left(\sqrt{2}\right)^{-4}\!\left(\cos\!\left(-\frac{4\pi}{4}\right)+i\sin\!\left(-\frac{4\pi}{4}\right)\right)$$
$$= \frac{1}{4}\!\left(\cos(-\pi)+i\sin(-\pi)\right)$$
$$= \frac{1}{4}(-1 + 0i) = -\frac{1}{4}$$

**Answer:** $(1+i)^{-4} = -\dfrac{1}{4}$ ✓

---

### Part 4 — Finding nth Roots

This is one of the most beautiful results in the entire course.

### The Fundamental Question

If $z^n = w$, what are all the possible values of z?

In real numbers, $x^2 = 9$ has just 2 solutions: $x = \pm 3$.

In complex numbers, **$z^n = w$ always has exactly n solutions** — the **nth roots** of w.

### The nth Root Formula

Let $w = Re^{i\phi}$ (the number we want to find roots of). Then the n roots are:

$$\boxed{z_k = R^{1/n}\,\exp\!\left(i\cdot\frac{\phi + 2\pi k}{n}\right) = R^{1/n}\!\left(\cos\frac{\phi+2\pi k}{n}+i\sin\frac{\phi+2\pi k}{n}\right)}$$

for $k = 0, 1, 2, \ldots, n-1$

### The Pizza Slice Pattern 🍕

All n roots have the **same modulus** $R^{1/n}$, so they all lie on a **circle** of radius $R^{1/n}$ in the Argand diagram.

Their arguments are equally spaced by $\dfrac{2\pi}{n}$ — like **perfectly equal pizza slices**, each separated by the same angle.

> **The n roots of any complex number form a regular n-sided polygon inscribed in a circle of radius $R^{1/n}$ centred at the origin.**

---

### Worked Example 4 — Square Roots of a Complex Number

$$\text{Find the two square roots of } z^2 = i$$

**Step 1 — Write i in polar form:**
$$i = 1\cdot e^{i\pi/2}, \quad \text{so } R = 1, \; \phi = \frac{\pi}{2}, \; n = 2$$

**Step 2 — Apply the formula for k = 0 and k = 1:**

For $k = 0$:
$$z_0 = 1^{1/2}\!\left(\cos\frac{\pi/2}{2}+i\sin\frac{\pi/2}{2}\right) = \cos\frac{\pi}{4}+i\sin\frac{\pi}{4} = \frac{\sqrt{2}}{2}+\frac{\sqrt{2}}{2}i$$

For $k = 1$:
$$z_1 = \cos\frac{\pi/2+2\pi}{2}+i\sin\frac{\pi/2+2\pi}{2} = \cos\frac{5\pi}{4}+i\sin\frac{5\pi}{4} = -\frac{\sqrt{2}}{2}-\frac{\sqrt{2}}{2}i$$

**Answers:** $z_0 = \dfrac{\sqrt{2}}{2}+\dfrac{\sqrt{2}}{2}i$ and $z_1 = -\dfrac{\sqrt{2}}{2}-\dfrac{\sqrt{2}}{2}i$ ✓

> 💡 Notice $z_1 = -z_0$ — the two square roots are always negatives of each other, just like $\pm3$ are the square roots of 9.

---

### Worked Example 5 — Cube Roots of Unity

$$\text{Find all solutions of } z^3 = 1$$

The three **cube roots of unity** are among the most important complex numbers in all of mathematics.

**Step 1 — Polar form of 1:**
$$1 = 1\cdot e^{i\cdot 0}, \quad R = 1, \; \phi = 0, \; n = 3$$

**Step 2 — Apply formula for k = 0, 1, 2:**

For $k = 0$:
$$z_0 = \cos 0 + i\sin 0 = 1$$

For $k = 1$:
$$z_1 = \cos\frac{2\pi}{3}+i\sin\frac{2\pi}{3} = -\frac{1}{2}+\frac{\sqrt{3}}{2}i$$

For $k = 2$:
$$z_2 = \cos\frac{4\pi}{3}+i\sin\frac{4\pi}{3} = -\frac{1}{2}-\frac{\sqrt{3}}{2}i$$

**Geometric picture:** These three points sit at the vertices of an **equilateral triangle** inscribed in the unit circle, spaced $120°$ apart.

**Key property:** The three roots always sum to zero:
$$z_0 + z_1 + z_2 = 1 + \left(-\frac{1}{2}+\frac{\sqrt{3}}{2}i\right) + \left(-\frac{1}{2}-\frac{\sqrt{3}}{2}i\right) = 0 \checkmark$$

> 🌟 **The sum of all nth roots of unity is always zero** — a profound and beautiful fact.

---

### Worked Example 6 — Fourth Roots of −16

$$\text{Find all solutions of } z^4 = -16$$

**Step 1 — Polar form of −16:**
$$-16 = 16\cdot e^{i\pi}, \quad R = 16, \; \phi = \pi, \; n = 4$$

**Step 2 — Modulus of roots:**
$$R^{1/4} = 16^{1/4} = 2$$

**Step 3 — Apply formula for k = 0, 1, 2, 3:**

For $k = 0$: $\theta_0 = \dfrac{\pi}{4}$, so $z_0 = 2\!\left(\cos\dfrac{\pi}{4}+i\sin\dfrac{\pi}{4}\right) = \sqrt{2}+\sqrt{2}i$

For $k = 1$: $\theta_1 = \dfrac{3\pi}{4}$, so $z_1 = 2\!\left(\cos\dfrac{3\pi}{4}+i\sin\dfrac{3\pi}{4}\right) = -\sqrt{2}+\sqrt{2}i$

For $k = 2$: $\theta_2 = \dfrac{5\pi}{4} \to -\dfrac{3\pi}{4}$, so $z_2 = -\sqrt{2}-\sqrt{2}i$

For $k = 3$: $\theta_3 = \dfrac{7\pi}{4} \to -\dfrac{\pi}{4}$, so $z_3 = \sqrt{2}-\sqrt{2}i$

**Geometric picture:** A perfect **square** inscribed in a circle of radius 2, rotated 45° from the axes. ✓

---

### Part 5 — Deriving Trigonometric Identities

One of the most powerful applications of De Moivre's theorem is deriving **multiple-angle formulas** for cos(nθ) and sin(nθ).

### Method

Use De Moivre combined with the binomial expansion:

$$\cos n\theta + i\sin n\theta = (\cos\theta + i\sin\theta)^n$$

Expand the right side using the binomial theorem, then:
- **Real part** of expansion = $\cos n\theta$
- **Imaginary part** of expansion = $\sin n\theta$

---

### Worked Example 7 — Double Angle Formulas (n = 2)

$$(\cos\theta + i\sin\theta)^2 = \cos 2\theta + i\sin 2\theta$$

**Expand left side:**
$$\cos^2\theta + 2i\cos\theta\sin\theta + i^2\sin^2\theta$$
$$= (\cos^2\theta - \sin^2\theta) + i(2\sin\theta\cos\theta)$$

**Equate real and imaginary parts:**
$$\cos 2\theta = \cos^2\theta - \sin^2\theta$$
$$\sin 2\theta = 2\sin\theta\cos\theta$$

These are the **double angle formulas** — derived in a single step from De Moivre! ✓

---

### Worked Example 8 — Triple Angle Formulas (n = 3)

$$(\cos\theta + i\sin\theta)^3 = \cos 3\theta + i\sin 3\theta$$

**Expand left side using binomial theorem:**
$$\cos^3\theta + 3\cos^2\theta(i\sin\theta) + 3\cos\theta(i\sin\theta)^2 + (i\sin\theta)^3$$
$$= \cos^3\theta + 3i\cos^2\theta\sin\theta - 3\cos\theta\sin^2\theta - i\sin^3\theta$$
$$= (\cos^3\theta - 3\cos\theta\sin^2\theta) + i(3\cos^2\theta\sin\theta - \sin^3\theta)$$

**Equate parts:**
$$\cos 3\theta = \cos^3\theta - 3\cos\theta\sin^2\theta = 4\cos^3\theta - 3\cos\theta$$
$$\sin 3\theta = 3\cos^2\theta\sin\theta - \sin^3\theta = 3\sin\theta - 4\sin^3\theta$$

> 💡 These identities would take pages to derive any other way. De Moivre produces them in moments.

---

### Worked Example 9 — Powers of cos and sin

De Moivre also works in reverse — expressing $\cos^n\theta$ and $\sin^n\theta$ as multiple angles.

Using $z = e^{i\theta}$ and $z^{-1} = e^{-i\theta}$:

$$z + z^{-1} = 2\cos\theta \qquad z - z^{-1} = 2i\sin\theta$$

**Express $\cos^3\theta$ in terms of multiple angles:**

$$\left(\frac{z+z^{-1}}{2}\right)^3 = \frac{1}{8}(z^3 + 3z + 3z^{-1} + z^{-3})$$

$$= \frac{1}{8}\!\left((z^3+z^{-3}) + 3(z+z^{-1})\right)$$

$$= \frac{1}{8}(2\cos 3\theta + 3 \times 2\cos\theta)$$

$$\cos^3\theta = \frac{1}{4}\cos 3\theta + \frac{3}{4}\cos\theta$$

This type of result is essential in **integration** — turning $\cos^3\theta$ into something integrable.

---

### Part 6 — Real-World Applications

Complex numbers are not just abstract mathematics. They are the essential language of modern science and engineering.

---

### Application 1 — Electrical Engineering (AC Circuits)

In alternating current (AC) circuits, voltages and currents oscillate sinusoidally. Engineers represent them as complex numbers called **phasors**:

$$V = V_0 e^{i\omega t} \qquad \text{(voltage as a rotating complex number)}$$

Where $\omega$ is the angular frequency and t is time. The real part gives the actual physical voltage.

- **Resistors** multiply the phasor by a real number (no phase change)
- **Capacitors** multiply by $\dfrac{1}{i\omega C}$ — a 90° phase shift
- **Inductors** multiply by $i\omega L$ — another 90° phase shift

Adding voltages across components becomes **complex addition**. Impedance (like resistance but for AC) is a complex number $Z = R + iX$. Without complex numbers, AC circuit analysis would be intractable.

---

### Application 2 — Quantum Mechanics

The **Schrödinger equation** — the fundamental equation of quantum physics — is written in terms of complex numbers:

$$i\hbar\frac{\partial\psi}{\partial t} = \hat{H}\psi$$

The wave function $\psi$ is a complex-valued function. Its modulus squared $|\psi|^2$ gives the probability of finding a particle at a given location. Complex numbers are not just convenient here — they are **physically necessary**.

---

### Application 3 — Signal Processing & Fourier Analysis

The **Fourier transform** decomposes any signal (sound, image, radio wave) into its frequency components. It is defined using complex exponentials:

$$\hat{f}(\xi) = \int_{-\infty}^{\infty} f(t)\,e^{-2\pi i\xi t}\,dt$$

Every time you use MP3 audio, JPEG images, mobile phone signals, or MRI scans, you are using this transform — and therefore using complex numbers — whether you know it or not.

---

### Application 4 — Fluid Dynamics & Aerodynamics

**Complex potential flow** uses complex functions to model how fluids move around objects. Engineers designing aircraft wings use **conformal mapping** — a technique based entirely on complex analysis — to transform simple flow patterns into realistic airfoil shapes.

---

### Application 5 — Fractals and Computer Graphics

The famous **Mandelbrot set** is defined using a simple complex iteration:

$$z_{n+1} = z_n^2 + c$$

Starting from $z_0 = 0$, a point $c$ in the complex plane belongs to the Mandelbrot set if this sequence never escapes to infinity. The resulting boundary produces one of the most intricate and beautiful structures in mathematics — infinite self-similar complexity from a single line of algebra.

---

### Application 6 — Control Theory & Robotics

The **stability** of engineering systems (autopilots, robot arms, chemical plant controllers) is analysed by plotting the **poles** of a transfer function — which are complex numbers — on the complex plane. A system is stable if and only if all its poles lie in the left half of the complex plane (negative real part). Complex numbers are the language of stability analysis.

---

### Part 7 — The Fundamental Theorem of Algebra

De Moivre's theorem and complex numbers together complete one of the greatest theorems in all of mathematics:

$$\boxed{\text{Every polynomial of degree n has exactly n roots in } \mathbb{C}}$$

This is the **Fundamental Theorem of Algebra**, first proved rigorously by Gauss in 1799.

It means:
- $z^2 + 1 = 0$ has 2 roots: $z = \pm i$
- $z^3 - 1 = 0$ has 3 roots: the cube roots of unity
- $z^5 + 3z^3 - z + 2 = 0$ has exactly 5 roots (counting multiplicity) in $\mathbb{C}$

The complex numbers are **algebraically closed** — you never need to invent any more new numbers beyond $\mathbb{C}$. The journey that started on Day 1 with "what is $\sqrt{-1}$?" ends here: the complex numbers are the **complete and final number system** for algebra.

---

### Part 8 — Key Rules to Memorise

$$\boxed{[r(\cos\theta+i\sin\theta)]^n = r^n(\cos n\theta + i\sin n\theta)} \qquad \text{(De Moivre's theorem)}$$

$$\boxed{z^n = r^n e^{in\theta}} \qquad \text{(exponential form)}$$

$$\boxed{z_k = R^{1/n}\!\left(\cos\frac{\phi+2\pi k}{n}+i\sin\frac{\phi+2\pi k}{n}\right), \quad k=0,1,\ldots,n-1} \qquad \text{(nth roots)}$$

$$\boxed{\text{n roots lie on a circle of radius } R^{1/n}\text{, equally spaced by angle }\frac{2\pi}{n}}$$

$$\boxed{\text{Sum of all nth roots of unity} = 0}$$

$$\text{Real part of }(\cos\theta+i\sin\theta)^n = \cos n\theta$$

$$\text{Imaginary part of }(\cos\theta+i\sin\theta)^n = \sin n\theta$$

---

### Part 9 — Common Mistakes to Avoid

| Mistake | Wrong | Correct |
|---------|-------|---------|
| Applying De Moivre in Cartesian form | $(1+i)^8 = 1^8 + i^8$ | Convert to **polar first**, then apply |
| Multiplying argument instead of scaling | $(re^{i\theta})^n = re^{in\theta}$ | Modulus must ALSO be raised: $r^ne^{in\theta}$ |
| Finding only one nth root | $z^3 = 1$ has solution $z=1$ | There are **3 roots**: use $k=0,1,2$ |
| Stopping k too early | k runs 0 to n | k runs **0 to n−1** (n values total) |
| Forgetting to adjust argument | $\theta = \frac{5\pi}{3}$ left as is | Subtract $2\pi$: $\theta = -\frac{\pi}{3}$ |
| Wrong trig identity derivation | Setting real = $\sin n\theta$ | Real part = $\cos n\theta$, imaginary = $\sin n\theta$ |

---

### Practice Problems

Try these yourself before checking answers!

**Level 1 — Basic**

1. Use De Moivre's theorem to find $(1+i)^4$
2. Find $\left(\cos\dfrac{\pi}{6}+i\sin\dfrac{\pi}{6}\right)^6$
3. Find $\left(\sqrt{3}+i\right)^4$
4. Write down all cube roots of $-1$ (i.e. solve $z^3 = -1$)

**Level 2 — Intermediate**

5. Find all fourth roots of $z^4 = 16$ and plot them on the Argand diagram
6. Use De Moivre's theorem to show that $\cos 2\theta = 1 - 2\sin^2\theta$
7. Find $(1-i)^{10}$ in Cartesian form
8. Find all solutions of $z^3 = 8i$

**Level 3 — Challenge**

9. Using De Moivre's theorem, show that:
$$\cos 4\theta = 8\cos^4\theta - 8\cos^2\theta + 1$$

10. Show that the nth roots of unity satisfy $1 + \omega + \omega^2 + \cdots + \omega^{n-1} = 0$, where $\omega = e^{2\pi i/n}$

11. If $z = \cos\theta + i\sin\theta$, use the result $z^n + z^{-n} = 2\cos n\theta$ to express $\cos^4\theta$ in terms of multiple angles, and hence evaluate $\displaystyle\int_0^{\pi/2}\cos^4\theta\,d\theta$

12. The transformation $w = \dfrac{z+1}{z-1}$ maps complex numbers from the z-plane to the w-plane. Show that if $|z| = 1$ (the unit circle in the z-plane), then $w$ is purely imaginary.

---

### Answers

**Level 1**

1. $1+i = \sqrt{2}e^{i\pi/4}$; $(1+i)^4 = (\sqrt{2})^4 e^{i\pi} = 4(\cos\pi+i\sin\pi) = 4(-1) =$ **$-4$**

2. $\left(\cos\frac{\pi}{6}+i\sin\frac{\pi}{6}\right)^6 = \cos\left(6\cdot\frac{\pi}{6}\right)+i\sin\left(6\cdot\frac{\pi}{6}\right) = \cos\pi+i\sin\pi =$ **$-1$**

3. $\sqrt{3}+i = 2e^{i\pi/6}$; $(\sqrt{3}+i)^4 = 2^4 e^{i\cdot4\pi/6} = 16\left(\cos\frac{2\pi}{3}+i\sin\frac{2\pi}{3}\right) = 16\left(-\frac{1}{2}+\frac{\sqrt{3}}{2}i\right) =$ **$-8+8\sqrt{3}i$**

4. $-1 = e^{i\pi}$, $n=3$, $R=1$; roots: $k=0$: $e^{i\pi/3} = \frac{1}{2}+\frac{\sqrt{3}}{2}i$; $k=1$: $e^{i\pi} = -1$; $k=2$: $e^{i5\pi/3} = \frac{1}{2}-\frac{\sqrt{3}}{2}i$; answers: **$\dfrac{1}{2}\pm\dfrac{\sqrt{3}}{2}i$ and $-1$**

**Level 2**

5. $16 = 16e^{i\cdot0}$; $R^{1/4}=2$; spacing $\frac{2\pi}{4}=\frac{\pi}{2}$; roots: $z_0=2$, $z_1=2i$, $z_2=-2$, $z_3=-2i$; these form a **square** on the circle of radius 2; answers: **$\pm2, \pm2i$**

6. From Example 7: $\cos2\theta = \cos^2\theta-\sin^2\theta$; since $\cos^2\theta = 1-\sin^2\theta$: $\cos2\theta = (1-\sin^2\theta)-\sin^2\theta = 1-2\sin^2\theta$ ✓

7. $1-i = \sqrt{2}e^{-i\pi/4}$; $(1-i)^{10} = (\sqrt{2})^{10}e^{-i10\pi/4} = 32\,e^{-i5\pi/2}$; adjust: $-\frac{5\pi}{2}+2\pi = -\frac{\pi}{2}$; $= 32\left(\cos(-\frac{\pi}{2})+i\sin(-\frac{\pi}{2})\right) = 32(0-i) =$ **$-32i$**

8. $8i = 8e^{i\pi/2}$; $R^{1/3}=2$; $k=0$: $\theta=\frac{\pi}{6}$: $z_0=2(\cos\frac{\pi}{6}+i\sin\frac{\pi}{6})=\sqrt{3}+i$; $k=1$: $\theta=\frac{\pi}{6}+\frac{2\pi}{3}=\frac{5\pi}{6}$: $z_1=2(\cos\frac{5\pi}{6}+i\sin\frac{5\pi}{6})=-\sqrt{3}+i$; $k=2$: $\theta=\frac{\pi}{6}+\frac{4\pi}{3}=\frac{3\pi}{2}\to-\frac{\pi}{2}$: $z_2=2(0-i)=-2i$; answers: **$\sqrt{3}+i,\; -\sqrt{3}+i,\; -2i$**

**Level 3**

9. $(\cos\theta+i\sin\theta)^4 = \cos4\theta+i\sin4\theta$; expand by binomial: $\cos^4\theta + 4\cos^3\theta(i\sin\theta)+6\cos^2\theta(i\sin\theta)^2+4\cos\theta(i\sin\theta)^3+(i\sin\theta)^4$; $= \cos^4\theta+4i\cos^3\theta\sin\theta-6\cos^2\theta\sin^2\theta-4i\cos\theta\sin^3\theta+\sin^4\theta$; real part: $\cos4\theta = \cos^4\theta-6\cos^2\theta\sin^2\theta+\sin^4\theta$; substitute $\sin^2\theta=1-\cos^2\theta$: $= \cos^4\theta-6\cos^2\theta(1-\cos^2\theta)+(1-\cos^2\theta)^2 = \cos^4\theta-6\cos^2\theta+6\cos^4\theta+1-2\cos^2\theta+\cos^4\theta = 8\cos^4\theta-8\cos^2\theta+1$ ✓

10. The roots are $1,\omega,\omega^2,\ldots,\omega^{n-1}$ where $\omega = e^{2\pi i/n}$; they are roots of $z^n-1=0$, which factors as $(z-1)(z^{n-1}+z^{n-2}+\cdots+z+1)=0$; for $z\neq1$: $z^{n-1}+\cdots+1=0$, meaning $1+\omega+\omega^2+\cdots+\omega^{n-1}=0$ ✓; alternatively, these are a geometric series with ratio $\omega\neq1$: sum $= \frac{1-\omega^n}{1-\omega} = \frac{1-1}{1-\omega} = 0$ ✓

11. $z+z^{-1}=2\cos\theta$, so $\cos^4\theta = \frac{1}{16}(z+z^{-1})^4 = \frac{1}{16}(z^4+4z^2+6+4z^{-2}+z^{-4}) = \frac{1}{16}((z^4+z^{-4})+4(z^2+z^{-2})+6) = \frac{1}{16}(2\cos4\theta+8\cos2\theta+6)$; so $\cos^4\theta = \frac{1}{8}\cos4\theta+\frac{1}{2}\cos2\theta+\frac{3}{8}$; integral: $\int_0^{\pi/2}\cos^4\theta\,d\theta = \left[\frac{\sin4\theta}{32}+\frac{\sin2\theta}{4}+\frac{3\theta}{8}\right]_0^{\pi/2} = \left(0+0+\frac{3\pi}{16}\right)-(0) =$ **$\dfrac{3\pi}{16}$**

12. Let $z = e^{i\theta} = \cos\theta+i\sin\theta$ (any point on unit circle); $z+1 = (1+\cos\theta)+i\sin\theta$; $z-1 = (\cos\theta-1)+i\sin\theta$; $w = \frac{(1+\cos\theta)+i\sin\theta}{(\cos\theta-1)+i\sin\theta}$; multiply top and bottom by conjugate of denominator $(\cos\theta-1)-i\sin\theta$; numerator: $[(1+\cos\theta)(\cos\theta-1)-\sin^2\theta]+i[-\sin\theta(1+\cos\theta)+\sin\theta(\cos\theta-1)]$; real part: $\cos^2\theta-1-\sin^2\theta = -(1-\cos^2\theta)-\sin^2\theta = -\sin^2\theta-\sin^2\theta = -2\sin^2\theta$... wait, let us use a cleaner approach: note that $1+\cos\theta = 2\cos^2(\theta/2)$ and $\sin\theta = 2\sin(\theta/2)\cos(\theta/2)$ and $\cos\theta-1=-2\sin^2(\theta/2)$; so $w = \frac{2\cos^2(\theta/2)+2i\sin(\theta/2)\cos(\theta/2)}{-2\sin^2(\theta/2)+2i\sin(\theta/2)\cos(\theta/2)} = \frac{2\cos(\theta/2)[\cos(\theta/2)+i\sin(\theta/2)]}{2\sin(\theta/2)[-\sin(\theta/2)+i\cos(\theta/2)]}$; $= \frac{\cos(\theta/2)}{\sin(\theta/2)}\cdot\frac{e^{i\theta/2}}{ie^{i\theta/2}} = \frac{\cot(\theta/2)}{i} = -i\cot(\theta/2)$; since $\cot(\theta/2)$ is real, $w$ is **purely imaginary** ✓

---

### Day 7 Summary

| Concept | Key Takeaway |
|---------|-------------|
| De Moivre's theorem | $(re^{i\theta})^n = r^n e^{in\theta}$ — raise modulus to n, multiply argument by n |
| Speed advantage | De Moivre turns a 50-step FOIL into a 3-line calculation |
| nth roots | n roots, all on a circle of radius $R^{1/n}$, spaced $\frac{2\pi}{n}$ apart |
| Pizza pattern | Roots always form a regular n-gon — elegant and geometric |
| Sum of roots of unity | Always zero — real and imaginary parts cancel perfectly |
| Trig identities | Expand $(\cos\theta+i\sin\theta)^n$, equate real and imaginary parts |
| Applications | AC circuits, quantum mechanics, signal processing, fractals, control systems |
| Fundamental Theorem | Every degree-n polynomial has exactly n roots in $\mathbb{C}$ |
| Big picture | $\mathbb{C}$ is the complete, final number system — nothing more is needed |

---

### Course Completion — The Full 7-Day Journey

Congratulations! Look how far you have travelled:

| Day | Topic | What You Mastered |
|-----|-------|------------------|
| 1 | Introduction | Why i exists; standard form z = a+bi |
| 2 | Addition & Subtraction | Real with real, imaginary with imaginary |
| 3 | Multiplication | FOIL + the i² = −1 transformation |
| 4 | Conjugates & Division | Rationalising with conjugates |
| 5 | Argand Diagram | Modulus, argument, geometry, loci |
| 6 | Polar Form & Euler | $e^{i\theta}=\cos\theta+i\sin\theta$; multiply = rotate+scale |
| 7 | De Moivre & Roots | Powers, nth roots, applications, the big picture |

You began by asking "what is $\sqrt{-1}$?" and ended with a number system that underpins quantum physics, electrical engineering, signal processing, and some of the most beautiful mathematics ever discovered.

The complex numbers were never really "imaginary" — they were always the true and complete picture.

---

> 🌟 **"Mathematics is not about numbers, equations, computations, or algorithms: it is about understanding."**
> — William Paul Thurston

