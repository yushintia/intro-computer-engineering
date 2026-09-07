# Week 10 Worksheet: Instructions for Your Own Laptop

Introduction to Computer Engineering (400507-001) · Week 10
Work with a partner. There can be more than one correct answer.

This worksheet stays with our running device, **"What's Actually Inside
Your Laptop."** Mia's laptop needs exact steps for every task. So does
yours.

---

## Part A (Session 2, in-class, ~15 minutes)

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

## Part B (Session 3, in-class, ~15 minutes)

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

## Part C: From Code to Chip (~15 minutes)

### C1. Three levels, one task

Match each line below to its level: **Machine code · Assembly
language · High-level language**.

1. `total = total + 5`
   Level: ______________________________________________
2. `10110000 00000101`
   Level: ______________________________________________
3. `ADD A, 5`
   Level: ______________________________________________

### C2. Compiler or interpreter?

Mia's photo-renaming script has a typo on line 150. For each
description, write **Compiler** or **Interpreter**.

1. Reads all of Mia's code first, translates the whole thing, and
   only then lets it run. It refuses to finish, and tells Mia about
   the typo before a single photo is touched.
   ______________________________________________
2. Starts renaming photos immediately, translating and running one
   line at a time. By the time it reaches line 150 and crashes, the
   first 149 photos are already renamed.
   ______________________________________________
3. Which of the two above usually runs the finished program faster,
   once it starts?
   ______________________________________________
4. Which of the two above is easier to use for testing a small change
   quickly?
   ______________________________________________

### C3. Syntax error or logic error?

1. Mia's program is missing an `END FOR`. The translator refuses to
   run any of it at all.
   ______________________________________________
2. Mia's program runs from start to finish with no complaints, but it
   renames the photos in the wrong order because two steps were
   swapped.
   ______________________________________________

**Discuss with your partner:** Which kind of error — syntax or logic —
would a compiler most likely catch automatically? Which one usually
needs a person to notice it? Explain in one sentence.

______________________________________________

---

## Part D: Languages in the Wild (~15 minutes)

### D1. Class, object, method

Here is a class written in pseudocode, in the same style as class:

```
CLASS Song
    title
    artist
    duration

    METHOD play()
        ...
    END METHOD
END CLASS
```

1. Is `Song` a **class** or an **object**? ______________________
2. `song1` and `song2` are both built from the `Song` class. What do
   we call `song1` and `song2`? ______________________
3. Write one line of pseudocode that calls the `play` method on
   `song1`.
   ______________________________________________

### D2. 3GL steps vs. 4GL question

Below are two ways to find Mia's photos taken in Seoul.

```
FOR EACH photo IN photo_list
  IF photo.place == "Seoul"
    SHOW photo
  END IF
END FOR
```

```
SELECT * FROM Photos
WHERE Place = 'Seoul';
```

1. Which version is the **3GL**, and which is the **4GL**?
   ______________________________________________
2. In one sentence, what is the key difference between them?
   ______________________________________________

### D3. HTML, CSS, or JavaScript?

Mia is building a tiny webpage for her Seoul photos. For each action,
write **HTML**, **CSS**, or **JavaScript**.

1. Places one heading, "My Seoul Trip," and one image on the page.
   ______________________________________________
2. Centers that heading, and gives it a larger, bold font.
   ______________________________________________
3. Makes the image swap to the next photo when Mia clicks a button.
   ______________________________________________

### D4. Quick match

Write the correct word for each blank: **Unix · shell script · C# · C**

1. The language created in the early 1970s specifically to help
   build the ______________ operating system.
2. A short program made of ordinary command-line commands, saved
   together to run as one automated sequence, is called a
   ______________.
3. The flagship language of Microsoft's .NET ecosystem, used to build
   Windows, web, and business applications, is ______________.

**Discuss with your partner:** Pick one language mentioned today
(Python, C, Java, JavaScript, SQL, C#, or another). Is it usually
compiled or interpreted, and is it object-oriented? Use what you
learned today to explain your guess.

______________________________________________
