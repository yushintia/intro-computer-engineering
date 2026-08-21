---
marp: true
theme: shintia
paginate: true
footer: 'Department of Intelligent Computing'
---

<!-- SLOT 1: Title -->
<!-- _class: title -->

# Week 5: Memory & Storage

<span class="subtitle">Introduction to Computer Engineering (400507-001)</span>

<div class="meta">
Yushintia Pramitarini, Ph.D · Dept. of Intelligent Computing · Thu [1-3] · 성파 701
</div>

<!--
notes: Ask everyone to take out their phone or laptop again. Ask:
"What happens to an open, unsaved document if the battery dies right
now?" Let a few students guess. Do not confirm or correct yet.
-->

---

<!-- SLOT 2: Where we are -->

# Where We Are

<div class="roadmap">
<div class="wk"><div class="n">Wk 1</div><div class="t">Introduction</div></div>
<div class="wk"><div class="n">Wk 2</div><div class="t">Computer History</div></div>
<div class="wk"><div class="n">Wk 3</div><div class="t">Boolean Logic</div></div>
<div class="wk"><div class="n">Wk 4</div><div class="t">CPU &amp; Instructions</div></div>
<div class="wk now"><div class="n">Wk 5</div><div class="t">Memory &amp; Storage</div></div>
<div class="wk"><div class="n">Wk 6</div><div class="t">Application Software · Quiz 1</div></div>
<div class="wk"><div class="n">Wk 7</div><div class="t">Operating Systems</div></div>
<div class="wk review"><div class="n">Wk 8</div><div class="t">Midterm Exam</div></div>
<div class="wk"><div class="n">Wk 9</div><div class="t">Computer &amp; Internet</div></div>
<div class="wk"><div class="n">Wk 10</div><div class="t">Programming Language</div></div>
<div class="wk"><div class="n">Wk 11</div><div class="t">Databases &amp; Security</div></div>
<div class="wk"><div class="n">Wk 12</div><div class="t">Computer Applications</div></div>
<div class="wk"><div class="n">Wk 13</div><div class="t">AI · Quiz 2</div></div>
<div class="wk"><div class="n">Wk 14</div><div class="t">Emerging Technologies</div></div>
<div class="wk review"><div class="n">Wk 15</div><div class="t">Final Exam</div></div>
</div>

<!-- notes: Point at the map. Say: "We are zooming into one more layer today: memory and storage." -->

---

<!-- SLOT 3: Recap + open wound -->

# Last Week, This Week

- **Last week delivered:** Week 4 showed how the CPU reads and runs program instructions.
- **Last week left broken:** The CPU executes instructions perfectly, but has nowhere permanent to keep anything once the power goes off.

---

<!-- SLOT 4: The pain (Act 1 / MOTIVATE), zero jargon -->

# Two Hours, Gone in One Second

<div class="pain">

Minjun writes a long essay for two hours. He does not save it yet.

His laptop battery suddenly dies. The screen goes black.

He plugs it in and turns it back on. He opens his essay again.

It is empty. Every word he wrote is gone.

</div>

<!-- notes: Ask: "Has this happened to you?" Let two or three students answer. Do not explain why yet. -->

---

<!-- SLOT 5: Cost of not knowing -->

# What This Actually Costs

- Losing hours of work wastes real time and real effort.
- A company can lose important files with no working backup.
- Every tech job expects you to know why unsaved work disappears.

<div class="why">
<strong>In industry:</strong> "Why did we lose that data after the
crash?" is a real question engineers must be able to answer.
</div>

---

# What Survives a Restart?

<div class="appgrid">
<div class="app"><div class="name">Unsaved typing</div><div class="desc">Gone. It lived only in temporary memory.</div></div>
<div class="app"><div class="name">A saved photo</div><div class="desc">Stays. It lives in permanent storage.</div></div>
<div class="app"><div class="name">An installed app</div><div class="desc">Stays. Apps are saved as files too.</div></div>
</div>

Restarting clears one kind of space, but not the other.

---

<!-- SLOT 6: Driving question -->

<!-- _class: section -->

# This Week's Question

<div class="driving-q">"Why does unsaved work disappear, but saved files survive a restart?"</div>

---

<!-- SLOT 7: Learning outcomes -->

# By the End of This Week, You Can

1. Explain the difference between memory (RAM) and storage.
2. Say why unsaved work disappears when the power stops.
3. Name common kinds of storage, like SSD and HDD.
4. Trace what happens inside a laptop when you click Save.

---

<!-- Key Words Today, 차시 1 -->

# Key Words Today

