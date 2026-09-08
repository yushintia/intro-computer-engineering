# Week 2 Handout: Computer History

Introduction to Computer Engineering (400507-001) · Week 2
This handout goes with the Week 2 slides. Keep it for the whole semester.

---

## 1. Glossary: Key Words

Simple, plain definitions. Read these before or after class.

| Word | Plain definition |
|---|---|
| **History** | The story of events, in the order they happened. |
| **Invention** | A new machine or idea, made for the first time. |
| **Generation** | A group of computers built with the same core technology. |
| **Pioneer** | A person who does something new, before anyone else. |
| **Vacuum tube** | An early, glass, light-bulb-like part used to build the first computers. |
| **Transistor** | A small electronic switch. It replaced the vacuum tube in 1947. |
| **Integrated circuit** | A chip that packs many transistors onto one small piece. |
| **Microprocessor** | A whole CPU, built onto a single chip. |
| **Binary** | A number system using only two digits: 0 and 1. |
| **Digit** | A single symbol used to write a number, like 0-9. |
| **Decimal** | The number system we use daily, with ten digits: 0 through 9. |
| **Bit** | One binary digit, either a 0 or a 1. |
| **Byte** | A group of eight bits, used to store one value. |
| **Place value** | How much a digit is worth, based on its position in a number. |
| **Convert** | To change a number from one system to another, like decimal to binary. |
| **Core** | One processing unit inside a modern CPU chip. |
| **Human computer** | Before "computer" meant a machine, a person paid to calculate tables of numbers by hand. |
| **Abacus** | A frame of sliding beads, used to count and calculate by hand, with no gears and no electricity. |
| **Mechanical calculator** | A machine that adds, subtracts, or otherwise calculates using gears and levers, with no electricity. |
| **Pascaline** | The first mechanical adding machine, built by Blaise Pascal in 1642. |
| **Stepped Reckoner** | Gottfried Leibniz's 1673 machine, the first to multiply and divide by repeated addition. |
| **Punch card** | A stiff card with holes in fixed positions, where the hole pattern tells a machine what to do. |
| **Difference Engine** | Babbage's 1822 design to automatically compute mathematical tables. |
| **Analytical Engine** | Babbage's 1837 design meant to run any calculation fed to it on punch cards, with a "store" and a "mill." |
| **Parallel processing** | A chip solving separate parts of a problem at the same time, using more than one processing unit. |
| **General-purpose computer** | A computer built to run many different kinds of programs. |
| **Special-purpose computer** | A computer built to do one specific job, and nothing else. |
| **Digital computer** | A computer that represents data as distinct, separate values, like binary 0s and 1s. |
| **Analog computer** | A computer that represents data as a continuously varying signal. |
| **Hybrid computer** | A computer that mixes digital and analog representation in the same machine. |
| **Supercomputer** | The fastest, most powerful class of computer, used for huge scientific problems. |
| **Mainframe** | A very powerful computer built to serve many users and huge transactions at once. |
| **Minicomputer** | A mid-sized computer, once common for a single department or lab. |
| **Microcomputer** | The smallest class of computer, built around one microprocessor chip. |

---

## 2. The Full Story: From ENIAC to Your Laptop

This is the full version of the timeline from class. The slide version
was shortened. Read this at home if you want more detail.

**Long before any machine had gears, people still needed to calculate
fast.** The **abacus**, a frame of sliding beads, let different
cultures count and calculate by hand, with no gears and no
electricity at all. Each row of beads stands for one place value, the
same idea decimal digits use today.

**Before electronic computers, there were mechanical calculators.** In
1642, Blaise Pascal built the **Pascaline**, the first mechanical
adding machine, to help his father, a tax official, add long columns
of coins and figures correctly. Each digit had its own toothed wheel,
and a small pin automatically carried a digit to the next wheel, an
early physical version of carrying in addition. In 1673, Gottfried
Leibniz built the **Stepped Reckoner**, the first machine that could
multiply and divide, not only add and subtract; it worked by
repeated addition, the same idea a simple CPU still uses today.

**Punch cards taught machines to follow instructions on their own.**
In 1804, Joseph Jacquard used punch cards, stiff cards with holes in
fixed positions, to control weaving looms automatically. In 1890,
Herman Hollerith adapted punch cards to tabulate the U.S. Census,
cutting a count that once took years down to months.

