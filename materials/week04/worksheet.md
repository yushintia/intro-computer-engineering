# Week 4 Worksheet: Inside Your Laptop's CPU

Introduction to Computer Engineering (400507-001) · Week 4
Work with a partner. Every task below is about the same CPU: the one
inside your own laptop or phone, running one instruction at a time.

---

## Part A (차시 2, in-class, ~15 minutes)

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

## Part B (차시 3, in-class, ~15 minutes)

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
---

## Instructor Answer Key — do not hand out this section

### Part A

1. Add two numbers: **2, 1, 3**
   (Control unit fetches → control unit decodes → ALU executes.)
2. Rotate a picture: **2, 3, 1**
   (Fetch happens first, decode second, execute third; the list is
   given out of order, so match the action to its step.)
3. Check volume: **2, 3, 1**
4. Check jump key: **1, 3, 2**
5. Display saved answer: **3, 1, 2**
6. Store temperature: **1, 3, 2**

Accept minor reordering disagreements if a pair can explain their
reasoning; the goal is understanding fetch-decode-execute, not
memorizing a list.

**Discuss:** Any reasonable answer is fine. Sample: "If the CPU
skipped execute, the instruction would be understood, but nothing
would actually happen — no math, no display, no store."

### Part B

Accept any reasonable, well-explained answer that uses the right
step correctly. Sample answers:

1. **Store this image.**
   - Fetch: the control unit gets the "store" instruction from memory.
   - Decode: the control unit sees this means "save data."
   - Execute: the image data moves into storage.

2. **Compare file size to memory available.**
   - Fetch: the control unit gets the "compare" instruction.
   - Decode: the control unit sees this is a true-or-false step.
   - Execute: the ALU compares the two numbers and decides true or
     false.

3. **Add 10 points to the score.**
   - Fetch: the control unit gets the "add" instruction from memory.
   - Decode: the control unit sees this is a math step.
   - Execute: the ALU adds 10 to the score; the new score goes into a
     register.

4. **Show the current time on screen.**
   - Fetch: the control unit gets the "display" instruction.
   - Decode: the control unit sees this means "show on screen."
   - Execute: the screen shows the current time.

**Discuss:** In scenario 3, the **ALU** does the addition. Its job is
to do the actual math, adding 10 to the current score.
