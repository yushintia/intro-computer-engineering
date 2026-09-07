---
marp: true
theme: shintia
paginate: true
footer: 'Department of Intelligent Computing'
---

<!-- SLOT 1: Title -->
<!-- _class: title -->

# Week 8: Midterm Review

<span class="subtitle">Introduction to Computer Engineering (400507-001)</span>

<div class="meta">
Yushintia Pramitarini, Ph.D · Dept. of Intelligent Computing · Thu [1-3] · Seongpa Hall 701
</div>

<!--
notes: Tell students this week has no new topic. Say: "Today we check
what you already know, from Week 1 to Week 7." Ask if anyone has
questions before you start.
-->

---

<!-- SLOT 2: Where we are (Act 0 / LOCATE) -->

# Where We Are

<div class="roadmap">
<div class="wk"><div class="n">Wk 1</div><div class="t">Introduction</div></div>
<div class="wk"><div class="n">Wk 2</div><div class="t">Computer History</div></div>
<div class="wk"><div class="n">Wk 3</div><div class="t">Boolean Logic</div></div>
<div class="wk"><div class="n">Wk 4</div><div class="t">CPU &amp; Instructions</div></div>
<div class="wk"><div class="n">Wk 5</div><div class="t">Memory &amp; Storage</div></div>
<div class="wk"><div class="n">Wk 6</div><div class="t">Application Software · Quiz 1</div></div>
<div class="wk"><div class="n">Wk 7</div><div class="t">Operating Systems</div></div>
<div class="wk now review"><div class="n">Wk 8</div><div class="t">Midterm Exam</div></div>
<div class="wk"><div class="n">Wk 9</div><div class="t">Computer &amp; Internet</div></div>
<div class="wk"><div class="n">Wk 10</div><div class="t">Programming Language</div></div>
<div class="wk"><div class="n">Wk 11</div><div class="t">Databases &amp; Security</div></div>
<div class="wk"><div class="n">Wk 12</div><div class="t">Computer Applications</div></div>
<div class="wk"><div class="n">Wk 13</div><div class="t">AI · Quiz 2</div></div>
<div class="wk"><div class="n">Wk 14</div><div class="t">Emerging Technologies</div></div>
<div class="wk review"><div class="n">Wk 15</div><div class="t">Final Exam</div></div>
</div>

<!-- notes: Point at Week 8. Say: "We stop here to look back, before we go on." -->

---

<!-- SLOT 3: Recap + open wound (Act 0 / LOCATE) -->

# Last Week, This Week

- **Last week delivered:** the OS shares one machine fairly between many running apps.
- **Last week left broken:** that machine is still alone. It cannot talk to any other machine yet.

<!-- notes: This gap is still open. Week 9 will close it, right after the midterm. -->

---

<!-- Act 3 / BUILD, entry point for the review variant -->
<!-- _class: section -->

# What You Should Now Know

<div class="driving-q">Seven weeks, one device: "What's Actually Inside Your Laptop."</div>

<!-- notes: Say: "We opened one laptop, layer by layer, for seven weeks. Today we put it back together." -->

---

# Week 1 Recap: Introduction

<div class="thread">"What is inside the device in your hand? How do its parts work together?"</div>

- **You can now:** name hardware parts and software parts in a device.
- **You can now:** explain what happens when you tap an app icon.

---

# Week 2 Recap: Computer History

<div class="thread">"How did computers evolve, and what number system works underneath them?"</div>

- **You can now:** put early computer generations in the right time order.
- **You can now:** convert a small decimal number into binary.

---

# Week 3 Recap: Boolean Logic

<div class="thread">"How do simple on/off switches let a computer decide true or false?"</div>

- **You can now:** read a truth table for an AND, OR, or NOT gate.
- **You can now:** combine simple gates to model one everyday decision.

---

# Week 4 Recap: CPU & Instructions

<div class="thread">How does a CPU turn one instruction into one action?</div>

- **You can now:** explain the fetch, decode, execute cycle in plain words.
- **You can now:** explain why a simple CPU runs one instruction at a time.

