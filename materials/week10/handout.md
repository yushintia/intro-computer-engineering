# Week 10 Handout: Programming Language

Introduction to Computer Engineering (400507-001) · Week 10
This handout goes with the Week 10 slides. Keep it for the whole semester.

---

## 1. Glossary: Key Words

Simple, plain definitions. Read these before or after class.

| Word | Plain definition |
|---|---|
| **Instruction** | One exact command a computer can follow. |
| **Programming language** | A set of exact rules for writing instructions. |
| **Syntax** | The exact grammar rules of a programming language. |
| **Code** | Instructions written in a programming language. |
| **Programmer** | A person who writes code. |
| **Sequence** | Steps done one after another, in order. |
| **Loop** | One step, or steps, repeated many times. |
| **Automate** | Let a computer do a repeated task for you. |
| **Task** | One job you want a computer to do. |
| **Decision** | A point where a program picks between two paths. |
| **Translator** | Software that changes code into instructions a chip can run. |
| **Compiler** | A translator that changes all the code at once, before running. |
| **Interpreter** | A translator that changes code one line at a time, while running. |
| **Bug** | A mistake in code that makes a program act wrong. |

---

## 2. The Photo-Renaming Plan, Step by Step

This is the full version of the story from class. The slide version was
shortened. Read this at home if you want more detail.

Mia has 200 photos from a school trip. She wants her laptop to rename
them all, in a neat pattern, before she sends them.

She knows what she wants. She does not know how to tell her laptop the
exact steps. Plain English is not exact enough for a computer. Words
like "nicely" mean nothing to a machine. A computer needs one exact
step at a time, in order.

Here is how the three building blocks solve her whole problem, one
photo at a time.

**Step 1 — Sequence.** For one photo, do three exact steps, in order:

1. Open the photo file.
2. Read its old name.
3. Write its new name.

Change the order of these steps, and the result can change too. For
example, writing a new name before reading the old one would lose the
old name forever.

**Step 2 — Loop.** Mia has 200 photos, not just one. A loop repeats the
same sequence, again and again. Do the sequence once, for photo 1.
Then do it again, for photo 2. Repeat until all 200 photos are done.
Mia only writes the three steps once; the loop repeats them 200 times.

**Step 3 — Decision.** Not every photo should get the same treatment.
A decision lets the program pick between two paths. Here, the rule is:
"If this name is already used, skip this photo. Otherwise, follow the
normal steps, and give it a new name." This stops the program from
overwriting a file by accident.

**Step 4 — Translator.** Mia writes all of this as code, in a
programming language. A translator (a compiler or an interpreter)
changes that code into signals only her laptop's chip can run. Only
then does the CPU (Week 4) actually carry out the plan.

Together, sequence, loop, and decision — plus a translator — take Mia
from "I want my photos renamed nicely" to a program that actually does
it, 200 times, correctly.

---

## 3. Optional Reading: More Detail

This section holds extra detail that was trimmed from the slides. It
is optional, but useful if you want to go deeper.

**Why so many languages exist.** No single language does every job
best. Python is easy to learn and popular for data and quick tasks.
JavaScript runs inside web pages, in your browser. C controls hardware
directly and is very fast, close to the chip. Swift builds apps for
iPhones and iPads. Java runs large business and Android apps. SQL asks
questions of a database (Week 11). Every one of these languages still
follows the same idea underneath: exact rules, exact steps.

**A short history.** In the 1940s, early computers were programmed by
rewiring cables and switches, by hand. In the late 1940s, short number
codes replaced some of that rewiring, but were still very hard to
read. In 1957, FORTRAN let people write steps using words and math,
much closer to plain language. Each step in this history made
instructions easier for a person to write, and to read again later.

**Compiler vs. interpreter, a little more precisely.** A compiler
reads all of a program's code first, translates it completely, and
only then lets the chip run it. An interpreter instead reads and
translates one line at a time, running each line as it goes. Both are
translators; they just do the translation work at a different time.

**Why this matters in industry.** Most tech job listings ask for at
least one programming language. Coding interviews test this exact
skill: can a candidate turn a plain request into exact, ordered steps,
the same way Mia's photo plan does.

---

## 4. Practice Problems (with Answers)

Try each problem yourself before checking the answer.

**Problem 1.** In your own words, what is a programming language?

> **Answer:** A set of exact rules for writing instructions a computer
> can follow, one step at a time.

**Problem 2.** Name the three basic building blocks of any program.

> **Answer:** Sequence, loop, and decision.

**Problem 3.** A program prints "Good morning" 50 times, once for each
student. Which building block does this need most: sequence, loop, or
decision?

> **Answer:** Loop. The same step (print "Good morning") repeats 50
> times.

**Problem 4.** A program checks a photo's name. If the name is already
used, it skips the photo. Otherwise, it renames the photo. Which
building block is this?

> **Answer:** Decision. The program picks between two paths: skip or
> rename.

**Problem 5.** True or false: "A compiler and an interpreter both
translate code, but at different times." Explain your answer in one
sentence.

> **Answer:** True. A compiler translates all the code first, before
> running; an interpreter translates one line at a time, while
> running.

**Problem 6.** Put these three steps in the correct sequence order for
renaming one photo: "write its new name," "open the photo file," "read
its old name."

> **Answer:** Open the photo file → read its old name → write its new
> name.