- **Memory (RAM)** — space that holds data only while a program runs.
- **Storage** — space that keeps data even when the power is off.
- **Volatile** — loses its data as soon as power stops.
- **Save** — copy data from memory into storage.

<!-- notes: Read each word aloud. Ask students to repeat it once. -->

---

<!-- Try-It preview, closes 차시 1 -->

# Coming Up: Worksheet Part A

<div class="thread">Next, you will sort real examples.</div>

- In **[Worksheet Part A](materials/week05/worksheet.html)**, you sort data as memory, storage, or both.
- Example: "An open, unsaved document." Which one is that?
- You will work with a partner. A guess is fine for now.

<!-- notes: Tell students to sit next to a partner for the next part. No prep needed. -->

---

<!-- _class: section -->

# End of 차시 1
<div class="driving-q">Short break. 차시 2: how memory and storage actually work.</div>

---

<!-- Key Words Today, 차시 2 -->

# Key Words Today

- **Non-volatile** — keeps its data even with no power.
- **Hard disk drive (HDD)** — older storage, uses a spinning disk.
- **Solid-state drive (SSD)** — newer storage, uses chips, no moving parts.
- **Byte** — a small unit that measures how much data fits.
- **Speed** — how fast a part can read or write data.

<!-- notes: Read each word aloud. Ask: "Which word did you not know before today?" -->

---

<!-- SLOT 8: Origin -->

# Where This Idea Came From

<div class="thread">You just felt the pain. Where did this split come from?</div>

- **1940s-50s:** early computers had fast memory, but no good permanent storage.
- **Punch cards** were permanent, but painfully slow to read.
- **1956:** IBM built the first hard disk drive. It was the size of a refrigerator.

<div class="why">
Engineers needed two different tools: one fast for working, one
permanent for keeping. That same split still shapes every device today.
</div>

---

<!-- SLOT 9: Core concept -->

# Memory vs Storage: Definition

<div class="thread">One split, one clear definition.</div>

> **Memory (RAM)** is fast, temporary space. It holds data only while
> a program runs. **Storage** is slower, permanent space. It keeps
> data even when the power is off.

- **Memory is volatile:** turn off the power, and its data disappears.
- **Storage is non-volatile:** turn off the power, and its data stays.

---

<!-- Act 3 / BUILD -->

# From CPU to Storage

<div class="thread">Last week's chip needs somewhere to keep its work.</div>

<div class="stack">
<div class="layer logical"><span class="h">CPU</span> <span class="s">runs instructions, needs data fast: Week 4</span></div>
<div class="layer view"><span class="h">Memory (RAM)</span> <span class="s">holds data while a program runs</span></div>
<div class="layer physical"><span class="h">Storage</span> <span class="s">keeps data even when the power is off</span></div>
</div>

The CPU talks to memory constantly. It talks to storage only sometimes.

---

# What RAM Does

- RAM holds the program and data a CPU is using right now.
- RAM is very fast. The CPU can read and write it instantly.
- RAM is small compared to storage, and often more expensive.
- RAM is volatile: it needs constant power to keep its data.

---

# What Storage Does

- Storage keeps your files: documents, photos, apps, and more.
- Storage is slower than RAM, but it does not need constant power.
- Storage is much bigger than RAM, and cheaper for the same amount of data.
- Storage is non-volatile: your files wait for you, even powered off.

---

# Fast vs Big: The Trade-off

<div class="barchart">
<div class="bar-row">
  <div class="bar-label">RAM (Memory)</div>
  <div class="bar-track"><div class="bar-fill risk-low" style="width: 95%"></div></div>
  <div class="bar-value">very fast, small, costly</div>
</div>
<div class="bar-row">
  <div class="bar-label">SSD (Storage)</div>
  <div class="bar-track"><div class="bar-fill risk-med" style="width: 55%"></div></div>
  <div class="bar-value">fast, medium size and cost</div>
</div>
<div class="bar-row">
  <div class="bar-label">HDD (Storage)</div>
  <div class="bar-track"><div class="bar-fill risk-high" style="width: 20%"></div></div>
  <div class="bar-value">slower, but big and cheap</div>
</div>
</div>

No single part is best at everything. Every device mixes all three.

---

# Kinds of Storage Today

<div class="appgrid">
<div class="app"><div class="name">HDD</div><div class="desc">A spinning disk. Cheap and big, but slower.</div></div>
<div class="app"><div class="name">SSD</div><div class="desc">Memory chips, no moving parts. Fast.</div></div>
<div class="app"><div class="name">USB drive</div><div class="desc">Small, portable storage you carry around.</div></div>
<div class="app"><div class="name">Cloud storage</div><div class="desc">Files kept on someone else's computer, online.</div></div>
</div>

