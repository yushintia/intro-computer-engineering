# Week 4 Handout: CPU & Instructions

Introduction to Computer Engineering (400507-001) · Week 4
This handout goes with the Week 4 slides. Keep it for the whole semester.

---

## 1. Glossary: Key Words

Simple, plain definitions. Read these before or after class.

| Word | Plain definition |
|---|---|
| **Chip** | A small hardware part with millions of tiny switches inside. |
| **Switch** | A simple part that is either on or off. |
| **Program** | A list of steps for a computer to follow. |
| **Step** | One single action in a list. |
| **Order** | The correct sequence to do steps in. |
| **CPU** | The chip that runs a program, one instruction at a time. |
| **Instruction** | One exact command the CPU can carry out. |
| **Fetch** | The CPU step that gets the next instruction. |
| **Decode** | The CPU step that figures out what the instruction means. |
| **Execute** | The CPU step that actually does the action. |
| **Register** | A tiny, very fast storage spot inside the CPU. |
| **ALU** | The CPU part that does math and comparisons. |
| **Control unit** | The CPU part that directs each step of the cycle. |
| **Clock** | A fast, steady beat that times each CPU step. |
| **Cycle** | One full round of fetch, decode, and execute. |
| **Core** | One small CPU inside a bigger chip. Many laptops have several. |
| **Computer system** | The CPU, memory, and I/O working together as three basic parts. |
| **I/O (input/output)** | How a machine talks to the outside world, like a keyboard, mouse, or screen. |
| **Bus** | A shared set of wires connecting the CPU, memory, and I/O devices. |
| **Address bus** | The bus that carries the memory location the CPU wants to read or write. |
| **Data bus** | The bus that carries the actual bits being read or written. |
| **Control bus** | The bus that carries signals like "read" or "write." |
| **Program counter (PC)** | A special register that always holds the memory address of the next instruction to fetch. |
| **Clock speed** | How many cycles a CPU can complete in one second, measured in hertz. |
| **Instruction throughput** | How many actual instructions a CPU finishes per second; not quite the same as clock speed. |
| **Pipelining** | Starting the next instruction's fetch before the current instruction has finished executing, overlapping the steps. |
| **Hazard** | A case where one instruction needs the exact result of the instruction right before it, forcing pipelining to pause. |
| **Single-core CPU** | A CPU with only one control unit, one ALU, and one set of registers. |
| **Multi-core CPU** | A CPU chip holding more than one core, each running its own cycle. |

---

## 2. The Calculator, Step by Step

This is the full version of the case study from class. The slide
version was shortened. Read this at home if you want more detail.

You open a calculator app on your laptop. You type 2 + 3. You press
enter. What actually happens, inside the chip, in that split second?

The CPU does not "know" math. It only follows exact instructions, one
at a time, using a repeating cycle: **fetch, decode, execute.**

**Cycle 1: Adding the numbers.**

1. **Fetch.** The control unit finds the next instruction. It says:
   "add these two numbers." The instruction waits close by, ready to
   be read.
2. **Decode.** The control unit reads the instruction. It figures out
   the job: this is a math step, not a compare or a load.
3. **Execute.** The ALU adds 2 and 3. The answer, 5, goes into a
   register, a tiny fast storage spot inside the CPU.

**Cycle 2: Showing the answer.**

4. **Fetch.** The CPU gets the next instruction: "show this answer on
   the screen."
5. **Decode.** The control unit sees this is a display step, not a
   math step.
6. **Execute.** The screen shows 5.

Two full cycles happened here: one to add, one to show the result.
Real apps use many more cycles than this, often millions, for even a
simple task.

**A third cycle: making a decision.**

Your calculator app also checks: "is the answer bigger than 999?"
This uses the same three steps, but the job is different:

7. **Fetch.** The CPU gets a compare instruction.
8. **Decode.** The control unit sees this is a true-or-false question,
   not a math step.
