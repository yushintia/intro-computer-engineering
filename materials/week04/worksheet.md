# Week 4 Worksheet: Inside Your Laptop's CPU

Introduction to Computer Engineering (400507-001) · Week 4
Work with a partner. Every task below is about the same CPU: the one
inside your own laptop or phone, running one instruction at a time.

---

## Part A (Session 2, in-class, ~15 minutes)

Each scenario below lists the three cycle steps **out of order**.
Write **1, 2, 3** next to each step, to show the correct order:
**fetch, decode, execute.**

1. **Your laptop's calculator app adds two numbers.**
   - ___ The ALU adds the two numbers together.
   - ___ The control unit gets the "add" instruction from memory.
   - ___ The control unit figures out this instruction is a math step.

2. **Your laptop's photo app rotates a picture.**
   - ___ The control unit figures out this instruction means "rotate."
   - ___ The right part turns the picture and updates the screen.
   - ___ The control unit gets the "rotate" instruction from memory.

3. **Your laptop's music app checks the volume level.**
   - ___ The ALU compares the volume to the maximum allowed level.
   - ___ The control unit gets the "compare volume" instruction.
   - ___ The control unit figures out this is a true-or-false step.

4. **Your laptop's game checks if you pressed the jump key.**
   - ___ The control unit gets the next instruction from memory.
   - ___ The ALU checks: true or false, was the key pressed?
   - ___ The control unit figures out this instruction is a comparison.

5. **Your laptop's browser shows a saved answer on screen.**
   - ___ The control unit figures out this instruction means "display."
   - ___ The screen shows the value that was in the register.
   - ___ The control unit gets the "display" instruction from memory.

6. **Your laptop's weather app stores a temperature it just read.**
   - ___ The control unit gets the "store" instruction from memory.
   - ___ The value moves into a register, ready for the next step.
   - ___ The control unit figures out this instruction means "store."

**Discuss with your partner:** Pick one scenario above. Explain, in
one sentence, what would go wrong if the CPU skipped the execute step.

______________________________________________

---

## Part B (Session 3, in-class, ~15 minutes)

Trace **one instruction** through the full cycle for each scenario.
Fill in what happens at each step, in your own words.

1. **Your laptop's camera app takes a photo. One instruction says:
   "store this image."**
   - Fetch: ______________________________________________
   - Decode: ______________________________________________
   - Execute: ______________________________________________

2. **Your laptop's browser loads a page. One instruction says:
   "compare the file size to the memory available."**
   - Fetch: ______________________________________________
   - Decode: ______________________________________________
   - Execute: ______________________________________________

3. **Your laptop's game runs. One instruction says: "add 10 points
   to the score."**
   - Fetch: ______________________________________________
   - Decode: ______________________________________________
   - Execute: ______________________________________________

4. **Your laptop's clock app runs. One instruction says: "show the
   current time on screen."**
   - Fetch: ______________________________________________
   - Decode: ______________________________________________
   - Execute: ______________________________________________

**Discuss with your partner:** Name one CPU part (control unit, ALU,
or register) used in scenario 3. Explain its job in that scenario, in
one sentence.

______________________________________________

---

## Part C (The Whole System: Memory, I/O, and the Bus)

1. A computer system is built from three basic parts. One is the CPU.
   Name the other two. ______________________ and ______________________
2. Which bus carries the memory location the CPU wants to read or
   write? ______________________
3. Which bus carries the actual bits being read or written? ______________________
4. Which bus carries signals like "read" or "write," telling the
   other parts what kind of action this is? ______________________
5. The program counter (PC) holds address 300 before a fetch happens.
   What value does the PC hold right after that fetch finishes? ______________________
6. **Trace a button press on a game controller.** Which part (CPU,
   memory, or I/O) detects the button press first? Which part decides,
   true or false, whether it means "jump"? ______________________

**Discuss with your partner:** Without a bus, could the CPU ever reach
memory at all? Explain in one sentence.

______________________________________________

---

## Part D (Speed and Parallelism: Clock, Pipelining, and Cores)

1. A laptop's spec sheet says "2.8 GHz." What does this mean, in
   plain words? ______________________
2. Laptop A runs at 2 GHz. Laptop B runs at 4 GHz. Both run the exact
   same program. Which one completes more cycles per second, and by
   what factor? ______________________
3. Without pipelining, 3 instructions take 9 separate steps to finish.
   With pipelining, how many steps do the same 3 instructions take? ______________________
4. Instruction 2 needs the exact result instruction 1 is still
   computing. What has to happen to instruction 2's execute step? ______________________
5. A laptop needs to calculate 4 separate spreadsheet columns.
   Compare: how does a single-core CPU handle this task, versus a
   4-core CPU? ______________________
6. **True or false:** "Two CPUs with the exact same GHz always finish
   the exact same number of instructions per second." Explain in one
   sentence. ______________________

**Discuss with your partner:** Name one real limit that can force
pipelining to pause (a hazard, or a wrong guess about which
instruction comes next).

______________________________________________
