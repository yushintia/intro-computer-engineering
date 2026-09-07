---
marp: true
theme: shintia
paginate: true
footer: 'Department of Intelligent Computing'
---

<!-- SLOT 1: Title -->
<!-- _class: title -->

# Week 4: CPU & Instructions

<span class="subtitle">Introduction to Computer Engineering (400507-001)</span>

<div class="meta">
Yushintia Pramitarini, Ph.D · Dept. of Intelligent Computing · Thu [1-3] · Seongpa Hall 701
</div>

<!--
notes: Ask everyone to look at their laptop or phone again. Ask: "Last
week, we found gates that answer true or false. Today, who tells the
gates what to do, and in what order?" Wait for guesses.
-->

---

<!-- SLOT 2: Where we are (Act 0 / LOCATE) -->

# Where We Are

<div class="roadmap">
<div class="wk"><div class="n">Wk 1</div><div class="t">Introduction</div></div>
<div class="wk"><div class="n">Wk 2</div><div class="t">Computer History</div></div>
<div class="wk"><div class="n">Wk 3</div><div class="t">Boolean Logic</div></div>
<div class="wk now"><div class="n">Wk 4</div><div class="t">CPU &amp; Instructions</div></div>
<div class="wk"><div class="n">Wk 5</div><div class="t">Memory &amp; Storage</div></div>
<div class="wk"><div class="n">Wk 6</div><div class="t">Application Software · Quiz 1</div></div>
<div class="wk"><div class="n">Wk 7</div><div class="t">Operating Systems</div></div>
<div class="wk review"><div class="n">Wk 8</div><div class="t">Midterm Exam</div></div>
<div class="wk"><div class="n">Wk 9</div><div class="t">Computer &amp; Internet</div></div>
<div class="wk"><div class="n">Wk 10</div><div class="t">Programming Language</div></div>
<div class="wk"><div class="n">Wk 11</div><div class="t">Databases &amp; Security</div></div>
<div class="wk"><div class="n">Wk 12</div><div class="t">Computer Applications</div></div>
<div class="wk"><div class="n">Wk 13</div><div class="t">AI · Quiz 2</div></div>
<div class="wk"><div class="n">Wk 14</div><div class="t">Emerging Technologies</div></div>
<div class="wk review"><div class="n">Wk 15</div><div class="t">Final Exam</div></div>
</div>

<!-- notes: Point at the map. Say: "Two weeks ago, the whole layered picture. Last week, one layer: gates. Today, we zoom into the CPU layer." -->

---

<!-- SLOT 3: Recap + open wound (Act 0 / LOCATE) -->

# Last Week, This Week

- **Last week delivered:** logic gates that decide true or false, built from simple on-off switches.
- **Last week left broken:** gates can decide true or false, but not yet follow a sequence of steps, a program.

---

<!-- SLOT 4: The pain (Act 1 / MOTIVATE), ZERO jargon -->

# The Silent Chip

<div class="pain">

Last week, you learned that gates can decide true or false.

But gates alone cannot yet follow a sequence of steps, a program.

Your laptop has millions of these gates, inside one chip.

You open a calculator app. You type 2 + 3. You press enter.

The chip can answer yes-or-no questions. But right now, nothing happens.

Who tells all these gates what to do, and in what order?

</div>

<!-- notes: Ask: "Any guesses? What is missing?" Let two or three students answer. Do not explain the answer yet. -->

---

<!-- SLOT 5: Cost of not knowing (Act 1 / MOTIVATE) -->

# What This Actually Costs

- Gates alone cannot run any real app, not even a simple calculator.
- Every program needs a clear, exact order of steps to work.
- A wrong order gives a wrong answer, or no answer at all.
- Games, browsers, and camera apps all depend on this order.

<div class="why">
<strong>In industry:</strong> "Explain how a CPU runs one instruction" is
a common interview question for hardware and firmware jobs. It checks
if you understand the whole chip, not just one part.
</div>

---

<!-- SLOT 6: Driving question (Act 1 / MOTIVATE) -->

<!-- _class: section -->

