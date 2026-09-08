# Week 3 Handout: Boolean Logic

Introduction to Computer Engineering (400507-001) · Week 3
This handout goes with the Week 3 slides. Keep it for the whole semester.

---

## 1. Glossary: Key Words

Simple, plain definitions. Read these before or after class.

| Word | Plain definition |
|---|---|
| **Boolean value** | A value that can only be true or false. Nothing in between. |
| **Bit** | The smallest piece of data a computer stores: a `1` or a `0`. |
| **True / false** | The two, and only two, Boolean values. |
| **On / off** | The everyday words for `1` and `0` inside a switch. |
| **Gate** | A tiny circuit that takes true/false inputs and gives one true/false answer. |
| **AND gate** | A gate that is true only when **every** input is true. |
| **OR gate** | A gate that is true when **at least one** input is true. |
| **NOT gate** | A gate with one input. It always flips the value: true becomes false. |
| **Truth table** | A table that lists every possible input, and the matching output. |
| **Input** | A true/false value going into a gate. |
| **Output** | The true/false answer a gate gives back. |
| **Circuit** | Two or more gates connected together to make one decision. |
| **Combine** | Connect gates so the output of one feeds into the next. |
| **Hexadecimal (hex)** | A number system using sixteen digits: 0-9, then A-F for ten through fifteen. |
| **Nibble** | 4 binary digits, exactly the amount one hex digit represents. |
| **Binary addition** | Adding binary numbers column by column, carrying exactly like decimal addition does. |
| **Integer representation** | Storing a whole number using a fixed number of bits, commonly 8, 16, 32, or 64. |
| **Sign bit** | The leftmost bit of an integer: 0 for positive, 1 for negative. |
| **Two's complement** | The method of flipping every bit of a positive number, then adding 1, to represent its negative. |
| **ASCII** | A standard assigning every English letter, digit, and common symbol a unique number, stored as one byte. |
| **Unicode** | A much larger character standard, covering characters from nearly every written language. |
| **Boolean algebra** | Writing AND, OR, and NOT as math operations, the same way plus and times are operations in ordinary algebra. |
| **Commutative law** | Order does not matter: A AND B gives the same answer as B AND A (same for OR). |
| **Associative law** | Grouping does not matter: (A AND B) AND C gives the same answer as A AND (B AND C). |
| **De Morgan's law** | NOT(A AND B) equals (NOT A) OR (NOT B), and NOT(A OR B) equals (NOT A) AND (NOT B). |
| **Transistor** | A tiny electronic switch, letting current flow or not, that gates are physically built from. |

---

## 2. Worked Example: The Full Umbrella Decision

This is the full version of the example from class. The slide version
was shortened. Read this at home if you want more detail.

Every morning, you decide: should I bring an umbrella? Your brain
checks a few things at once, and you probably do this in less than a
second. Broken into small true/false steps, it looks like this:

**Step 1 — NOT gate.** Check: "Am I already carrying an umbrella?" If
yes, the NOT gate flips it to false — you do not need another one.
If no, NOT flips it to true — you might still need one.

**Step 2 — OR gate.** Check two things: "Is it raining right now?"
and "Does the forecast say rain later?" If either one is true, the OR
gate outputs true. Only if both are false does it output false.

**Step 3 — AND gate.** Combine Step 1 and Step 2: "Do I need one?"
(from Step 1) AND "Will it rain?" (from Step 2). Only if **both** are
true does the AND gate say: bring the umbrella.

The full rule is:

**Bring umbrella = ("Raining" OR "Forecast says rain later") AND
(NOT "Already carrying one").**

| Raining or forecast rain? | Already carrying one? | Bring umbrella? |
|---|---|---|
| No | No | No |
| No | Yes | No |
| Yes | No | **Yes** |
| Yes | Yes | No |

Notice the last row: even if it will rain, you do not need to bring
one if you are already carrying one. The NOT gate handles that.

### A real chip does the same thing

