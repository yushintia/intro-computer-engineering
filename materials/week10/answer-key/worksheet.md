## Professor Answer Key — do not hand out this section

Accept any reasonable, well-explained answer. The goal is correct
ordering and reasoning, not one exact wording.

### Part A

1. Sample: (1) check the speaker works, (2) load the word "hello,"
   (3) play it as sound. Order matters: playing before loading fails.
2. Sample: (1) check for unsaved changes, (2) write the essay to a
   file, (3) confirm it saved, (4) close the app.
3. Sample: (1) turn on, (2) check the current time, (3) show it on
   screen.
4. Sample: (1) detect headphones plugged in, (2) check current volume,
   (3) lower the volume, (4) apply the new level.
5. Sample: (1) open the photo file, (2) read the old name ("IMG_001"),
   (3) write the new name ("trip_1"), (4) save the file.
6. Sample: (1) start a timer at last keypress, (2) check if 5 minutes
   passed with no typing, (3) if yes, lock the screen.

### Part B

1. **Loop.** The same rename steps repeat for each of the 200 photos.
2. **Decision.** The program picks between two paths: skip, or
   continue renaming.
3. **Sequence.** Three exact steps happen once, in a fixed order.
4. **Loop.** The "play next song" step repeats automatically, again
   and again.
5. **Decision.** The program picks between two paths based on one
   check: plugged in, or not.
6. **Sequence.** Four exact steps happen once, in a fixed order, to
   produce one forecast.

Scenario with more than one block (for the discussion question): the
overall photo-renaming plan (Case Study, main slides) uses all three —
sequence for one photo, loop for 200 photos, decision to skip taken
names. Accept students who notice scenario 1 or 2 also implies a
sequence underneath the loop or decision.

### Part C

**C1.**
1. High-level language. Close to human thought, e.g. `total = total + 5`.
2. Machine code. Raw 0s and 1s the CPU reads directly.
3. Assembly language. Short, readable mnemonics, matching the chip's instructions almost one-for-one.

**C2.**
1. Compiler. Translates all the code first, before running.
2. Interpreter. Translates and runs one line at a time.
3. Compiler. Once translated, the finished program usually runs faster.
4. Interpreter. Runs almost immediately, so testing a small change is quick.

**C3.**
1. Syntax error. It breaks the language's own exact rules; the
   translator refuses to proceed.
2. Logic error. Every rule is followed, but the program still does
   the wrong thing.

Discuss answer (sample): "A compiler (or interpreter) catches a syntax
error automatically, since it breaks the language's own rules. A
logic error still follows every rule, so only a person, checking the
results, tends to catch it."

### Part D

**D1.**
1. `Song` is a **class**: it only describes the shape of a song
   (title, artist, duration), not any one specific song.
2. `song1` and `song2` are both **objects**, built from the `Song`
   class.
3. Sample: `song1.play()`.

**D2.**
1. The `FOR EACH ... IF ... END FOR` version is the **3GL**; the
   `SELECT * FROM Photos WHERE ...` version is the **4GL**.
2. Sample: The 3GL spells out every step (loop, check, show); the
   4GL only describes the result wanted, and never mentions a loop
   at all.

**D3.**
1. HTML: structure and content.
2. CSS: appearance: colors, fonts, layout.
3. JavaScript: behavior: what happens on a click.

**D4.**
1. Unix.
2. Shell script.
3. C#.

Discuss answer (sample): "Python is usually interpreted, and is
object-oriented: it supports classes and objects, even though this
week's simple pseudocode examples did not use Python syntax
specifically."