# This Week's Question

<div class="driving-q">"How does a chip run a program, one step at a time, in the right order?"</div>

---

<!-- SLOT 7: Learning outcomes (Act 1 / MOTIVATE) -->

# By the End of This Week, You Can

<div class="cardlist">
<div class="card"><div class="h">What a CPU Does</div><div class="d">Explain what a CPU does, in plain words.</div></div>
<div class="card"><div class="h">Fetch-Decode-Execute</div><div class="d">Describe the fetch-decode-execute cycle, step by step.</div></div>
<div class="card"><div class="h">CPU Parts</div><div class="d">Name the three main parts inside a CPU.</div></div>
<div class="card"><div class="h">Tracing Instructions</div><div class="d">Trace one instruction through your laptop's CPU.</div></div>
</div>

---

<!-- Key Words, Session 1 -->

# Key Words Today

- **Chip** — a small hardware part with millions of tiny switches inside.
- **Switch** — a simple part that is either on or off.
- **Program** — a list of steps for a computer to follow.
- **Step** — one single action in a list.
- **Order** — the correct sequence to do steps in.

<!-- notes: Read each word aloud. Ask students to repeat it once. Say: "Keep these words. We will build on them all class." -->

---

<!-- Key Words, Session 2 -->

# Key Words Today

- **CPU** — the chip that runs a program, one instruction at a time.
- **Instruction** — one exact command the CPU can carry out.
- **Fetch** — the CPU step that gets the next instruction.
- **Decode** — the CPU step that figures out what the instruction means.
- **Execute** — the CPU step that actually does the action.

<!-- notes: Read each word aloud. Say: "These five words are today's whole lesson. We will use every one of them." -->

---

<!-- SLOT 8: Origin (Act 2 / GROUND) -->

# Where This Idea Came From

<div class="thread">You just felt the pain. Where did this idea come from?</div>

- **1940s:** early computers were wired by hand, for one task only.
- Changing the task meant days of rewiring, by hand, with real wires.
- **1945:** mathematician John von Neumann wrote down a simpler idea.
- Store the program as data. Let the machine step through it alone.

<div class="why">
This idea is why your laptop can run many programs. Nobody rewires
the chip for each one.
</div>

---

<!-- SLOT 9: Core concept (Act 2 / GROUND) -->

# CPU: Definition

<div class="thread">One field-defining idea, one clear definition.</div>

> A **CPU** (central processing unit) is a chip that reads
> **instructions**, one at a time, and carries each one out.

- **Instruction:** one exact command, like "add these two numbers."
- **Program:** a full list of instructions, in the right order.

A CPU cannot think. It only follows instructions, exactly as written.

---

<!-- Act 3 / BUILD -->

# The Whole Computer System: CPU, Memory, and I/O

<div class="thread">The CPU never works alone. Zoom out to the whole machine around it.</div>

> A **computer system** is built from three basic parts working together: the **CPU** (processes instructions), **memory** (holds data and instructions temporarily), and **I/O** (input/output — how the machine talks to the outside world, like a keyboard or screen).

- Memory holds the program and data close by, ready for the CPU to fetch.
- I/O devices, like a keyboard, mouse, or screen, are how you and the CPU exchange information at all.

**Worked example:** when you type "2" on your calculator app, the keyboard (I/O) sends that keystroke in, memory holds it briefly, and the CPU reads it during its next fetch step.

---

# The Bus: How Parts Talk to Each Other

<div class="thread">CPU, memory, and I/O sit in different places on the same chip and board. How do they actually reach each other?</div>

> A **bus** is a shared set of wires connecting the CPU, memory, and I/O devices, letting them send data back and forth.

- Think of a bus like a shared hallway: every part uses the same hallway to pass information along.
- Without a bus, the CPU, memory, and keyboard would have no physical way to reach each other at all.

**Worked example:** fetching an instruction means the CPU sends a memory address out on the bus, and memory sends the instruction's bits back across that same bus.

---

# Types of Buses: Address, Data, and Control

<div class="thread">Not everything traveling on the bus carries the same kind of information.</div>

