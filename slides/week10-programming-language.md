---
marp: true
theme: shintia
paginate: true
footer: 'Department of Intelligent Computing'
---

<!-- SLOT 1: Title -->
<!-- _class: title -->

# Week 10: Programming Language

<span class="subtitle">Introduction to Computer Engineering (400507-001)</span>

<div class="meta">
Yushintia Pramitarini, Ph.D · Dept. of Intelligent Computing · Thu [1-3] · Seongpa Hall 701
</div>

<!--
notes: Ask everyone: "Have you ever wanted your computer to do a
boring task for you, automatically?" Collect two or three answers.
-->

---

<!-- SLOT 2: Where we are -->

# Where We Are

<div class="roadmap">
<div class="wk"><div class="n">Wk 1</div><div class="t">Introduction</div></div>
<div class="wk"><div class="n">Wk 2</div><div class="t">Computer History</div></div>
<div class="wk"><div class="n">Wk 3</div><div class="t">Boolean Logic</div></div>
<div class="wk"><div class="n">Wk 4</div><div class="t">CPU &amp; Instructions</div></div>
<div class="wk"><div class="n">Wk 5</div><div class="t">Memory &amp; Storage</div></div>
<div class="wk"><div class="n">Wk 6</div><div class="t">Application Software · Quiz 1</div></div>
<div class="wk"><div class="n">Wk 7</div><div class="t">Operating Systems</div></div>
<div class="wk review"><div class="n">Wk 8</div><div class="t">Midterm Exam</div></div>
<div class="wk"><div class="n">Wk 9</div><div class="t">Computer &amp; Internet</div></div>
<div class="wk now"><div class="n">Wk 10</div><div class="t">Programming Language</div></div>
<div class="wk"><div class="n">Wk 11</div><div class="t">Databases &amp; Security</div></div>
<div class="wk"><div class="n">Wk 12</div><div class="t">Computer Applications</div></div>
<div class="wk"><div class="n">Wk 13</div><div class="t">AI · Quiz 2</div></div>
<div class="wk"><div class="n">Wk 14</div><div class="t">Emerging Technologies</div></div>
<div class="wk review"><div class="n">Wk 15</div><div class="t">Final Exam</div></div>
</div>

<!-- notes: Point at Week 10. Say: "Today we learn how people actually write the instructions a machine follows." -->

---

<!-- SLOT 3: Recap + open wound -->

# Last Week, This Week

- **Last week delivered:** two machines can now talk, and send data in small packets.
- **Last week left broken:** someone still has to write the instructions they exchange.

---

<!-- SLOT 4: The pain (Act 1 / MOTIVATE), ZERO jargon -->

# Who Writes The Instructions?

<div class="pain">

Two laptops can now send messages to each other. The connection
works fine.

But nothing happens by itself. A machine does not know what to send
back, on its own.

Someone still has to write the exact steps it should follow.

For example, Mia has 200 photos from a school trip. She wants her
laptop to rename them all, in a neat pattern, before she sends them.

She knows what she wants. She does not know how to tell her laptop
the exact steps.

</div>

<!-- notes: Ask: "How would you explain 200 renames to a machine that only follows exact steps?" Let two or three students guess. Do not explain yet. -->

---

<!-- SLOT 5: Cost of not knowing -->

# What This Actually Costs

- Without exact steps, boring tasks stay slow and full of mistakes.
- Every app, game, and website is just a long list of instructions.
- You cannot build anything new for a computer without this skill.

<div class="why">
<strong>In industry:</strong> most tech job listings ask for at least
one programming language. Coding interviews test this exact skill.
</div>

---

<!-- SLOT 6: Driving question -->

<!-- _class: section -->

# This Week's Question

<div class="driving-q">"What is a programming language, and why do computers need one?"</div>

---

<!-- SLOT 7: Learning outcomes -->

# By the End of This Week, You Can

