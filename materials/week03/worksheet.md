# Week 3 Worksheet: AND, OR, or NOT?

Introduction to Computer Engineering (400507-001) · Week 3
Work with a partner. There can be more than one correct answer.

For every scenario, decide which gate (or gates) it needs:

**AND · OR · NOT**

If you are not sure, guess. Then explain your guess in one short
sentence.

---

## Part A (Session 2, in-class, ~15 minutes)

For each scenario, circle the gate(s) that best model it, and fill in
the small truth table.

1. **Turn on the fan = "Room is hot" AND "Fan switch is set to auto."**
   Gate(s): AND / OR / NOT
   | Room hot? | Switch on auto? | Fan on? |
   |---|---|---|
   | No | No | _____ |
   | No | Yes | _____ |
   | Yes | No | _____ |
   | Yes | Yes | _____ |

2. **Door alarm sounds = "Door open" OR "Window open."**
   Gate(s): AND / OR / NOT
   | Door open? | Window open? | Alarm sounds? |
   |---|---|---|
   | No | No | _____ |
   | No | Yes | _____ |
   | Yes | No | _____ |
   | Yes | Yes | _____ |

3. **Screen stays on = NOT "No one is looking at it."**
   Gate(s): AND / OR / NOT
   | No one looking? | Screen stays on? |
   |---|---|
   | Yes | _____ |
   | No | _____ |

4. **Free seat light turns on = "Seat empty" AND "Seatbelt sign is off."**
   Gate(s): AND / OR / NOT
   Why: ______________________________________________

5. **Game controller vibrates = "Hit landed" OR "Low health warning."**
   Gate(s): AND / OR / NOT
   Why: ______________________________________________

**Discuss with your partner:** Pick one scenario above. Name a
different everyday situation that uses the same gate.

______________________________________________

---

## Part B (Session 3, in-class, ~15 minutes)

Same task, harder scenarios. Some need more than one gate. Work with
a partner again (same or new).

1. **Elevator door opens = "Floor reached" AND NOT "Doors already open."**
   Gate(s): AND / OR / NOT
   Why: ______________________________________________

2. **Washing machine starts = "Door closed" AND ("Start button pressed"
   OR "Timer reached zero").**
   Gate(s): AND / OR / NOT
   Why: ______________________________________________

3. **Traffic light turns green = NOT "Pedestrian button pressed"
   AND "Timer done."**
   Gate(s): AND / OR / NOT
   Why: ______________________________________________

4. **Low-fuel warning shows = "Fuel below 10%" AND NOT "Just refueled."**
   Fuel is at 8%, and the car was refueled two minutes ago. Does the
   warning show? Explain in one sentence.
   ______________________________________________

5. **Build your own:** Write one true/false decision from your own
   life (like the umbrella example). Use at least one AND, OR, or NOT.
   ______________________________________________
   ______________________________________________

**Discuss with your partner:** Which scenario in Part B needed more
than one gate? Draw a small chain, like in class, if you have time.

______________________________________________

---

## Part C (Numbers and Text: Hex, Addition, Sign Bit, ASCII)

**Section 1: Hexadecimal.**

1. Convert decimal **44** to hexadecimal. Show your steps (divide by
   16, keep the remainder). Hex: ______________________
2. Convert binary `10110100` to hexadecimal by splitting it into two
   nibbles. Hex: ______________________

**Section 2: Binary addition.** Show each column and any carries.

3. Add `0110` (6) + `0101` (5). Result: ______________________
4. Add `1001` (9) + `0111` (7). Result: ______________________

**Section 3: Sign bit and two's complement.** Show your steps:
positive version, flip every bit, add 1.

5. Represent **−6** in 8-bit two's complement. ______________________
6. A weather app records an overnight change of **−4** degrees.
   Represent −4 in 8-bit two's complement. ______________________

**Section 4: ASCII and Unicode.**

7. The ASCII code for lowercase **'a'** is 97. Convert 97 to binary,
   using the same place-value method from Week 2. ______________________
8. **True or false:** "Unicode was created because ASCII ran out of
   room for the world's languages." Explain in one sentence.
   ______________________________________________

**Discuss with your partner:** Pick one hex value from Section 1.
Name the decimal number and the binary number it stands for, all
three together.

______________________________________________

---

## Part D (Boolean Algebra: Notation, Laws, and Transistors)

**Section 1: Boolean algebra notation.**

1. Write "Cold AND Windy" using Boolean algebra notation (use **C**
   for cold, **W** for windy). ______________________
2. Write "NOT Charging" using Boolean algebra notation (use **G** for
   charging). ______________________
3. Write "Raining OR Snowing" using Boolean algebra notation (use
   **R** for raining, **S** for snowing). ______________________

**Section 2: Laws of Boolean algebra.**

4. The commutative law says A AND B gives the same answer as B AND A.
   Check this using Raining = Yes, Cold = No: does "Raining AND Cold"
   give the same answer as "Cold AND Raining"? ______________________
5. Use De Morgan's law to rewrite **NOT(Sunny AND Warm)** as an OR
   expression. ______________________

**Section 3: From gate to transistor.**

6. A NOT gate uses about 2 transistors. A simple AND gate uses about
   6. Roughly how many transistors would a NOT gate feeding into an
   AND gate use together? ______________________

**Discuss with your partner:** Pick one law (commutative, associative,
or De Morgan's). Explain in one sentence why a chip designer would
find it useful.

______________________________________________