- **Address bus:** carries the memory location the CPU wants to read or write.
- **Data bus:** carries the actual bits being read or written.
- **Control bus:** carries signals like "read" or "write," telling the other parts what kind of action this is.

**Worked example:** to fetch the instruction stored at memory address 100, the CPU puts `100` on the address bus, sets the control bus to "read," and memory replies by putting the instruction's bits on the data bus.

This three-way split shows up in nearly every real hardware diagram, from a phone to a supercomputer.

---

# Worked Example: Tracing One Keystroke Across the Bus

<div class="thread">One full trip, start to finish, using every part from this section.</div>

1. The keyboard (I/O) detects the "5" key press.
2. The keystroke's data travels across the bus into memory.
3. During its next fetch step, the CPU reads that data from memory, across the bus.
4. The ALU processes it, and the result eventually travels back across the bus to the screen (I/O).

Every single character you type takes this same bus trip, every time.

---

# Real Instructions Are Simple

<div class="thread">One instruction, one tiny job. Never more.</div>

<div class="chip-row">
<span class="chip">Load a number</span>
<span class="chip">Add two numbers</span>
<span class="chip">Store a result</span>
<span class="chip">Compare two values</span>
<span class="chip">Show something on screen</span>
</div>

A program is just hundreds, or millions, of instructions like these.
Each one alone looks almost too simple to matter.

---

# From Program to Instructions

<div class="thread">You do not write instructions like this yourself, not yet.</div>

- A programmer writes code in a programming language, like Python.
- A translator program turns that code into simple instructions.
- The CPU only ever sees the simple instructions, never the code.

<div class="why">
You will write real code starting in Week 10. Today, you only need
to know what the CPU receives at the very end.
</div>

---

<!-- SLOT 10: Mechanics -->

# The Fetch-Decode-Execute Cycle

<div class="thread">Three steps, repeated over and over.</div>

<div class="pipeline">
<div class="stage"><div class="h">Fetch</div><div class="s">Get the next instruction from memory.</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Decode</div><div class="s">Figure out what the instruction means.</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Execute</div><div class="s">Do the action. Then fetch the next one.</div></div>
</div>

The CPU repeats this cycle, without stopping, until the program ends.

<!-- notes: Trace the cycle with your hands, pointing left to right. Say: "Fetch, decode, execute. Then back to fetch. Again and again." -->

---

# What Happens at Each Step (1/2)

<div class="thread">The cycle again, this time in more detail.</div>

**Step 1: Fetch.**
The control unit finds the next instruction. It waits close by,
ready to be read.

**Step 2: Decode.**
The control unit reads the instruction. It figures out the job:
add, compare, load, or something else.

---

# What Happens at Each Step (2/2)

**Step 3: Execute.**
The right part does the job. The ALU may do math. A register may
hold a value.

**Step 4: Repeat.**
The CPU fetches the very next instruction. The whole cycle starts
again, right away.

<!-- notes: Ask: "What happens if the CPU skips step 4?" (Answer: the program would only ever run one instruction.) -->

---

<!-- SLOT 11: Mechanics -->

# Try It: Worksheet Part A

<div class="thread">Now you practice. Work with a partner.</div>

- Open **[Worksheet Part A](materials/week04/worksheet.html)**.
- Put mixed-up cycle steps back into the right order.
- You have about 15 minutes. Ask your partner before you ask me.

<!-- notes: Hand out Worksheet Part A. Walk around and help pairs. After 15 minutes, ask 2-3 pairs to share their order. -->

---

<!-- Key Words, Session 3 -->

# Key Words Today

- **Register** — a tiny, very fast storage spot inside the CPU.
- **ALU** — the CPU part that does math and comparisons.
- **Control unit** — the CPU part that directs each step of the cycle.
- **Clock** — a fast, steady beat that times each CPU step.
- **Cycle** — one full round of fetch, decode, and execute.

<!-- notes: Read each word aloud. Say: "You will see all five words again in the next two slides." -->

---

<!-- SLOT 12: Mechanics -->

# What Is Inside a CPU?