**Charles Babbage tried to combine "calculates on its own" with
"follows any instructions."** In 1822, he designed the Difference
Engine, meant to automatically compute mathematical tables like the
navigation tables ships relied on. In 1837, he designed the far more
ambitious Analytical Engine, a machine that could, in theory, run any
set of instructions fed to it on punch cards. It was never fully
built in his lifetime, but the design was correct, and it introduced a
"store" to hold numbers and a "mill" to process them: the same split
that still separates memory from the CPU today, in Weeks 4 and 5. Ada
Lovelace wrote notes for this machine describing how it could follow
a sequence of steps; many people consider her notes the first
computer program ever written, even though the machine that would run
it did not yet exist.

**World War II created the real, urgent pain.** Armies needed fast,
correct tables for aiming artillery. Before electronic computers,
people called "human computers" calculated these tables by hand. This
was slow, and small mistakes were common and costly. In 1945, ENIAC
(Electronic Numerical Integrator and Computer) was built in the United
States to solve exactly this problem. It used about 17,000 vacuum
tubes, filled a large room, and was among the first general-purpose
electronic computers.

**Five generations followed, each smaller and faster than the last:**

1. **1st generation (1940s):** vacuum tubes. Room-sized, very slow,
   and the tubes often burned out and needed replacing.
2. **2nd generation (1950s):** transistors, invented in 1947. Smaller,
   more reliable, and cabinet-sized instead of room-sized.
3. **3rd generation (1960s):** integrated circuits, invented in 1958.
   Many transistors packed onto one small chip. Desk-sized computers
   became possible.
4. **4th generation (1971 onward):** the microprocessor put a whole
   CPU onto a single chip. The chip inside your own laptop or phone is
   a microprocessor.
5. **5th generation (1980s onward, accelerating in the last decade):**
   AI and parallel processing. A chip solves separate parts of a
   problem at the same time, using more than one processing unit,
   instead of one instruction at a time. This generation is still
   ongoing; many laptops and phones now ship with a chip dedicated to
   AI tasks, running alongside the regular CPU.

Five generations, one direction: smaller, faster, and able to do more
at the exact same instant.

**Along the way, key people shaped how computers work today:**

- **Ada Lovelace** wrote the first computer program, in the 1840s, for
  a machine that had not been built yet.
- **Alan Turing** described, in the 1930s, what any computer could
  ever be able to compute — a foundational idea behind all computing.
- **Grace Hopper** built early tools that turned human-readable code
  into programs a machine could run.
- **John von Neumann** described a computer design, in the 1940s,
  where memory holds both data and instructions together. Most
  computers today, including your laptop, still follow this design.

---

## 3. Why Computers Use Binary

Alongside this history, computers settled on one number system:
**binary**, using only the digits 0 and 1.

- **Decimal** (what people use daily) has ten digits: 0 through 9.
  Each position is worth ten times the position to its right (1, 10,
  100, 1000...).
- **Binary** has only two digits: 0 and 1. Each position is worth
  **double** the position to its right (1, 2, 4, 8, 16, 32, 64, 128...).

To convert a decimal number to binary, check each place value from
biggest to smallest, and ask: "does this fit?"

**Worked example: convert 13 to binary.**

| Place value | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
|---|---|---|---|---|---|---|---|---|
| Fits into 13? | No | No | No | No | Yes | Yes | No | Yes |
| Digit | 0 | 0 | 0 | 0 | 1 | 1 | 0 | 1 |

Steps: 13 is smaller than 128, 64, 32, and 16, so those are all 0.
13 is at least 8, so use it: 13 − 8 = 5 left over.
5 is at least 4, so use it: 5 − 4 = 1 left over.
1 is smaller than 2, so that place is 0.
1 is at least 1, so use it: 1 − 1 = 0 left over.

**Result: 13 in decimal is `00001101` in binary.**

This handout does not yet explain *why* a switch naturally has two
states, on and off — that is next week's topic, Boolean Logic.

---

## 4. Classifying Computers: Three Ways to Sort Any Machine

History gave us machines. Beyond generations, there are three
independent ways to sort *any* computer you meet, today or in the
past.

**By purpose: general vs special.** A **general-purpose computer** is
built to run many different kinds of programs, your laptop, phone,
or a lab desktop: today an essay, tomorrow a game. A **special-purpose
computer** is built to do one specific job and nothing else; a
washing machine's controller, a car's anti-lock brake controller, or a
supermarket barcode scanner. Swap a washing machine's chip into a
laptop, and it could not run a web browser; it was never built to.