---

# Week 5 Recap: Memory & Storage

<div class="thread">Where does a computer keep data, while it runs and after power stops?</div>

- **You can now:** explain the difference between memory (RAM) and storage.
- **You can now:** explain why a device needs both, not just one.

---

# Week 6 Recap: Application Software

<div class="thread">What turns raw hardware into something a person can actually use?</div>

- **You can now:** give an example of application software and system software.
- **You can now:** explain how an app differs from the operating system.

---

# Week 7 Recap: Operating Systems

<div class="thread">How does one machine share itself fairly between many running programs?</div>

- **You can now:** explain what an operating system manages: apps, memory, hardware.
- **You can now:** explain why two apps do not simply fight over the CPU.

---

<!-- SLOT N: Check yourself (expanded review) -->
<!-- _class: section -->

# Check Yourself

<div class="driving-q">Ten questions. Weeks 1 through 7. Try each one before you read the answer.</div>

<!-- notes: Encourage students to answer out loud, or on paper, before you reveal each answer slide. -->

---

# Questions 1-2: Weeks 1-2

1. Name one hardware part and one software part of a laptop.
2. Put these in time order: transistors, vacuum tubes, integrated circuits.

---

# Answers 1-2

1. Hardware: CPU, memory, or screen. Software: the OS, or an app.
2. **Vacuum tubes → transistors → integrated circuits.**

---

# Questions 3-4: Week 3

3. An AND gate has inputs true and false. What is the output?
4. An OR gate has inputs false and true. What is the output?

---

# Answers 3-4

3. **False.** AND needs every input to be true.
4. **True.** OR needs only one true input.

---

# Questions 5-6: Week 4

5. Put these three steps in order: decode, execute, fetch.
6. True or false: a simple CPU runs many instructions at the exact same instant.

---

# Answers 5-6

5. **Fetch → decode → execute.**
6. **False.** A simple CPU runs one instruction at a time.

---

# Questions 7-8: Week 5

7. Which one keeps data with no power: memory or storage?
8. A laptop loses unsaved work after a power cut. What failed to keep it?

---

# Answers 7-8

7. **Storage** keeps data with no power. Memory needs power.
8. **Memory (RAM).** It only holds data while the power is on.

---

# Questions 9-10: Weeks 6-7

9. Give one example of application software, and one of system software.
10. Two apps are open at once. What decides which one uses the CPU right now?

---

# Answers 9-10

9. Application: a game or camera app. System: the operating system.
10. **The operating system.** It shares the CPU fairly between apps.

---

<!-- SLOT N+1: What to focus on next (replaces Limits, Act 4 / CLOSE) -->

# What to Focus On Next

<div class="limits">

<div class="cardlist">
<div class="card"><div class="h">Boolean logic (Week 3)</div><div class="d">Practice more AND/OR/NOT truth tables.</div></div>
<div class="card"><div class="h">CPU cycle (Week 4)</div><div class="d">Say fetch, decode, execute, in order, from memory.</div></div>
<div class="card"><div class="h">Memory vs. storage (Week 5)</div><div class="d">Know which one needs power to keep data.</div></div>
<div class="card"><div class="h">The six layers (Week 1)</div><div class="d">Review app icon → OS → CPU → gates.</div></div>
</div>

</div>

<!-- notes: Ask students which topic feels hardest. Spend extra time there if the room agrees. -->

---

<!-- SLOT N+2: Bridge (Act 4 / CLOSE) -->

# Next Week

Week 8 was review only. **Week 9, Computer & Internet**, starts new
content: how one machine finally talks to another.

---

<!-- SLOT N+3: Summary (Act 4 / CLOSE) -->

# Summary

- Weeks 1-7 built one full picture: a working, single computer.
- Today's ten questions covered every week on the midterm.
- **Reading:** re-read Weeks 1-7 handouts before the exam.
- **Prepare:** bring a pencil and your student ID to the midterm.

---

<!-- SLOT N+4: Thank You (Act 4 / CLOSE) -->
<!-- _class: end -->

# Thank You