<div class="thread">Three parts, working together, every single step.</div>

<div class="appgrid">
<div class="app"><div class="name">Control unit</div><div class="desc">Directs each step. Tells the other parts what to do next.</div></div>
<div class="app"><div class="name">ALU</div><div class="desc">Does math and comparisons: adds, subtracts, checks true or false.</div></div>
<div class="app"><div class="name">Registers</div><div class="desc">Hold the data the CPU is using right now, very fast.</div></div>
</div>

These three parts repeat the fetch-decode-execute cycle, again and again.

---

# The Control Unit: The CPU's Traffic Director

<div class="thread">You just met all three parts as one grid. Each deserves its own definition.</div>

> The **control unit** is the CPU part that reads each instruction and signals every other part what to do next, without doing any math itself.

- It does not calculate. It only directs: "ALU, add these two values now," or "register, hold this result."

**Worked example:** for the instruction "add 2 and 3," the control unit does not compute 5. It tells the ALU to compute 5, then tells a register to store it.

---

# The ALU: Where Math and Comparisons Happen

<div class="thread">The control unit gives the order. This part actually does the work.</div>

> The **ALU (arithmetic logic unit)** is the CPU part that performs math, like addition, and comparisons, like checking whether one value is bigger than another.

- "Arithmetic" covers add, subtract, multiply, divide.
- "Logic" covers true/false comparisons, built from the very gates you learned last week.

**Worked example:** given the instruction "add 2 and 3," the ALU is the only part that actually computes 2 + 3 = 5.

---

# Registers: The CPU's Scratch Pad

<div class="thread">The ALU needs somewhere to read its inputs from, and write its answer to.</div>

> A **register** is a tiny, extremely fast storage spot inside the CPU, holding one value the CPU is actively working with right now.

- Registers hold far less than memory, but are read and written far faster.
- A CPU has only a handful of registers, each with its own short name, like R1 or R2.

**Worked example:** before adding 2 and 3, the CPU first loads 2 into register R1 and 3 into register R2. The ALU then reads both registers to compute the sum.

---

# Worked Example: Naming Every Register in One Instruction

<div class="thread">Put a name and a value on every register in one single instruction.</div>

**Instruction: `ADD R1, R2`**

| Register | Holds |
|---|---|
| R1 | 2 |
| R2 | 3 |
| Result register | 5, once execute finishes |

Meanwhile, a separate, special register is already pointing at the next instruction, whether or not it is part of this add. The next few slides meet that register directly.

---

<!-- SLOT 13: Mechanics -->

# Why So Fast?

<div class="thread">One cycle is quick. Millions of them are instant.</div>

<div class="barchart">
<div class="bar-row">
  <div class="bar-label">You, reading one word</div>
  <div class="bar-track"><div class="bar-fill short" style="width: 5%"></div></div>
  <div class="bar-value">about 1 word per second</div>
</div>
<div class="bar-row">
  <div class="bar-label">A laptop CPU</div>
  <div class="bar-track"><div class="bar-fill long" style="width: 100%"></div></div>
  <div class="bar-value">billions of cycles per second</div>
</div>
</div>

Check your laptop's spec sheet. "3 GHz" means 3 billion cycles a second.

---

# More Than One Core

<div class="thread">One CPU chip can hold more than one CPU.</div>

- Many laptops have 4, 8, or more **cores** inside one chip.
- Each core is its own small CPU. It runs its own cycle.
- More cores let a laptop run more programs smoothly, at once.

Your laptop's spec sheet may say "8-core CPU." Now you know what that means.

---

# Meet the Program Counter: Tracking Which Instruction Is Next

<div class="thread">One more register deserves its own name before the full worked example.</div>

> The **program counter (PC)** is a special register that always holds the memory address of the next instruction to fetch.

- After each fetch, the PC automatically moves forward to the next address, ready for the next cycle.

**Worked example:** if the current instruction sits at memory address 100, the PC already holds 100. The moment fetch finishes, the PC updates to 101, pointing at the next instruction in line.

---

# Full Worked Example: Tracing ADD R1, R2 (Fetch)