<div class="cardlist">
<div class="card"><div class="h">What a Language Is</div><div class="d">Explain what a programming language is, in plain words.</div></div>
<div class="card"><div class="h">Exact Steps</div><div class="d">Explain why computers need exact steps, not plain English.</div></div>
<div class="card"><div class="h">Building Blocks</div><div class="d">Name the three basic building blocks of any program.</div></div>
<div class="card"><div class="h">Task to Steps</div><div class="d">Turn one everyday task into a short list of steps.</div></div>
</div>

---

<!-- SLOT 8: Origin -->

# Where This Idea Came From

<div class="thread">You just felt the pain. Where did the answer come from?</div>

- **1940s:** early computers were programmed by rewiring cables and switches, by hand.
- **Late 1940s:** short number codes replaced some rewiring. Still very hard to read.
- **1957:** FORTRAN let people write steps using words and math, closer to plain language.

<div class="why">
Each step made instructions easier for a person to write, and to
read again later.
</div>

---

<!-- SLOT 9: Core concept -->

# Programming Language: Definition

<div class="thread">One idea, one clear definition.</div>

> A **programming language** is a set of exact rules for writing
> instructions a computer can follow, one step at a time.

- It is not plain English. Its rules leave no room for confusion.
- **Code** is a list of instructions written in a programming language.
- A **programmer** is a person who writes code.

---

<!-- NEW: Key Words Today, session 1 -->

# Key Words Today

- **Instruction** — one exact command a computer can follow.
- **Programming language** — a set of exact rules for writing instructions.
- **Syntax** — the exact grammar rules of a programming language.
- **Code** — instructions written in a programming language.
- **Programmer** — a person who writes code.

<!-- notes: Read each word aloud. Ask students to repeat it once. Ask: "Which word did you already know?" -->

---

<!-- NEW: Try-It preview, closes session 1 -->

# Coming Up: Worksheet Part A

<div class="thread">Next, you will practice using these words.</div>

- In **[Worksheet Part A](materials/week10/worksheet.html)**, you turn plain requests into ordered steps.
- Example: "Make my laptop say hello." What steps does that need?
- You will work with a partner. A guess is fine for now.

<!-- notes: Tell students to sit next to a partner for the next part. No prep needed. -->

---

<!-- NEW: Key Words Today, session 2 -->

# Key Words Today

- **Sequence** — steps done one after another, in order.
- **Loop** — one step, or steps, repeated many times.
- **Automate** — let a computer do a repeated task for you.
- **Task** — one job you want a computer to do.

<!-- notes: Read each word aloud. Say: "You will use all four words in the next slides." -->

---

<!-- Act 3 / BUILD -->

# Plain English Is Not Exact Enough

<div class="thread">Words like "nicely" or "soon" mean nothing to a computer.</div>

- A person understands: "Rename my photos nicely."
- A computer understands none of that. It is not exact.
- A computer needs one exact step at a time, in order.

---

# A Program Is an Exact List of Steps

<div class="thread">This ordered list is called a sequence.</div>

<div class="pipeline">
<div class="stage"><div class="h">1. Open</div><div class="s">open one photo file</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">2. Read</div><div class="s">read its old name</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">3. Write</div><div class="s">write its new name</div></div>
</div>

Change the order, and the result can change too.

---

# Sequence in Pseudocode: A Worked Example

<div class="thread">"Open, read, write": now written as real pseudocode.</div>

```
OPEN photo_file
READ old_name FROM photo_file
WRITE new_name TO photo_file
```

- Each line runs exactly once, in exactly this order.
- Swap lines 2 and 3, and the program would try to write a name before it even reads the old one.
- A **sequence** is simply this: one instruction after another, top to bottom.

---

# Doing One Task Many Times

<div class="thread">Mia has 200 photos, not just one.</div>

- A **loop** repeats the same steps, again and again.
- Do the sequence once. Then do it again, for the next photo.
- 200 photos means 200 repeats. You only write the steps once.