---

<!-- Try-It hand-off, Worksheet Part A -->

# Try It: Worksheet Part A

<div class="thread">Now you practice. Work with a partner.</div>

- Open **[Worksheet Part A](materials/week05/worksheet.html)**.
- Sort each example: memory, storage, or both.
- You have about 15 minutes. Ask your partner before you ask me.

<!-- notes: Hand out Worksheet Part A. Walk around and help pairs. After 15 minutes, ask 2-3 pairs to share one answer. -->

---

<!-- _class: section -->

# End of 차시 2
<div class="driving-q">Short break. 차시 3: saving files, and common mistakes.</div>

---

<!-- Key Words Today, 차시 3 -->

# Key Words Today

- **Crash** — a program or device suddenly stops working.
- **Auto-save** — a feature that saves your work again and again.
- **Backup** — a second copy of a file, kept somewhere safe.
- **Restart** — turning a device off, then on again.

<!-- notes: Read each word aloud. Say: "You will see these words in Worksheet Part B." -->

---

<!-- SLOT N-2: Worked example -->

# Case Study: Saving Your Essay

<div class="thread">Back to Minjun. Now you have the words.</div>

**Step 1: Minjun types.**
Every word lives in memory (RAM) first, not storage yet.

**Step 2: Minjun clicks Save.**
The computer copies his words from memory into storage.

**Step 3: The power goes off.**
Memory empties completely. Storage keeps whatever was already saved.

If Minjun had clicked Save before the battery died, his essay would survive.

---

<!-- SLOT N-1: Common mistakes -->

# Common Mistakes

- **"Memory and storage are the same thing":** Wrong. One is fast and temporary; the other is slow and permanent.
- **"If I don't click Save, my file is still there":** Wrong. Unsaved work lives only in memory.
- **"Bigger storage means a faster computer":** Wrong. Size and speed are different things.

---

<!-- Try-It hand-off, Worksheet Part B -->

# Try It: Worksheet Part B

<div class="thread">More practice. New scenarios.</div>

- Open **[Worksheet Part B](materials/week05/worksheet.html)**.
- Decide what survives a restart, and what does not.
- You have about 15 minutes. Then we discuss answers together.

<!-- notes: Hand out Worksheet Part B. After 15 minutes, go through the answer key as a class. Ask for volunteers first. -->

---

<!-- SLOT N: Check yourself -->

# Check Yourself

1. Name one thing memory (RAM) does, and one thing storage does.
2. Your laptop's battery dies while you write an essay. What happens to your unsaved words? Why?
3. Which is faster: memory (RAM) or a hard disk drive (HDD)?

---

# Answers

1. Memory holds data while a program runs; storage keeps data with no power.
2. The unsaved words disappear. Memory is volatile; it loses data when power stops.
3. Memory (RAM) is faster than a hard disk drive.

---

<!-- Self-check quiz hand-off -->

# Self-Check Quiz

<div class="thread">One more check, on your own.</div>

- Take the **[Week 5 Quiz](materials/week05/quiz.html)** (5-8 short questions).
- This quiz is not graded. It just checks your understanding.
- About 10 minutes. Check your own answers at the end.

<!-- notes: Hand out the quiz. Give students 10 minutes. Then read the answer key aloud, or let students self-check. -->

---

<!-- SLOT N+1: Limits (Act 4 / CLOSE), becomes Week 6 slot 4 -->

# What Memory & Storage Cannot Do Yet

<div class="limits">
Data can now be kept and retrieved, but nothing yet turns it into
something a person can actually use. A saved file, by itself, is not
useful without a program that can open it and show it to you.
</div>

---

<!-- SLOT N+2: Bridge -->

# Next Week

Week 5 leaves **turning saved data into something usable** unsolved.
**Week 6, Application Software**, addresses it: the apps that open
and use your files.

---

<!-- SLOT N+3: Summary -->

# Summary

- Memory (RAM) is fast and temporary; storage is slower and permanent.
- Saving copies your work from memory into storage.
- HDD, SSD, USB drives, and cloud storage are all kinds of storage.
- **Reading:** Harris & Harris, chapter on memory systems.
- **Handout:** [materials/week05/handout.md](materials/week05/handout.html), glossary and the full case study
- **Prepare:** Think of one time you lost unsaved work. Bring it to Week 6.

---

<!-- SLOT N+4: Thank You -->
<!-- _class: end -->

# Thank You