**By data representation: digital, analog, or hybrid.** A **digital
computer** represents data as distinct, separate values, like binary
0s and 1s; nearly every computer you meet today, including your
laptop. An **analog computer** represents data as a continuously
varying signal, like a smoothly changing voltage; a classic mercury
thermometer is analog, since the mercury rises smoothly, skipping no
in-between height. A **hybrid computer** mixes both in the same
machine, like a hospital heart monitor, which takes in a continuous
analog heartbeat signal and converts it into digital numbers on
screen.

**By processing capacity: four sizes.** A **supercomputer** is the
fastest, most powerful class, used for huge scientific problems like
weather forecasting. A **mainframe** is very powerful, built to serve
many users and huge transactions at once, like a bank's central
system. A **minicomputer** is mid-sized, once common for a single
department or lab, mostly replaced today by powerful servers. A
**microcomputer** is the smallest class, built around one
microprocessor chip: this is your laptop, phone, or desktop.

**These three schemes are independent.** One device can sit in a
different spot on each scheme at once. A hospital heart monitor, for
example, is special-purpose, hybrid, and microcomputer-sized, all at
the same time: three separate questions, three separate answers, for
the very same machine.

---

## 5. Optional Reading: More Detail

This section holds extra detail that was trimmed from the slides. It
is optional, but useful if you want to go deeper.

**Why "generations" is still a useful word.** Engineers still use the
word "generation" today, even beyond hardware. A "4th-generation"
Intel or AMD processor, for example, refers to one product line's
design era, echoing the same idea: a shared core technology, replaced
every so often by something smaller and faster.

**Museums keep this history alive.** Working replicas and original
parts of ENIAC, early IBM machines, and other historic computers are
on display in computing museums worldwide. Seeing a room-sized
computer next to a modern laptop makes the size difference concrete.

**Why this matters in industry.** Some technical interviews include a
short history or fundamentals question, not to test memorization, but
to check that a candidate understands computing is built on decades of
real engineering trade-offs, not something that appeared overnight.
Understanding *why* computers got smaller and faster also helps
explain *why* certain hardware costs money and other hardware does
not — a very practical, real-world skill.

---

## 6. Practice Problems (with Answers)

Try each problem yourself before checking the answer.

**Problem 1.** Put these four inventions in the correct order, oldest
first: transistor, integrated circuit, vacuum tube, microprocessor.

> **Answer:** Vacuum tube (1940s) → transistor (1947) → integrated
> circuit (1958) → microprocessor (1971).

**Problem 2.** Convert the decimal number 10 to binary. Show your
place-value steps.

> **Answer:** 10 is at least 8 (10 − 8 = 2), less than 4, at least 2
> (2 − 2 = 0), less than 1. Result: `00001010`.

**Problem 3.** Why was ENIAC built? Answer in one or two sentences.

> **Answer:** Armies in World War II needed fast, correct artillery
> calculations. Human calculation by hand was too slow and error-prone.

**Problem 4.** True or false: "Binary digits can appear in any order,
since they are just symbols." Explain your answer in one sentence.

> **Answer:** False. Each position has a fixed, doubling value (1, 2,
> 4, 8...), so the order of digits changes the number's value.

**Problem 5.** Name one person from this week's history, and one
thing they are known for.

> **Answer (sample):** Ada Lovelace — wrote the first computer program.
> Any of Turing, Hopper, or von Neumann with a matching fact is also
> correct.

**Problem 6.** A friend says: "My phone is much newer, so it must use
a totally different number system than old computers did." Is this
true? Explain in one or two sentences.

> **Answer:** False. Both old and new computers use the same binary
> number system underneath; only the physical technology changed.

**Problem 7.** A friend says: "Generations stopped at the
microprocessor. Nothing has changed since 1971." Explain in one or
two sentences why this is wrong.

> **Answer:** False. A 5th generation exists too: AI and parallel
> processing, where a chip solves separate parts of a problem at the
> same time using more than one processing unit.

**Problem 8.** A hospital heart monitor takes in a continuous
heartbeat signal and converts it into digital numbers on screen. By
data representation, is it digital, analog, or hybrid? Explain in one
sentence.

> **Answer:** Hybrid. It mixes an analog input signal with a digital
> display in the same machine.