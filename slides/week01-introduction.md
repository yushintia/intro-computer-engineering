---
marp: true
theme: shintia
paginate: true
footer: 'Department of Intelligent Computing'
---

<!-- SLOT 1: Title -->
<!-- _class: title -->

# Week 1: Introduction

<span class="subtitle">Introduction to Computer Engineering (400507-001)</span>

<div class="meta">
Yushintia Pramitarini, Ph.D · Dept. of Intelligent Computing · Thu [1-3] · 성파 701
</div>

<!--
notes: Ask everyone to take out their phone or laptop. Ask out loud:
"What happens inside this when you tap an app icon?" Wait for answers.
It is OK if no one can answer yet. That is the point of today.
-->

---

<!-- SLOT 2: Where we are -->

# Where We Are

<div class="roadmap">
<div class="wk now"><div class="n">Wk 1</div><div class="t">Introduction</div></div>
<div class="wk"><div class="n">Wk 2</div><div class="t">Computer History</div></div>
<div class="wk"><div class="n">Wk 3</div><div class="t">Boolean Logic</div></div>
<div class="wk"><div class="n">Wk 4</div><div class="t">CPU &amp; Instructions</div></div>
<div class="wk"><div class="n">Wk 5</div><div class="t">Memory &amp; Storage</div></div>
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

<!-- notes: Point at the map. Say: "We open one device, layer by layer, all semester." -->

---

<!-- NEW: warm-up, right after slot 2 -->

# Before We Start

<div class="thread">Warm-up: 3 minutes. Work with the person next to you.</div>

- Take out your phone or laptop.
- Name three parts you already know. Example: screen, battery, app icon.
- Write down what each part does, in your own words.

<div class="why">
You already know more than you think. This course gives names to
things you already use every day.
</div>

<!--
notes: Give students 2-3 minutes. Walk around the room. Then ask the
whole class, one question at a time:
1. "What is one part of your phone you wrote down?"
2. "What does that part do?"
3. "Can you touch that part, or not?"
Do not correct answers yet. Just collect words on the board.
-->

---

<!-- SLOT 3: What you already bring -->

# What You Already Bring

No prerequisite is needed for this course. Here is why:

- **You already use devices.** Phones, laptops, game consoles. You are already an expert user.
- **You already troubleshoot.** You restart devices. You close apps. You check your signal. These are early versions of ideas in this course.
- **You are curious.** That is the only real requirement.

This course does not expect you to know how to code. By the end, you
will understand hardware and software, at least the basics.

---

<!-- Course logistics appendix -->

<!-- _class: section -->

# Course Logistics
<div class="driving-q">Read once now. Use all semester.</div>

---

# Grading & Materials

| Item | Weight |
|---|---|
| Attendance | 10% |
| Midterm | 30% |
| Final | 30% |
| Assignments | 10% |
| In-class items | 20% |

<!-- notes: Assignment 1 is due Week 4. Assignment 2 is due Week 11. Quiz 1 is Week 6. Quiz 2 is Week 13. -->

---

# Textbook, Policy & Contact

- **Textbook:** Harris & Harris, *Digital Design and Computer Architecture* (RISC-V ed.), 2021
- **Reference:** Tanenbaum & Austin, *Structured Computer Organization*, 6th ed.
- **Policy:** Come to every class. Late work loses points. Cheating is not allowed.
- **Contact:** yushintia@deu.ac.kr. Email me to book office hours.

---

<!-- SLOT 4: The pain (Act 1 / MOTIVATE), zero jargon -->

# The Call That Froze

<div class="pain">

Four students are on a video call. They share a screen. They talk
about their project.

Suddenly, one student's screen freezes. Her camera stops. Her voice
stops too.

"Just restart it," someone says. She does. Thirty seconds later, she
is back. But no one knows what just happened.

</div>

<!-- notes: Ask: "Has this happened to you?" Let two or three students answer. Do not explain the cause yet. -->

---

# "Restart It" Is Not an Explanation

<div class="barchart">
<div class="bar-row">
  <div class="bar-label">What she can explain</div>
  <div class="bar-track"><div class="bar-fill short" style="width: 8%"></div></div>
  <div class="bar-value">"it froze, then it worked"</div>
</div>
<div class="bar-row">
  <div class="bar-label">What really happened</div>
  <div class="bar-track"><div class="bar-fill long" style="width: 100%"></div></div>
  <div class="bar-value">many parts, working together</div>
</div>
</div>

This gap is big. This course closes it, step by step.

<!-- notes: Point at the two bars. Say: "See the size difference? That gap is what this course teaches." -->

---

<!-- SLOT 5: Cost of not knowing -->

# What This Costs You

- A frozen device in an interview or exam becomes a real problem, fast.
- A team picking the wrong tool wastes time and money.
- Later courses in this major all assume you understand this picture.

<div class="why">
<strong>In industry:</strong> "What happens when you tap an icon?" is a
common interview question. It tests if you understand the whole
system.
</div>

---

# One Freeze, Many Possible Causes

