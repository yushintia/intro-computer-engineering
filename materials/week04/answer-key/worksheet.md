## Professor Answer Key — do not hand out this section

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
