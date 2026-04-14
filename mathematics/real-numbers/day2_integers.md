## Day 2: Expanding the Line — Integers

---

### Quick recap

Before we dive in, let's make sure Day 1 is solid:

- **Natural Numbers (ℕ)** = { 1, 2, 3, 4, ... } — counting numbers, starting at 1
- **Whole Numbers (𝕎)** = { 0, 1, 2, 3, ... } — natural numbers plus zero
- **ℕ ⊂ 𝕎** — every natural number is also a whole number
- Our number line only went to the **right** of zero. The left side was empty.

Today we fill that left side in.

---

### Let's start with a problem

Imagine these three situations:

1. It's winter. The temperature outside is 3°C. Overnight it drops by 5 degrees. What is the temperature now?
2. You have \$10 in your bank account. You spend \$15. What is your balance?
3. You're in a building. You're on the ground floor — that's floor 0. You take the lift down two floors to the car park. What floor are you on?

Try to answer each one using only the numbers we know so far — Natural Numbers and Whole Numbers.

...

You can't, can you? Our number system simply doesn't have an answer for these situations yet. 3 − 5 is impossible with the numbers we built yesterday. You'd need something *less than zero*.

That's exactly why mathematicians invented a new set.

---

### Meet the Integers

The **Integers** solve this problem by extending the number line in both directions — not just to the right, but to the left of zero as well.

Every time you go left of zero, you get a **negative number**. These are written with a minus sign in front:

> −1, −2, −3, −4, −5, ...

And the full set of Integers looks like this:

$$\mathbb{Z} = \{ \ldots, -4, -3, -2, -1, 0, 1, 2, 3, 4, \ldots \}$$

Notice the three dots on **both** sides this time. The set goes on forever in both directions — infinitely to the left with negatives, and infinitely to the right with positives.

> The symbol **ℤ** comes from the German word *Zahlen*, which simply means "numbers." German mathematicians were among the first to formalise this system, and the name stuck.

---

### The number line, updated

Remember our number line from yesterday? Let's extend it:

```
←──┬────┬────┬────┬────┬────┬────┬────┬────┬────┬──→
  −4   −3   −2   −1    0    1    2    3    4    5
                       ↑
                    still here!
```

Zero is still in the middle. All the natural and whole numbers are still there on the right side — nothing got removed. We simply opened up the left side and filled it with negative numbers.

> **Important:** Integers don't replace the old sets. They *contain* them.

---

### The growing family of sets

Think of it like Russian nesting dolls. Each new set we build is bigger than the last, and it always contains everything from before:

| Set | Members | What's new |
|-----|---------|------------|
| ℕ | 1, 2, 3, ... | The original counting numbers |
| 𝕎 | 0, 1, 2, 3, ... | Added zero |
| ℤ | ..., −2, −1, 0, 1, 2, ... | Added all the negatives |

We write this chain as:

$$\mathbb{N} \subset \mathbb{W} \subset \mathbb{Z}$$

Every natural number is a whole number. Every whole number is an integer. But not every integer is a whole number — because the negatives are new.

---

### Direction vs distance — a crucial idea

Here's something that confuses a lot of students, so let's be very careful.

On the number line, every number has **two pieces of information** baked into it:

- **Direction** — which side of zero are you on? Positive means right. Negative means left.
- **Distance** — how far are you from zero? This is called the **absolute value**.

Look at the numbers 3 and −3 on the number line:

```
←──┬────┬────┬────┬────┬────┬────┬────┬──→
  −4   −3   −2   −1    0    1    2    3
        ↑                             ↑
    3 steps left                 3 steps right
    from zero                    from zero
```

Both −3 and 3 are exactly the same *distance* from zero — 3 steps. But they are in **opposite directions**.

That distance from zero is called the **absolute value**, and we write it with vertical bars:

$$|3| = 3 \quad \text{and} \quad |-3| = 3$$

The absolute value is **always positive** (or zero), because distance can never be negative. You wouldn't say "I walked −5 steps." You walked 5 steps, in a certain direction.

### Practice: absolute values

| Expression | Answer |
|------------|--------|
| \|7\| | 7 |
| \|−7\| | 7 |
| \|0\| | 0 |
| \|−100\| | 100 |
| \|−23\| | 23 |

Same distance, different direction. The absolute value strips away the direction and just tells you how far.