<div class="appgrid">
<div class="app"><div class="name">Hardware</div><div class="desc">Did a chip get too hot?</div></div>
<div class="app"><div class="name">Software</div><div class="desc">Did the app itself crash?</div></div>
<div class="app"><div class="name">Operating system</div><div class="desc">Did it fail to share resources?</div></div>
<div class="app"><div class="name">Network</div><div class="desc">Did the internet connection drop?</div></div>
</div>

Any one of these four can cause the exact same frozen screen.

---

<!-- SLOT 6: Driving question -->

<!-- _class: section -->

# This Week's Question

<div class="driving-q">"What is inside the device in your hand? How do its parts work together?"</div>

---

<!-- SLOT 7: Learning outcomes -->

# By the End of This Week, You Can

1. Name the main hardware and software parts inside a computer.
2. Explain, simply, what happens when you tap an app icon.
3. Show how this semester's topics connect to those parts.
4. State this course's five goals and where each is taught.

---

# This Course's Five Objectives

<div class="thread">Not just this week's goals. This is the whole course's promise.</div>

| # | Objective (from the syllabus) | Where |
|---|---|---|
| 1 | Explain basic hardware and software structure | All semester |
| 2 | Understand how data and instructions work | Weeks 3-4 |
| 3 | Describe system software, OS, and networks | Weeks 6-7, 9 |
| 4 | Survey databases, security, and multimedia | Weeks 11-12 |
| 5 | Introduce AI, IoT, cloud, and mobile tech | Weeks 13-14 |

---

<!-- NEW: Key Words Today, 차시 1 -->

# Key Words Today

- **Device** — a phone, laptop, or tablet you use.
- **Hardware** — the physical parts you can touch.
- **Software** — the instructions that tell hardware what to do.
- **App** — a software program you open, like a game.
- **Network** — the connection that lets devices talk to each other.

<!-- notes: Read each word aloud. Ask students to repeat it once. Ask: "Which of your warm-up words match these?" -->

---

<!-- NEW: Try-It preview, closes 차시 1 -->

# Coming Up: Worksheet Part A

<div class="thread">Next, you will practice using these words.</div>

- In **Worksheet Part A**, you label everyday problems by layer.
- Example: "My phone is hot." Which layer is that?
- You will work with a partner. A guess is fine for now.

<!-- notes: Tell students to sit next to a partner for the next part. No prep needed. -->

---

<!-- _class: section -->

# End of 차시 1
<div class="driving-q">Short break. 차시 2: what a computer system really is.</div>

---

<!-- NEW: Key Words Today, 차시 2 -->

# Key Words Today

- **Computer system** — hardware and software working together.
- **Operating system (OS)** — software that manages all apps and hardware.
- **CPU** — the chip that runs instructions. The "brain" of the device.
- **Memory** — space that holds data while an app is running.
- **Layer** — one level in a stack of parts working together.

<!-- notes: Read each word aloud. Ask: "Which word did you not know before today?" -->

---

<!-- SLOT 8: Origin -->

# This Field Is Younger Than You Think

<div class="thread">You just felt the pain. Where did this field come from?</div>

- **Before the 1970s:** building computers and writing programs were two separate fields.
- **1970s onward:** computers needed people who understood both sides. "Computer engineering" was born.

<div class="why">
This course exists for that reason. A frozen call needs both hardware
and software knowledge to explain. That is this major's whole point.
</div>

---

<!-- SLOT 9: Core concept -->

# Computer System: Definition

<div class="thread">One field, one clear definition.</div>

> A **computer system** is **hardware** (the physical parts) and
> **software** (the instructions), working together.

- **Hardware:** CPU, memory, storage, and screen. Parts you can touch.
- **Software:** the OS and apps. You cannot touch it. It is stored data.

A phone with no software does nothing. Software with no hardware
cannot run at all. Both are needed.

---

<!-- Act 3 / BUILD -->

# From an App Icon to the Chip (1/2)

<div class="thread">Six layers. Here is the top half: software.</div>

<div class="stack">
<div class="layer view"><span class="h">Application Software</span> <span class="s">the app you tap, like a game: Week 6</span></div>
<div class="layer view"><span class="h">System Software / OS</span> <span class="s">shares the device between apps: Week 7</span></div>
<div class="layer logical"><span class="h">Programs &amp; Instructions</span> <span class="s">written in a programming language: Week 10</span></div>
</div>

Every app is a program. Every program needs an OS to run.

---

# From an App Icon to the Chip (2/2)

<div class="thread">The bottom half: hardware.</div>

<div class="stack">
<div class="layer logical"><span class="h">CPU</span> <span class="s">runs instructions, very fast: Week 4</span></div>
<div class="layer physical"><span class="h">Memory &amp; Storage</span> <span class="s">holds data, short or long term: Week 5</span></div>
<div class="layer physical"><span class="h">Logic Gates</span> <span class="s">tiny on/off switches. Everything is built from these: Week 3</span></div>
</div>

This course studies each layer, one at a time, from the bottom up.

---

# Tracing One Tap (1/2)

<div class="thread">Six layers is abstract. Here is one real tap.</div>

**Step 1: You tap the app icon.**
The screen (hardware) senses your finger. It sends a signal to the OS.