---

# Loop in Pseudocode: A Worked Example

<div class="thread">200 photos means writing the sequence exactly once.</div>

```
FOR EACH photo IN photo_list
    OPEN photo
    READ old_name FROM photo
    WRITE new_name TO photo
END FOR
```

- `FOR EACH ... END FOR` marks where the repeating block starts and stops.
- The three lines inside run once per photo: 200 photos, 200 repeats, one loop.
- A **loop** does not copy the steps 200 times; it reuses the same three lines.

---

<!-- NEW: Try-It hand-off, Worksheet Part A -->

# Try It: Worksheet Part A

<div class="thread">Now you practice. Work with a partner.</div>

- Open **[Worksheet Part A](materials/week10/worksheet.html)**.
- Turn each plain request into an ordered list of steps.
- You have about 15 minutes. Ask your partner before you ask me.

<!-- notes: Hand out Worksheet Part A. Walk around and help pairs. After 15 minutes, ask 2-3 pairs to share one answer. -->

---

<!-- NEW: Key Words Today, session 3 -->

# Key Words Today

- **Decision** — a point where a program picks between two paths.
- **Translator** — software that changes code into instructions a chip can run.
- **Compiler** — a translator that changes all the code at once, before running.
- **Interpreter** — a translator that changes code one line at a time, while running.
- **Bug** — a mistake in code that makes a program act wrong.

<!-- notes: Read each word aloud. Say: "These words tie everything together today." -->

---

# Making a Choice

<div class="thread">Not every photo should get the same treatment.</div>

- A **decision** lets a program pick between two paths.
- Example: "If this name is already used, skip this photo."
- Otherwise, follow the normal steps, and give it a new name.

---

# Decision in Pseudocode: A Worked Example

<div class="thread">Not every photo should be renamed the same way.</div>

```
FOR EACH photo IN photo_list
    IF new_name ALREADY EXISTS
        SKIP photo
    ELSE
        WRITE new_name TO photo
    END IF
END FOR
```

- `IF ... ELSE ... END IF` marks the two possible paths.
- Only one branch runs for each photo: either **SKIP**, or **WRITE**, never both.
- A **decision** lets the same loop treat different photos differently.

---

# Pseudocode Cheat Sheet

<div class="thread">Three keywords, three building blocks, before we zoom out.</div>

<div class="chip-row">
<span class="chip">Sequence: one line after another</span>
<span class="chip">FOR EACH ... END FOR: a loop</span>
<span class="chip">IF ... ELSE ... END IF: a decision</span>
</div>

---

# From Words to Something a Chip Can Run

<div class="thread">Week 4 met the CPU. Here is how it gets fed.</div>

<div class="pipeline">
<div class="stage"><div class="h">Code</div><div class="s">written by a person, in a language</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Translator</div><div class="s">a compiler or an interpreter</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">CPU</div><div class="s">runs the translated instructions</div></div>
</div>

A translator changes code a person can read into signals only the chip understands.

---

# Machine Code: The Chip's Only Native Language

<div class="thread">A "translator" was mentioned. Translated into what, exactly?</div>

> **Machine code** is the raw pattern of 0s and 1s that a CPU's circuits can directly read and execute, with no translation needed.

- Week 3 and Week 4 already met this idea: instructions as patterns of on and off signals.
- A single machine-code instruction might look like `10110000 00000101`: add two tiny numbers together.
- No one writes large programs directly in machine code today. It is far too tedious, and too easy to mistype.

---

# Assembly Language: One Small Step Up

<div class="thread">The very next rung up the ladder, still close to the chip.</div>

> **Assembly language** replaces raw binary patterns with short, readable mnemonics, one mnemonic per machine instruction.

- The same instruction from the last slide might be written as `ADD A, 5`.
- Assembly still matches the chip's instructions almost one-for-one, just spelled in words a person can read.
- A translator called an **assembler** turns assembly back into the exact machine code the chip needs.