Inside your laptop, a very similar circuit decides when to show the
low-battery warning:

**Show low-battery warning = "Battery below 20%" AND NOT "Charger
plugged in."**

- Battery at 15%, no charger: both inputs to the AND gate are true.
  **The warning shows.**
- Battery at 15%, charger plugged in: the NOT gate flips "charger
  plugged in" (true) to false. Now the AND gate has one false input.
  **No warning.**

The circuit never "thinks." It just follows the exact same rule,
every single time, thousands of times a second.

---

## 3. Beyond True/False: Numbers, Text, and the Math Behind Gates

Boolean values are not the only thing built on top of bits. This
section covers everything else bits are used to represent, and the
math notation used to write gates on paper.

**A shorthand for long binary numbers: hexadecimal.** A **hexadecimal
(hex)** number system uses sixteen digits: 0-9, then A, B, C, D, E, F
standing for ten through fifteen. Every hex digit maps to exactly 4
binary digits, called a **nibble**, since 2⁴ = 16. To convert decimal
to hex, divide by 16 repeatedly and keep each remainder: 202 ÷ 16 = 12
remainder 10 (the digit A); 12 ÷ 16 = 0 remainder 12 (the digit C);
reading the remainders last to first gives `CA`. To convert binary to
hex, split the bits into nibbles and convert each alone: `11001010`
splits into `1100` (12 = C) and `1010` (10 = A), giving the same `CA`.

**Adding binary numbers.** Binary addition follows one rule per
column: 0+0=0, 1+0=1, 0+1=1, and 1+1=`10` (write 0, carry 1), the
same way 9+1 carries into a new decimal column. Adding `1011` (11) and
`0110` (6) column by column, with carries, gives `10001`, which is 17.

**Storing whole numbers in a fixed width.** An **integer
representation** stores a whole number using a fixed number of bits,
commonly 8, 16, 32, or 64. An 8-bit integer can represent 2⁸ = 256
different values. More bits give a bigger range, but every extra bit
costs more memory.

**Negative numbers: the sign bit and two's complement.** Computers
reserve the leftmost bit of an integer as a **sign bit**: 0 for
positive, 1 for negative. Most systems use **two's complement** so
ordinary addition still works with that sign bit included. The rule:
flip every bit of the positive version, then add 1. Example: to
represent −5 in 8-bit two's complement, start from positive 5
(`00000101`), flip every bit (`11111010`), then add 1 (`11111011`).

**Representing text: ASCII and Unicode.** **ASCII** assigns every
English letter, digit, and common symbol a unique number, stored as
one byte: capital 'A' is 65, lowercase 'a' is 97. ASCII only had room
for 128 characters, far too few for the world's alphabets, so
**Unicode** assigns a unique number to characters from nearly every
written language, plus symbols and emoji, while still keeping 'A' at
its original ASCII number, 65. A chip never "knows" it is storing a
letter; it only stores bits. Binary, decimal, hex, and ASCII are just
different ways humans choose to read the exact same bits.

**Writing logic like math: Boolean algebra.** **Boolean algebra**
writes AND, OR, and NOT as operations, the same way plus and times are
operations in ordinary algebra: AND is often written like
multiplication (**A · B**), OR like addition (**A + B**), and NOT with
a bar over the value (**Ā**). Two basic laws hold: the **commutative
law** says order does not matter (A AND B gives the same answer as B
AND A, and the same for OR), and the **associative law** says grouping
does not matter ((A AND B) AND C gives the same answer as A AND (B AND
C)). **De Morgan's law** lets you flip AND and OR: NOT(A AND B) is the
same as (NOT A) OR (NOT B), and NOT(A OR B) is the same as (NOT A) AND
(NOT B). These laws mean a chip designer can rearrange or regroup
gates for convenience, without ever changing the final answer.

**From gate to transistor.** A **transistor** acts as a tiny
electronic switch, letting current flow (on) or blocking it (off),
controlled by another signal. A single NOT gate can be built from just
one transistor. An AND gate needs several transistors arranged so
current only flows through when every switch along the path is also
on. A modern CPU chip holds billions of transistors, wired into
millions of gates like the ones in this handout.

