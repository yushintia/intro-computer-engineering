## Professor Answer Key — do not hand out this section

Accept any reasonable, well-explained answer. The goal is correct gate
reasoning, not a single memorized phrasing.

### Part A

1. **AND.** Row order: No/No → No, No/Yes → No, Yes/No → No,
   Yes/Yes → **Yes**. Both conditions must hold.
2. **OR.** Row order: No/No → No, No/Yes → **Yes**, Yes/No → **Yes**,
   Yes/Yes → **Yes**. Either condition is enough.
3. **NOT.** Row order: Yes (someone looking) → No; No (no one
   looking) → **Yes**. The gate flips the input.
4. **AND.** Both "seat empty" and "seatbelt sign off" must be true at
   the same time for the light to turn on.
5. **OR.** Either a landed hit or a low-health warning alone is
   enough to trigger vibration.

### Part B

1. **AND with a NOT inside it.** The elevator needs the floor reached
   AND the doors not already open (NOT flips "doors already open").
2. **AND with an OR inside it.** The door must be closed (AND), and
   either the button was pressed or the timer reached zero (OR).
3. **AND with a NOT inside it.** The light needs no pedestrian request
   (NOT) AND the timer being done.
4. **Yes, the warning shows only if the AND gate's inputs are both
   true.** Fuel below 10% is true (8%). But NOT "just refueled" is
   false, since the car was just refueled. One false input means the
   AND gate outputs false. **So the warning does NOT show.** This is
   a common trap: fuel is low, but the recent refuel input matters.
5. **Open-ended.** Accept any answer that correctly names at least one
   gate and matches its own stated logic. Ask students to explain
   their gate choice out loud if time allows.

### Part C

**Section 1:**
1. **44 → `2C`.** 44 ÷ 16 = 2, remainder 12 (C); 2 ÷ 16 = 0, remainder
   2. Read last to first: 2, C.
2. **`10110100` → `B4`.** Split into `1011` (11 = B) and `0100` (4).

**Section 2:**
3. **0110 + 0101 = `1011`** (6 + 5 = 11). Column 1: 0+1=1. Column 2:
   1+0=1. Column 3: 1+1=0, carry 1. Column 4: 0+0+1=1.
4. **1001 + 0111 = `10000`** (9 + 7 = 16). Every column carries,
   producing a new leading digit.

**Section 3:**
5. **−6 = `11111010`.** Positive 6 = `00000110`. Flip: `11111001`.
   Add 1: `11111010`.
6. **−4 = `11111100`.** Positive 4 = `00000100`. Flip: `11111011`.
   Add 1: `11111100`.

**Section 4:**
7. **97 → `01100001`.** 64? Yes (97−64=33). 32? Yes (33−32=1). 16? No.
   8? No. 4? No. 2? No. 1? Yes (1−1=0).
8. **True.** ASCII only had room for 128 characters. Unicode assigns
   a unique number to characters from nearly every written language,
   plus symbols and emoji.

### Part D

**Section 1:**
1. **C · W**
2. **Ḡ**
3. **R + S**

**Section 2:**
4. **Yes, they agree.** Raining=Yes, Cold=No means AND needs every
   input true; one input is false either way, so both orders give
   **No**. Order never changes an AND's output.
5. **(NOT Sunny) OR (NOT Warm).**

**Section 3:**
6. **About 8 transistors** (2 for the NOT gate + 6 for the AND gate).