**Step 2: The OS responds.**
The OS finds the app on storage. It asks memory to make room.

---

# Tracing One Tap (2/2)

**Step 3: The CPU takes over.**
The CPU reads the app's instructions. It runs them, one at a time.

**Step 4: You see the result.**
The screen lights up the app. This is what happens when nothing breaks.

<!-- notes: Ask: "Which step do you think broke, in the frozen-call story?" -->

---

<!-- NEW: Try-It hand-off, Worksheet Part A -->

# Try It: Worksheet Part A

<div class="thread">Now you practice. Work with a partner.</div>

- Open **Worksheet Part A**.
- Label each scenario: hardware, software, OS, or network.
- You have about 15 minutes. Ask your partner before you ask me.

<!-- notes: Hand out Worksheet Part A. Walk around and help pairs. After 15 minutes, ask 2-3 pairs to share one answer. -->

---

<!-- _class: section -->

# End of 차시 2
<div class="driving-q">Short break. 차시 3: more practice, then a short quiz.</div>

---

<!-- NEW: Key Words Today, 차시 3 -->

# Key Words Today

- **Overheat** — a device gets too hot.
- **Crash** — an app suddenly stops working.
- **Wifi drop** — the network connection cuts out.
- **Diagnose** — figure out what is wrong.

<!-- notes: Read each word aloud. Say: "You will see these words in Worksheet Part B." -->

---

# Case Study: What Really Froze

<div class="thread">Back to the frozen call. Now you have the words.</div>

Here are four real possible causes:

<div class="chip-row">
<span class="chip">CPU overloaded</span>
<span class="chip">Memory ran out</span>
<span class="chip">App crashed</span>
<span class="chip">Network dropped</span>
</div>

Restarting resets all four layers at once. That is why it often works.

---

# Who Works at Each Layer

<div class="thread">Six layers, six kinds of jobs.</div>

<div class="appgrid">
<div class="app"><div class="name">Hardware engineer</div><div class="desc">Designs chips and memory.</div></div>
<div class="app"><div class="name">OS engineer</div><div class="desc">Builds software that shares the device.</div></div>
<div class="app"><div class="name">Network engineer</div><div class="desc">Keeps devices talking to each other.</div></div>
<div class="app"><div class="name">App developer</div><div class="desc">Builds the apps you use.</div></div>
<div class="app"><div class="name">Security analyst</div><div class="desc">Protects every layer from misuse.</div></div>
<div class="app"><div class="name">AI / data engineer</div><div class="desc">Builds the newest layer: Weeks 13-14.</div></div>
</div>

Each job exists because a real device can break in many ways.

---

# Common Mistakes

- **"Hardware and software are unrelated":** Wrong. Neither works without the other.
- **"Computer engineering is just coding":** Wrong. Coding is one layer of six.
- **"You must already know programming":** Wrong. This course starts from zero.

---

<!-- NEW: Try-It hand-off, Worksheet Part B -->

# Try It: Worksheet Part B

<div class="thread">More practice. New scenarios.</div>

- Open **Worksheet Part B**.
- Label each scenario the same way: hardware, software, OS, or network.
- You have about 15 minutes. Then we discuss answers together.

<!-- notes: Hand out Worksheet Part B. After 15 minutes, go through the answer key as a class. Ask for volunteers first. -->

---

# Check Yourself

1. Name one hardware part and one software part.
2. Your friend's laptop freezes. Name two layers that could cause it.
3. An app keeps crashing, not the whole device. Who do you ask first?

---

# Answers

1. Hardware: CPU, memory, storage, or screen. Software: the OS, or an app.
2. Any two: CPU overloaded, memory full, app crashed, or network dropped.
3. The **app developer**. The app itself is the problem, not the device.

---

<!-- NEW: Self-check quiz hand-off -->

# Self-Check Quiz

<div class="thread">One more check, on your own.</div>

- Take the **Week 1 Quiz** (5-8 short questions).
- This quiz is not graded. It just checks your understanding.
- About 10 minutes. Check your own answers at the end.

<!-- notes: Hand out the quiz. Give students 10 minutes. Then read the answer key aloud, or let students self-check. -->

---

<!-- SLOT 17: Limits (Act 4 / CLOSE), becomes Week 2 slot 4 -->

# What Today's Map Cannot Do Yet

<div class="limits">
We now have a map of computer layers, and some words for them. But we
do not know where any of this started. Who built the first computer?
Why? We have the map. We do not have its history yet.
</div>

---

<!-- SLOT 18: Bridge -->

# Next Week

Week 1 leaves **where this all started** unsolved. **Week 2, Computer
History**, answers it: how computers evolved, and the number systems
behind them.

---

<!-- SLOT 19: Summary -->

# Summary

- A computer system is hardware and software, working together.
- Six layers connect an app icon to a physical chip.
- Every later week studies one of those six layers.
- **Reading:** Harris & Harris, Preface and Chapter 1.
- **Prepare:** Think of one time your device confused you. Bring it to Week 2.

---

<!-- SLOT 20: Thank You -->
<!-- _class: end -->

# Thank You