<div class="thread">Real memory address, real registers, real values. One instruction, traced completely.</div>

**Setup:** memory address 100 holds the instruction `ADD R1, R2`. Registers already hold R1 = 2, R2 = 3, loaded by earlier instructions. PC = 100.

1. **Fetch:** the PC holds 100. The CPU sends 100 out on the address bus; memory returns `ADD R1, R2` on the data bus.
2. The PC updates to 101, ready for whatever instruction comes right after this one.

| Part | Value after fetch |
|---|---|
| PC | 101 |
| Instruction register | `ADD R1, R2` |
| R1 | 2 |
| R2 | 3 |

---

# Full Worked Example: Tracing ADD R1, R2 (Decode & Execute)

<div class="thread">Same instruction, same registers, the next two steps.</div>

3. **Decode:** the control unit reads `ADD R1, R2` sitting in the instruction register, and recognizes: this is an ADD, using R1 and R2.
4. **Execute:** the control unit tells the ALU to add R1 (2) and R2 (3). The ALU computes 2 + 3 = 5, and the result is written into a result register.

| Part | Final value |
|---|---|
| PC | 101 |
| R1 | 2 |
| R2 | 3 |
| Result register | 5 |

Every value in this table is real: two registers, one memory address, one result. This is Week 4's driving question, now with actual numbers attached.

---

<!-- SLOT N-2: Worked example -->

# Case Study: Running the Calculator (1/2)

<div class="thread">Back to the frozen calculator. Now you have the words.</div>

You type 2 + 3 and press enter. The CPU repeats its cycle:

1. **Fetch:** the CPU gets the next instruction: "add these two numbers."
2. **Decode:** the control unit figures out this is a math step.

---

# Case Study: Running the Calculator (2/2)

3. **Execute:** the ALU adds 2 and 3. The answer, 5, goes into a register.
4. **Fetch again:** the next instruction says "show this answer."
5. **Decode, then execute:** the screen shows 5.

This whole cycle takes a tiny fraction of one second.

<!-- notes: Ask: "How many cycles did this take?" (At least two full cycles: one to add, one to show the result.) -->

---

# Case Study: A Decision, Not Just Math

<div class="thread">Instructions are not only math. They can also decide.</div>

Your calculator app checks: "is the answer bigger than 999?"

1. **Fetch:** the CPU gets a compare instruction.
2. **Decode:** the control unit sees this is a true-or-false question.
3. **Execute:** the ALU compares the two numbers, using a gate, from last week, to decide true or false.

This is why last week's gates still matter, inside this week's ALU.

---

# Careers Built on the CPU

<div class="thread">This one chip creates entire careers.</div>

<div class="appgrid">
<div class="app"><div class="name">Computer architect</div><div class="desc">Designs how the CPU's parts fit and work together.</div></div>
<div class="app"><div class="name">Firmware engineer</div><div class="desc">Writes the lowest-level instructions a device runs first.</div></div>
<div class="app"><div class="name">Embedded engineer</div><div class="desc">Builds small CPUs inside cars, watches, and appliances.</div></div>
</div>

Every one of these jobs starts with the fetch-decode-execute cycle.

---

# Clock Speed: What Gigahertz Actually Means

<div class="thread">You saw the bar chart earlier. Here is exactly what the number means.</div>

> **Clock speed** is how many cycles a CPU can complete in one second, measured in **hertz** (cycles per second). "Giga" means billion, so 1 GHz means 1 billion cycles per second.

**Worked example:** a 3 GHz CPU completes 3,000,000,000 cycles every single second — three billion complete fetch-decode-execute rounds, if every instruction took exactly one cycle.

---

# Worked Example: How Long Is One Clock Cycle?

<div class="thread">Flip the last slide's number around: how long does just one cycle take?</div>

- One second ÷ 3,000,000,000 cycles ≈ **0.33 nanoseconds per cycle.**
- A single human blink takes roughly 300 milliseconds, or 0.3 seconds.

