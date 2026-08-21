# Week 10 Worksheet: Instructions for Your Own Laptop

Introduction to Computer Engineering (400507-001) · Week 10
Work with a partner. There can be more than one correct answer.

This worksheet stays with our running device, **"What's Actually Inside
Your Laptop."** Mia's laptop needs exact steps for every task. So does
yours.

---

## Part A (차시 2, in-class, ~15 minutes)

For each plain request, write an ordered list of exact steps a laptop
would need. Use short, exact actions (open, read, write, check, show,
save). Aim for 3-5 steps each.

1. **"Make my laptop say hello."**
   Steps: ______________________________________________
   ______________________________________________________

2. **"Save my essay before I close the app."**
   Steps: ______________________________________________
   ______________________________________________________

3. **"Show me the time when I open my laptop."**
   Steps: ______________________________________________
   ______________________________________________________

4. **"Turn the volume down when I plug in my headphones."**
   Steps: ______________________________________________
   ______________________________________________________

5. **"Rename one photo, from 'IMG_001' to 'trip_1'."**
   Steps: ______________________________________________
   ______________________________________________________

6. **"Lock my laptop after five minutes with no typing."**
   Steps: ______________________________________________
   ______________________________________________________

**Discuss with your partner:** Pick one request above. Could the order
of your steps change the result? Give one example.

______________________________________________

---

## Part B (차시 3, in-class, ~15 minutes)

Mia's laptop now runs several small programs. For each scenario, name
which building block matters most: **sequence, loop, or decision**.
Then explain your choice in one short sentence.

1. **Mia's laptop renames all 200 trip photos, one after another.**
   Building block: Sequence / Loop / Decision
   Why: ______________________________________________

2. **Before renaming a photo, the laptop checks: "Is this name already
   used?" If yes, it skips the photo.**
   Building block: Sequence / Loop / Decision
   Why: ______________________________________________

3. **For one photo, the laptop opens the file, reads the old name,
   then writes the new name, in that exact order.**
   Building block: Sequence / Loop / Decision
   Why: ______________________________________________

4. **Mia's laptop plays the next song automatically after each song
   ends, all evening.**
   Building block: Sequence / Loop / Decision
   Why: ______________________________________________

5. **A backup program checks: "Is the laptop plugged in?" If yes, it
   backs up files now. If no, it waits.**
   Building block: Sequence / Loop / Decision
   Why: ______________________________________________

6. **A weather app opens, connects to the internet, downloads data,
   then shows today's forecast, in that exact order.**
   Building block: Sequence / Loop / Decision
   Why: ______________________________________________

**Discuss with your partner:** Which scenario in Part B used more than
one building block? Name both.

______________________________________________

---
---

## Instructor Answer Key — do not hand out this section

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
