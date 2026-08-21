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
Yushintia Pramitarini, Ph.D · Dept. of Intelligent Computing · Thu [1-3] · 성파 701
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

1. Explain what a programming language is, in plain words.
2. Explain why computers need exact steps, not plain English.
3. Name the three basic building blocks of any program.
4. Turn one everyday task into a short list of steps.

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

<!-- NEW: Key Words Today, 차시 1 -->

# Key Words Today

- **Instruction** — one exact command a computer can follow.
- **Programming language** — a set of exact rules for writing instructions.
- **Syntax** — the exact grammar rules of a programming language.
- **Code** — instructions written in a programming language.
- **Programmer** — a person who writes code.

<!-- notes: Read each word aloud. Ask students to repeat it once. Ask: "Which word did you already know?" -->

---

<!-- NEW: Try-It preview, closes 차시 1 -->

# Coming Up: Worksheet Part A

<div class="thread">Next, you will practice using these words.</div>

- In **[Worksheet Part A](materials/week10/worksheet.html)**, you turn plain requests into ordered steps.
- Example: "Make my laptop say hello." What steps does that need?
- You will work with a partner. A guess is fine for now.

<!-- notes: Tell students to sit next to a partner for the next part. No prep needed. -->

---

<!-- _class: section -->

# End of 차시 1
<div class="driving-q">Short break. 차시 2: turning plain requests into exact steps.</div>

---

<!-- NEW: Key Words Today, 차시 2 -->

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

# Doing One Task Many Times

<div class="thread">Mia has 200 photos, not just one.</div>

- A **loop** repeats the same steps, again and again.
- Do the sequence once. Then do it again, for the next photo.
- 200 photos means 200 repeats. You only write the steps once.

---

<!-- NEW: Try-It hand-off, Worksheet Part A -->

# Try It: Worksheet Part A

<div class="thread">Now you practice. Work with a partner.</div>

- Open **[Worksheet Part A](materials/week10/worksheet.html)**.
- Turn each plain request into an ordered list of steps.
- You have about 15 minutes. Ask your partner before you ask me.

<!-- notes: Hand out Worksheet Part A. Walk around and help pairs. After 15 minutes, ask 2-3 pairs to share one answer. -->

---

<!-- _class: section -->

# End of 차시 2
<div class="driving-q">Short break. 차시 3: choices, translators, and many languages.</div>

---

<!-- NEW: Key Words Today, 차시 3 -->

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