**Result:** in the time it takes you to blink once, a 3 GHz CPU could complete roughly 900 million cycles (0.3 × 3,000,000,000).

---

# Instruction Throughput: Why More GHz Isn't the Whole Story

<div class="thread">Clock speed counts cycles. It does not always count finished instructions the same way.</div>

> **Instruction throughput** is how many actual instructions a CPU finishes per second. It is not quite the same as clock speed, because some instructions take more than one cycle to finish.

- A simple instruction like "add" might finish in one cycle. A more complex one, like "divide," might need several cycles chained together.
- Two CPUs with the exact same GHz can still finish a different number of instructions per second, depending on how many cycles each instruction needs.

**Worked example:** if "add" takes 1 cycle but "divide" takes 4 cycles, a program full of divides finishes far fewer instructions per second than a program full of adds, even on the exact same chip.

---

# Worked Example: Comparing Two Laptops by Clock Speed

<div class="thread">Back to your own laptop, one more time, next to a second machine.</div>

- **Laptop A:** 2.4 GHz.
- **Laptop B:** 3.6 GHz.
- Both run the exact same calculator app.

**Result:** Laptop B completes about 1.5 times as many cycles per second as Laptop A (3.6 ÷ 2.4 = 1.5). Running the exact same program, Laptop B likely finishes first — "likely," not "always," since instruction throughput can still differ underneath the same GHz number.

---

# Pipelining: Overlapping the Three Steps

<div class="thread">One more idea hiding inside "why so fast": the CPU rarely waits for one instruction to fully finish before starting the next.</div>

> **Pipelining** means a CPU starts fetching the next instruction before the current instruction has finished executing, overlapping the three steps across several instructions at once.

- Without pipelining, the CPU finishes fetch, decode, and execute completely before starting the next instruction's fetch.
- With pipelining, while instruction 1 executes, instruction 2 can already be decoding, and instruction 3 can already be fetching.

**Worked example:** like a laundry line — while one load dries, a second load can already be washing, and a third can already be loading in, instead of finishing one load completely before touching the next.

---

# Worked Example: Three Instructions, Pipelined

<div class="thread">The laundry-line idea, with real time steps.</div>

| Time step | Instruction 1 | Instruction 2 | Instruction 3 |
|---|---|---|---|
| 1 | Fetch | | |
| 2 | Decode | Fetch | |
| 3 | Execute | Decode | Fetch |
| 4 | | Execute | Decode |
| 5 | | | Execute |

Without pipelining, these same three instructions would take 9 separate steps, one after another. Pipelining finishes them in 5.

---

# Why Pipelining Still Has Limits

<div class="thread">Pipelining is not free. Sometimes it has to pause.</div>

- Sometimes one instruction needs the exact result of the instruction right before it, before it can even start. Pipelining then has to pause and wait, losing some of its speed advantage.
- A wrong guess about which instruction comes next, common around decisions, can force the CPU to throw away already-started work.

**Worked example:** if instruction 2 needs the exact result instruction 1 is still computing, instruction 2's execute step must wait, even though its fetch and decode already finished early.

---

# Why Simple CPUs Run One Instruction at a Time

<div class="thread">Pipelining overlaps steps. It still does not mean two full programs run at once.</div>

> A **single-core CPU** completes each instruction's cycle, pipelined overlap included, using only one set of CPU parts: one control unit, one ALU, one set of registers.

- Even with pipelining, a single core is still fundamentally moving through one program's instructions, in order.
- Running two unrelated programs at once, on one core, means rapidly switching between them, not truly doing both at the exact same instant.

**Worked example:** your calculator app and a music player can look like they run at the same time on a single core, but the CPU is actually rapidly switching back and forth, finishing tiny slices of each in turn.

---

# Worked Example: One Core vs. Many, Same Workload

<div class="thread">Back to "More Than One Core," now with an actual task.</div>

**Task: calculate 4 separate spreadsheet columns.**

- **One core:** finishes column 1 completely, then column 2, then column 3, then column 4 — one at a time.
- **Four cores:** each core takes one column, and all four finish at roughly the same time.