---

### Ordering integers — don't let the negatives fool you

Here's where students often make errors. Look at this question:

> Which is bigger: −3 or −7?

A lot of people instinctively say "−7, because 7 is bigger than 3."

**That is wrong.** Here's why.

Look at the number line. The further **right** you go, the **bigger** the number. The further **left** you go, the **smaller** the number.

```
←──┬────┬────┬────┬────┬────┬────┬────┬──→
  −8   −7   −6   −5   −4   −3   −2   −1
        ↑                   ↑
      smaller             bigger
      (further left)     (further right)
```

−3 is to the **right** of −7 on the number line. So −3 is the bigger number.

Think of it with temperature: if it's −7°C today and warms up to −3°C tomorrow, is it warmer? Yes! So −3 is greater than −7.

$$-3 > -7$$

> **The golden rule:** On the number line, right is always bigger, left is always smaller. This works for every number — positive or negative, no exceptions.

---

### Now go back and solve the problems from the start

Remember those three questions I asked at the beginning? Let's answer them now:

1. **Temperature:** 3°C drops by 5 degrees → 3 − 5 = **−2°C** ✅
2. **Bank account:** $10 − $15 = **−$5** (you are $5 in debt) ✅
3. **Building:** Ground floor is 0, go down 2 floors → **floor −2** ✅

The integers gave us the language to describe all three situations. Before integers, mathematics simply couldn't express "less than nothing." Now it can.

---

### Summary of what we learned

| Concept | Definition / Rule |
|---|---|
| Integers (ℤ) | All whole numbers plus their negatives: {..., −2, −1, 0, 1, 2, ...} |
| Negative numbers | Numbers to the left of zero on the number line |
| Absolute value \|n\| | Distance from zero — always zero or positive |
| Ordering integers | Further right = bigger. Further left = smaller. Always. |
| Subset chain | ℕ ⊂ 𝕎 ⊂ ℤ |

---

### Common mistakes — don't fall for these!

**Mistake 1:** "−7 is bigger than −3 because 7 is bigger than 3."
→ Wrong. On the number line, −3 is to the *right* of −7, so **−3 > −7**.

**Mistake 2:** "Absolute value just removes the minus sign."
→ Mostly true, but the real meaning is *distance from zero*. |0| = 0, not "removing" anything.

**Mistake 3:** "Integers and whole numbers are the same thing."
→ No. Whole numbers are {0, 1, 2, 3, ...}. Integers also include the negatives {..., −3, −2, −1}.

**Mistake 4:** "−5 is a natural number."
→ Negative numbers are **only** integers. They are not whole numbers and not natural numbers.

---

### Try yourself

Try these before checking the answers:

1. What is the absolute value of −9?
2. Which is greater: −1 or −10?
3. Order these from least to greatest: 3, −5, 0, −1, 7, −8
4. Is −6 an integer? Is it a whole number? Is it a natural number?
5. What integer is exactly 4 steps to the left of 2 on the number line?

---

### Answers

| # | Question | Answer |
|---|----------|--------|
| 1 | \|−9\| | **9** |
| 2 | −1 or −10? | **−1** is greater (further right on the number line) |
| 3 | Order: 3, −5, 0, −1, 7, −8 | **−8, −5, −1, 0, 3, 7** |
| 4 | Is −6 an integer / whole / natural? | ✅ Integer only. ❌ Not whole. ❌ Not natural. |
| 5 | 4 steps left of 2 | 2 → 1 → 0 → −1 → **−2** |

---

### Homework

Find **5 real-life uses of negative integers**. For each one, write the number and describe where it sits on a number line.

Try to use **different contexts** — don't use five temperature examples! Some ideas:

- Sport (goal difference, points deductions)
- Elevation (below sea level)
- Finance (debt, overdraft)
- Time zones (behind UTC)
- Floors in a building (basement levels)

---

### Something to think about tonight...

Today we filled in the left side of the number line with whole negative numbers like −1, −2, −3. But look at the number line again:

```
←──┬────┬────┬────┬────┬────┬────┬────┬──→
  −3   −2   −1    0    1    2    3
```

Between 1 and 2, there is a gap. Between 0 and 1, there is a gap. Between −1 and 0, there is a gap. There are numbers living in those gaps that we haven't met yet.

> *What kind of number lives between 0 and 1? Can you think of any?*