---

# High-Level Languages: Closer to Human Thought

<div class="thread">Most programmers today never see assembly at all.</div>

> A **high-level language** lets a programmer describe a task using words and structure close to human thought, far from the chip's own instructions.

- One line of a high-level language, like `total = total + 5`, can replace several lines of assembly.
- High-level code is not tied to one specific chip design, unlike assembly.
- This week's "sequence, loop, decision" pseudocode is written at this high level.

---

# Worked Mini-Example: One Task, Three Levels

<div class="thread">"Add 5 to a number": the exact same task, three different levels.</div>

| Level | What it looks like |
|---|---|
| High-level | `total = total + 5` |
| Assembly | `ADD A, 5` |
| Machine code | `10110000 00000101` |

Same task, same final result inside the chip, just written for three very different readers: a person, an assembler, and a CPU.

---

# Language Timeline: From FORTRAN to Today

<div class="thread">Slot 8 met FORTRAN. Many more languages followed.</div>

<div class="timeline">
<div class="pt"><div class="dot"></div><div class="y">1957</div><div class="d">FORTRAN: an early high-level language, built for math and science.</div></div>
<div class="pt"><div class="dot"></div><div class="y">1972</div><div class="d">C: fast, close to hardware, later builds much of Unix.</div></div>
<div class="pt"><div class="dot"></div><div class="y">1991</div><div class="d">Python: readable syntax, aimed at fast, easy development.</div></div>
<div class="pt"><div class="dot"></div><div class="y">1995</div><div class="d">Java and JavaScript: one for large apps, one for web pages.</div></div>
</div>

Each new language answered a limit of the languages before it, the same pattern as slot 8's own story.

---

# Compiler: Translate First, Then Run

<div class="thread">One of the two translator styles named in session 3's key words.</div>

> A **compiler** reads all of a program's code at once, translates the whole thing into machine code, and only then lets it run.

- Compiling happens once, ahead of time; running happens separately, afterward.
- A compiler can catch many mistakes during translation, before the program ever runs at all.
- C is usually compiled, which is part of why compiled C programs run so fast.

---

# Interpreter: Translate and Run, Line by Line

<div class="thread">The other translator style.</div>

> An **interpreter** reads and translates a program one line at a time, running each line immediately, without a separate translation stage first.

- There is no separate "compile now, run later" step; translating and running happen together.
- Mistakes on a later line are not caught until the program actually reaches that line while running.
- Python is usually interpreted, which is part of why testing a small change is so quick.

---

# Compiler vs. Interpreter: Trade-offs

<div class="thread">Neither style is simply "better." Each trades one thing for another.</div>

<div class="two-col">
<div>

**Compiler**
- Slower to start (must translate first).
- Catches many mistakes before running.
- Finished program usually runs faster.

</div>
<div>

**Interpreter**
- Runs almost immediately, line by line.
- Some mistakes only appear while running.
- Easier to test small changes quickly.

</div>
</div>

---

# Worked Example: Compiling vs. Interpreting Mia's Script

<div class="thread">Back to the photo-renaming program, both ways.</div>

- **Compiled version:** Mia's whole renaming program is translated into machine code first. If line 150 has a typo, the compiler refuses to finish, and tells her before any photo is touched.
- **Interpreted version:** Mia's program starts renaming photos immediately. If line 150 has a typo, the first 149 photos may already be renamed before it crashes.

<div class="why">
Same bug, same program, but the two translator styles catch it at very different moments.
</div>

---

# Many Languages, Many Jobs

<div class="thread">No single language does every job best.</div>