This is exactly why your laptop's spec sheet advertises its core count, right alongside its GHz.

---

# Teaser: What Happens When One Isn't Enough

<div class="thread">One last look ahead, before this week's limits.</div>

- Modern chips increasingly lean on multiple cores, and specialized chips like AI accelerators, rather than only raw clock speed increases.
- Even with many cores working in parallel, every single core still depends on somewhere to keep its results once the work is done.

Running many instructions at once is one open question this course revisits later. Keeping any of those results afterward is the very next one.

---

# Inside the CPU: A Cheat Sheet

<div class="thread">Before common mistakes, one more look at everything Act 3 covered.</div>

<div class="chip-row">
<span class="chip">Bus: shared wires between parts</span>
<span class="chip">Control unit: directs the steps</span>
<span class="chip">ALU: does the math</span>
<span class="chip">Registers: fast scratch storage</span>
<span class="chip">PC: points at the next instruction</span>
<span class="chip">Pipelining: overlaps fetch/decode/execute</span>
<span class="chip">Clock speed: cycles per second</span>
<span class="chip">Cores: run in parallel</span>
</div>

---

<!-- SLOT N-1: Common mistakes -->

# Common Mistakes

- **"The CPU understands math":** wrong. It only follows exact steps.
- **"One instruction does everything":** wrong. Even 2 + 3 takes several small steps.
- **"A faster CPU always fixes a slow app":** wrong. A slow app can also be a software problem, not a CPU problem.

---

<!-- Try-It hand-off, Worksheet Part B -->

# Try It: Worksheet Part B

<div class="thread">More practice. New scenarios.</div>

- Open **[Worksheet Part B](materials/week04/worksheet.html)**.
- Trace one instruction through fetch, decode, and execute.
- You have about 15 minutes. Then we discuss answers together.

<!-- notes: Hand out Worksheet Part B. After 15 minutes, go through the answer key as a class. Ask for volunteers first. -->

---

<!-- SLOT N: Check yourself -->

# Check Yourself

1. Name the three steps in the CPU's repeating cycle.
2. Which CPU part does math and comparisons?
3. Your calculator app shows the wrong answer. Name one part that could explain why.

---

# Answers

1. Fetch, decode, execute.
2. The **ALU** (arithmetic logic unit).
3. Any one: the ALU did the math step wrong, or the app gave the CPU the wrong instruction.

---

<!-- Self-check quiz hand-off -->

# Self-Check Quiz

<div class="thread">One more check, on your own.</div>

- Take the **[Week 4 Quiz](materials/week04/quiz.html)** (5-8 short questions).
- This quiz is not graded. It just checks your understanding.
- About 10 minutes. Check your own answers at the end.

<!-- notes: Hand out the quiz. Give students 10 minutes. Then read the answer key aloud, or let students self-check. -->

---

<!-- SLOT N+1: Limits (Act 4 / CLOSE), becomes next week's slot 4 -->

# What the CPU Cannot Do

<div class="limits">
The CPU executes instructions perfectly, every single time. But once
an instruction finishes, where does the answer go? The CPU has
nowhere permanent to keep anything. When the laptop loses power,
everything inside the CPU disappears.
</div>

---

<!-- SLOT N+2: Bridge (Act 4 / CLOSE) -->

# Next Week

Week 4 leaves **a permanent place to keep data** unsolved. **Week 5,
Memory & Storage**, addresses it: how a laptop remembers, even after
the power goes off.

---

<!-- SLOT N+3: Summary (Act 4 / CLOSE) -->

# Summary

- A CPU repeats one cycle: fetch, decode, execute.
- Three parts work together: control unit, ALU, and registers.
- Every app you open is really just a long list of instructions.
- **Reading:** Harris & Harris, Chapter 4 (plain overview sections only).
- **Handout:** [materials/week04/handout.md](materials/week04/handout.html), glossary and the full worked example
- **Prepare:** think about what happens to your work when your laptop shuts down. Bring it to Week 5.

---

<!-- SLOT N+4: Thank You (Act 4 / CLOSE) -->

<!-- _class: end -->

# Thank You