9. **Execute.** The ALU compares the two numbers, using a logic gate,
   the same kind you studied last week, to decide true or false.

This is why last week's gates still matter. The ALU is built from
gates. It just uses many of them together, to do one exact job.

The whole calculator example, all three cycles, takes a tiny fraction
of one second. A real laptop CPU repeats this cycle billions of times
every second.

---

## 3. The Whole System: Memory, I/O, and the Bus

The CPU never works alone. A **computer system** is built from three
basic parts working together: the **CPU** (processes instructions),
**memory** (holds data and instructions temporarily), and **I/O**
(input/output: how the machine talks to the outside world, like a
keyboard or screen). Memory holds the program and data close by, ready
for the CPU to fetch. I/O devices are how you and the CPU exchange
information at all.

**The bus: how parts talk to each other.** CPU, memory, and I/O sit
in different places on the same chip and board. A **bus** is a shared
set of wires connecting them, letting them send data back and forth;
think of it like a shared hallway that every part uses to pass
information along. Without a bus, the CPU, memory, and keyboard would
have no physical way to reach each other at all.

Not everything traveling on the bus carries the same kind of
information:

- **Address bus:** carries the memory location the CPU wants to read
  or write.
- **Data bus:** carries the actual bits being read or written.
- **Control bus:** carries signals like "read" or "write," telling the
  other parts what kind of action this is.

**Worked example: fetching an instruction at address 100.** The CPU
puts `100` on the address bus, sets the control bus to "read," and
memory replies by putting the instruction's bits on the data bus.
Every single character you type takes a similar bus trip: the keyboard
(I/O) sends the keystroke in, memory holds it briefly, the CPU reads
it during its next fetch, and the result eventually travels back
across the bus to the screen (I/O).

**Meet the program counter.** The **program counter (PC)** is a
special register that always holds the memory address of the next
instruction to fetch. After each fetch, the PC automatically moves
forward to the next address. If the current instruction sits at
memory address 100, the PC already holds 100; the moment fetch
finishes, the PC updates to 101, pointing at the next instruction in
line.

---

## 4. Optional Reading: More Detail

This section holds extra detail that was trimmed from the slides. It
is optional, but useful if you want to go deeper.

**Why the stored-program idea mattered.** Before 1945, early computers
were wired by hand, for one task only. Changing the task meant days of
rewiring, with real wires, by hand. In 1945, mathematician John von
Neumann wrote down a simpler idea: store the program as data, in
memory, next to the numbers it works on. Let the machine step through
it alone, one instruction at a time. This idea is why your laptop can
run many different programs. Nobody rewires the chip for each app you
open.

**Why instructions are so simple.** Each instruction that a CPU
understands does one tiny job: load a number, add two numbers, store
a result, compare two values, or show something on screen. A single
instruction alone looks almost too simple to matter. But a real
program is just hundreds, or millions, of instructions like these, run
in the right order, very fast.

**From code to instructions.** A programmer writes code in a
programming language, like Python. This code is easy for a person to
read, but the CPU cannot read it directly. A translator program turns
that code into the simple instructions the CPU actually understands.
The CPU only ever sees these simple instructions, never the original
code. You will write real code starting in Week 10.

**Why clock speed and cores matter.** A CPU's clock is a fast, steady
beat that times each step of the cycle. **Clock speed** is how many
cycles a CPU can complete in one second, measured in hertz (cycles
per second); "giga" means billion, so "3 GHz" on a spec sheet means 3
billion cycles happen every second: about 0.33 nanoseconds per
cycle. Comparing two laptops running the exact same program: a 3.6
GHz laptop completes about 1.5 times as many cycles per second as a
2.4 GHz laptop (3.6 ÷ 2.4 = 1.5), so it likely finishes first.