---

## 4. Optional Reading: More Detail

This section holds extra detail that was trimmed from the slides. It
is optional, but useful if you want to go deeper.

**Where this idea came from.** In 1854, a mathematician named George
Boole published a book called *The Laws of Thought*. He wanted to
write logical reasoning ("if this, then that") using math symbols,
the same way arithmetic uses `+` and `-`. For decades, this stayed a
purely academic idea, with no connection to machines at all.

In 1937, a graduate student named Claude Shannon noticed something
important: Boole's true/false math matches on/off electrical switches
exactly. A switch that is "on" can represent "true." A switch that is
"off" can represent "false." Connecting switches together, the same
way Boole connected true/false statements, builds a working circuit.
This single insight is the foundation of every digital chip made
since.

**Why only two values?** A switch is easy to build and easy to check:
it is clearly on, or clearly off. Real electricity is noisy — voltage
levels drift a little all the time. If a chip tried to use five or
ten different voltage levels to mean five or ten different things, tiny
drifts would cause constant mistakes. Two states, kept far apart, are
almost never confused with each other. That reliability is why every
chip still uses just two values today, even though far more powerful
designs have been tried.

**Who works with logic gates.** Real engineering jobs are built on
exactly this material:

- **Hardware engineer** — designs the physical gates and connections on a chip.
- **Firmware engineer** — writes the lowest-level code, closest to the hardware.
- **Chip designer** — plans how billions of gates fit onto one small chip.
- **Embedded / IoT engineer** — builds small devices that sense and decide, like a smart thermostat.
- **Robotics engineer** — uses gates for fast, simple sensor-based decisions.
- **Test engineer** — checks that every gate matches its truth table exactly, before a chip ships.

**Why this matters in industry.** Hardware and firmware job interviews
often start with a small truth table or a simple logic circuit on a
whiteboard. Interviewers use this because it is a fast way to check
whether a candidate truly understands the material this course covers
in Week 3, not just whether they can use a computer.

---

## 5. Practice Problems (with Answers)

Try each problem yourself before checking the answer.

**Problem 1.** An AND gate has two inputs: true and true. What is the output?

> **Answer:** True. AND needs every input to be true, and both are.

**Problem 2.** An OR gate has two inputs: false and true. What is the output?

> **Answer:** True. OR only needs at least one true input.

**Problem 3.** A NOT gate has one input: false. What is the output?

> **Answer:** True. NOT always flips the value it receives.

**Problem 4.** Write the truth table for: "Turn on porch light = 'It
is dark' AND 'Someone is home.'" List all four rows.

> **Answer:**
> Dark=No, Home=No → No. Dark=No, Home=Yes → No.
> Dark=Yes, Home=No → No. Dark=Yes, Home=Yes → Yes.

**Problem 5.** A smoke detector alarms when: "Smoke detected" OR
"Battery critically low." The battery is fine, but smoke is detected.
Does the alarm sound? Explain in one sentence.

> **Answer:** Yes. OR only needs one true input, and "smoke detected"
> is true here.

**Problem 6.** True or false: "A gate can change its rule depending
on the situation." Explain your answer in one sentence.

> **Answer:** False. A gate always follows the exact same fixed rule,
> every time, no matter what situation it is used in.

**Problem 7.** Convert decimal 15 to hexadecimal.

> **Answer:** `F`. Hex uses A-F for ten through fifteen, so 15 is a
> single digit: F.

**Problem 8.** Represent −2 in 8-bit two's complement. Show your
steps.

> **Answer:** Positive 2 = `00000010`. Flip every bit: `11111101`.
> Add 1: `11111110`. Result: −2 = `11111110`.

**Problem 9.** Use De Morgan's law to rewrite NOT(Hot AND Humid) as
an OR expression.

> **Answer:** (NOT Hot) OR (NOT Humid).
