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