More GHz is not the whole story, though. **Instruction throughput** is
how many actual instructions a CPU finishes per second, and it is not
quite the same as clock speed, because some instructions take more
than one cycle to finish. A simple instruction like "add" might finish
in one cycle, while a more complex one, like "divide," might need
several cycles chained together. Two CPUs with the exact same GHz can
still finish a different number of instructions per second, depending
on how many cycles each instruction needs.

**Pipelining** is one more reason CPUs feel so fast: the CPU rarely
waits for one instruction to fully finish before starting the next.
Pipelining means the CPU starts fetching the next instruction before
the current instruction has finished executing, overlapping the three
steps across several instructions at once, like a laundry line, where
while one load dries, a second load can already be washing, and a
third can already be loading in. Without pipelining, 3 instructions
take 9 separate steps (fetch, decode, execute, one at a time, for each
instruction). With pipelining, the same 3 instructions finish in only
5 steps, because each stage overlaps with the next instruction's
earlier stage.

Pipelining is not free, though. Sometimes one instruction needs the
exact result of the instruction right before it, before it can even
start; pipelining then has to pause and wait, losing some of its speed
advantage. A wrong guess about which instruction comes next, common
around decisions, can also force the CPU to throw away already-started
work.

Many modern laptops also have more than one **core** inside a single
chip. Each core is its own small CPU (a **single-core CPU** has only
one control unit, one ALU, and one set of registers), running its own
cycle, pipelined overlap included. More cores let a laptop run more
programs smoothly, at the same time, instead of rapidly switching
between them one by one. Given a task like calculating 4 separate
spreadsheet columns, a single core finishes column 1 completely, then
column 2, then column 3, then column 4; four cores can each take one
column, and all four finish at roughly the same time.

**Where this leads to careers.** Every job below starts with the same
fetch-decode-execute cycle you learned this week:

- **Computer architect** — designs how the CPU's parts fit together.
- **Firmware engineer** — writes the lowest-level instructions a
  device runs first, before any app opens.
- **Embedded engineer** — builds small CPUs inside cars, watches, and
  home appliances.

"Explain how a CPU runs one instruction" is a common interview
question for hardware and firmware jobs, because it checks whether a
candidate understands the whole chip, not just one part.

---

## 5. Practice Problems (with Answers)

Try each problem yourself before checking the answer.

**Problem 1.** Name the three steps in the CPU's repeating cycle, in
the correct order.

> **Answer:** Fetch, then decode, then execute.

**Problem 2.** Which CPU part actually does the math, like adding two
numbers?

> **Answer:** The ALU (arithmetic logic unit).

**Problem 3.** A friend says: "The CPU understands math, like a
person does." Explain, in one sentence, why this is wrong.

> **Answer:** The CPU does not understand anything; it only follows
> exact instructions, step by step, exactly as written.

**Problem 4.** Your laptop's spec sheet says "3 GHz, 8 cores." Explain
what each number means, in plain words.

> **Answer:** "3 GHz" means the clock ticks 3 billion times a second.
> "8 cores" means the chip holds 8 small CPUs, each running its own
> cycle.

**Problem 5.** Put these three CPU parts with their correct job:
control unit, ALU, register.

> **Answer:** Control unit directs each step. ALU does math and
> comparisons. Register holds data the CPU is using right now.

**Problem 6.** A calculator app shows the wrong answer. Name two
different parts, or steps, that could each explain this alone.

> **Answer:** Any two of: the ALU did the math step wrong, the
> program sent the wrong instruction, or a value in a register was
> read at the wrong step.

**Problem 7.** Which bus carries signals like "read" or "write"?

> **Answer:** The control bus.

**Problem 8.** The program counter (PC) holds address 500 before a
fetch. What value does it hold right after that fetch finishes?

> **Answer:** 501. The PC always moves forward to the next address
> right after a fetch.

**Problem 9.** Without pipelining, 3 instructions take 9 separate
steps. With pipelining, how many steps do they take, and why?

> **Answer:** 5 steps, because pipelining overlaps fetch, decode, and
> execute across instructions instead of finishing each one fully
> before starting the next.