<div class="appgrid">
<div class="app"><div class="name">Python</div><div class="desc">Easy to learn. Popular for data and quick tasks.</div></div>
<div class="app"><div class="name">JavaScript</div><div class="desc">Runs inside web pages, in your browser.</div></div>
<div class="app"><div class="name">C</div><div class="desc">Controls hardware directly. Very fast, close to the chip.</div></div>
<div class="app"><div class="name">Swift</div><div class="desc">Builds apps for iPhones and iPads.</div></div>
<div class="app"><div class="name">Java</div><div class="desc">Runs large business and Android apps.</div></div>
<div class="app"><div class="name">SQL</div><div class="desc">Asks questions of a database. Week 11.</div></div>
</div>

Every language follows the same idea: exact rules, exact steps.

---

# Major Languages at a Glance

<div class="thread">Four languages, one defining trait each, before we go deeper.</div>

| Language | Defining trait | Typical use |
|---|---|---|
| C | Fast, close to hardware | Operating systems, embedded devices |
| Python | Readable, quick to write | Data analysis, automation, quick scripts |
| Java | Runs the same on many machines | Large business systems, Android apps |
| JavaScript | Runs inside a web browser | Interactive, dynamic web pages |

---

# Worked Example: Same Task, Two Languages' Styles

<div class="thread">"Print hello 3 times": the same task, two very different feels.</div>

<div class="two-col">
<div>

**Python-style**
```
for i in range(3):
    print("hello")
```

</div>
<div>

**C-style**
```
for (i=0; i<3; i++) {
    printf("hello");
}
```

</div>
</div>

Same loop, same result: Python favors short, readable lines; C favors explicit, exact control.

---

# Fourth-Generation Languages: Getting Even Higher-Level

<div class="thread">High-level languages themselves come in different "how high" levels.</div>

> A **fourth-generation language (4GL)** lets a person describe *what* result they want, without spelling out *how* to compute it step by step.

- Earlier ("third-generation") languages like Python or C still need an explicit sequence, loop, and decision written out.
- SQL, which Week 11 introduces, is a classic 4GL: you describe the data you want, not the steps to fetch it.
- A higher generation number roughly means: less step-by-step detail is left for the programmer to spell out.

---

# Worked Example: A 3GL's Steps vs. a 4GL's Question

<div class="thread">Same goal: "find Mia's photos taken in Seoul."</div>

<div class="two-col">
<div>

**3GL (step by step)**
```
FOR EACH photo IN photo_list
  IF photo.place == "Seoul"
    SHOW photo
  END IF
END FOR
```

</div>
<div>

**4GL (just the question)**
```
SELECT * FROM Photos
WHERE Place = 'Seoul';
```

</div>
</div>

The 4GL version never mentions a loop at all: the database handles the "how" on its own.

---

# Object-Oriented Programming: The Big Idea

<div class="thread">A different way to organize a program's code entirely.</div>

> **Object-oriented programming** organizes a program around **objects**: bundles that hold both data and the actions that work on that data, together.

- Instead of writing separate steps and separate data, each object owns both at once.
- A **class** is the blueprint that describes what an object of that kind will contain.
- An **object** is one actual instance built from that blueprint.

---

# Class vs. Object: Blueprint vs. Real Thing

<div class="thread">One blueprint, many real things built from it.</div>

```
CLASS Photo
    name
    date
    place
END CLASS
```

- **`Photo`** the class only describes the *shape* of a photo: name, date, place. It is not any specific photo.
- `photo1` and `photo2` are two separate **objects**, each built from the `Photo` class, each with its own actual values.
- Mia's 200 photos are 200 objects, all built from one single `Photo` class.

---

# Methods: Actions an Object Can Do

<div class="thread">An object's data, and its own actions, travel together.</div>

```
CLASS Photo
    name
    date
    place

    METHOD rename(new_name)
        name = new_name
    END METHOD
END CLASS
```

- A **method** is an action defined inside a class, that an object of that class can perform.
- Calling `photo1.rename("IMG_seoul_01")` runs the `rename` method on that one specific object.
- The renaming logic lives right next to the data it changes, instead of sitting somewhere else entirely.

---

# C and Unix: Close Partners

<div class="thread">One language, one operating system family, built together.</div>

- The C language was created in the early 1970s specifically to help build the **Unix** operating system.
- Because C compiles into fast, hardware-close code, it became the natural choice for writing an operating system itself.
- Linux, Unix's best-known descendant, is still written mostly in C today, decades later.

---

# Shell Scripting: Automating the Command Line

<div class="thread">Not every program needs a full application. Some just need a short list of commands.</div>

> A **shell script** is a short program made of ordinary command-line commands, saved together so they can run as one single automated sequence.

```
mkdir renamed_photos
mv IMG001.jpg renamed_photos/
mv IMG002.jpg renamed_photos/
```

- Each line is a command a person could type by hand: a shell script just runs them all in order, automatically.
- Common on Unix and Linux systems, where the command line is a first-class way to work.

---

# HTML, CSS, and JavaScript: Three Different Jobs

<div class="thread">A single webpage is actually written in three separate languages.</div>

<div class="cardlist">
<div class="card"><div class="h">HTML</div><div class="d">Defines the page's structure and content: headings, paragraphs, images.</div></div>
<div class="card"><div class="h">CSS</div><div class="d">Defines the page's appearance: colors, fonts, spacing, layout.</div></div>
<div class="card"><div class="h">JavaScript</div><div class="d">Defines the page's behavior: what happens when you click or type.</div></div>
</div>

None of the three replaces another. A modern webpage almost always uses all three together.

---

# Worked Example: Building One Simple Webpage

<div class="thread">Mia wants a tiny webpage to show off her Seoul photos.</div>

- **HTML** places one heading, "My Seoul Trip," and one image on the page.
- **CSS** centers that heading, and gives it a larger, bold font.
- **JavaScript** makes the image swap to the next photo when Mia clicks a button.

Remove the JavaScript, and the page still shows the same photo; it just cannot respond to a click.

---

# The .NET Family: C# and a Managed Ecosystem

<div class="thread">One more major family, common in business software.</div>

> **.NET** is a language-and-tools ecosystem built by Microsoft; **C#** is its flagship language, designed to build Windows, web, and business applications.

- C# borrows much of its structure and feel from Java, including strong support for object-oriented programming.
- The .NET ecosystem also includes shared libraries and tools that many different applications reuse.
- Like Java, C# is common in large organizations that need to maintain software for many years.

---

# The Wider Language Ecosystem

<div class="thread">Zoom all the way out before choosing.</div>

<div class="appgrid">
<div class="app"><div class="name">Compiled languages</div><div class="desc">Translated fully before running, e.g. C.</div></div>
<div class="app"><div class="name">Interpreted languages</div><div class="desc">Translated and run line by line, e.g. Python.</div></div>
<div class="app"><div class="name">Object-oriented languages</div><div class="desc">Organized around objects, e.g. Java, C#.</div></div>
<div class="app"><div class="name">Query languages</div><div class="desc">Ask a question of stored data, e.g. SQL.</div></div>
<div class="app"><div class="name">Scripting languages</div><div class="desc">Automate short, repeated tasks, e.g. shell scripts.</div></div>
<div class="app"><div class="name">Web languages</div><div class="desc">Build what runs inside a browser: HTML, CSS, JavaScript.</div></div>
</div>

---

# Syntax Errors vs. Logic Errors

<div class="thread">Session 3 named "bug." Not every bug looks the same.</div>

- A **syntax error** breaks the language's own exact rules, like a missing `END FOR`. A translator refuses to proceed at all.
- A **logic error** follows every rule perfectly, but still does the wrong thing, like renaming photos in the wrong order.
- A compiler or interpreter can catch a syntax error automatically. Only a person, checking results, tends to catch a logic error.

---

# How Do You Pick a Language?

<div class="thread">One last, practical question, before we move to Week 11.</div>

<div class="cardlist">
<div class="card"><div class="h">What's the task?</div><div class="d">A quick script favors Python; an operating system favors C.</div></div>
<div class="card"><div class="h">Where does it run?</div><div class="d">Inside a browser, JavaScript is close to the only choice.</div></div>
<div class="card"><div class="h">How fast must it run?</div><div class="d">Compiled languages usually beat interpreted ones for raw speed.</div></div>
<div class="card"><div class="h">What does your team know?</div><div class="d">A language your team already knows ships faster than a "perfect" unfamiliar one.</div></div>
</div>

---

<!-- SLOT N-2: Worked example -->

# Case Study: The Photo-Renaming Plan

<div class="thread">Back to Mia's laptop. Now she has the words.</div>

<div class="chip-row">
<span class="chip">Sequence: open, read, write</span>
<span class="chip">Loop: repeat for each photo</span>
<span class="chip">Decision: skip if name is taken</span>
</div>

Together, these three blocks solve Mia's whole problem. A translator
then turns her code into steps her laptop's chip can run.

---

<!-- SLOT N-1: Common mistakes -->

# Common Mistakes

- **"The computer understands normal English":** Wrong. It needs exact, agreed steps.
- **"A program only runs once, top to bottom":** Wrong. Loops repeat steps many times.
- **"Only one language is the 'real' one":** Wrong. Different languages suit different jobs.

---

<!-- NEW: Try-It hand-off, Worksheet Part B -->

# Try It: Worksheet Part B

<div class="thread">More practice. New scenarios.</div>

- Open **[Worksheet Part B](materials/week10/worksheet.html)**.
- Find the sequence, the loop, and the decision in each scenario.
- You have about 15 minutes. Then we discuss answers together.

<!-- notes: Hand out Worksheet Part B. After 15 minutes, go through the answer key as a class. Ask for volunteers first. -->

---

<!-- SLOT N: Check yourself -->

# Check Yourself

1. What is a programming language, in your own words?
2. Name the three building blocks of a program.
3. Mia's laptop must skip photos that already have a name. Which building block does that?

---

# Answers

1. Sample: exact rules for writing instructions a computer can follow.
2. Sequence, loop, and decision.
3. Decision — it picks between two paths, like skip or rename.

---

<!-- NEW: Self-check quiz hand-off -->

# Self-Check Quiz

<div class="thread">One more check, on your own.</div>

- Take the **[Week 10 Quiz](materials/week10/quiz.html)** (5-8 short questions).
- This quiz is not graded. It just checks your understanding.
- About 10 minutes. Check your own answers at the end.

<!-- notes: Hand out the quiz. Give students 10 minutes. Then read the answer key aloud, or let students self-check. -->

---

<!-- SLOT N+1: Limits (Act 4 / CLOSE), becomes Week 11 slot 4 -->

# What Writing Instructions Cannot Do Yet

<div class="limits">
We can now write those instructions. But a program with no data to
manage is not very useful yet. Where does a program keep the names,
numbers, and photos it works with? We do not know yet.
</div>

---

<!-- SLOT N+2: Bridge -->

# Next Week

Week 10 leaves **managing data** unsolved. **Week 11, Databases &
Security**, addresses it: how programs store, find, and protect data.

---

<!-- SLOT N+3: Summary -->

# Summary

- A programming language is a set of exact rules for instructions.
- Every program is built from three blocks: sequence, loop, decision.
- A translator changes code into instructions a chip can run.
- **Reading:** Tanenbaum & Austin, the chapter on programming languages and software development.
- **Handout:** [materials/week10/handout.md](materials/week10/handout.html), glossary and the full worked example.
- **Prepare:** Think of one task your laptop repeats for you. Bring it to Week 11.

---

<!-- SLOT N+4: Thank You -->
<!-- _class: end -->

# Thank You
