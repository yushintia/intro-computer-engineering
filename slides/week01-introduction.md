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
notes: Ask everyone to take out their phone or laptop. Ask: "can anyone
explain, in one sentence, what actually happens inside this when you tap
an app icon?" Let the silence be the hook.
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

<!-- notes: Point out the arc: one device, opened layer by layer, all semester. -->

---

<!-- SLOT 3: What you already bring -->

# What You Already Bring

No formal prerequisite is required for this course, and that is by
design:

- **Years of using devices**: phones, laptops, game consoles. You are already an expert user, just not yet an expert in how they work
- **Everyday troubleshooting instinct**: you already restart devices, close apps, check your signal bars. Those habits are early, informal versions of ideas this course makes precise
- **Curiosity**: the only real requirement. Everything technical starts from zero this semester

This course does not assume you have ever written a line of code or
opened a computer's case. By the end, you will have done both, at least
conceptually.

---

<!-- Course logistics appendix -->

<!-- _class: section -->

# Course Logistics
<div class="driving-q">Read once now, referenced all semester.</div>

---

# Grading & Materials

| Item | Weight |
|---|---|
| Attendance | 10% |
| Midterm | 30% |
| Final | 30% |
| Assignments | 10% |
| In-class items | 20% |

<!-- notes: Assignment 1 due Week 4 (CPU & Instructions). Assignment 2 due Week 11 (Databases & Security). Quiz 1 Week 6 (Application Software), Quiz 2 Week 13 (AI). -->

---

# Textbook, Policy & Contact

- **Textbook:** Harris & Harris, *Digital Design and Computer Architecture* (RISC-V ed.), Morgan Kaufmann, 2021
- **Reference:** Tanenbaum & Austin, *Structured Computer Organization*, 6th ed., Pearson, 2012
- **Policy:** attend and participate every class; late assignments are penalized; plagiarism and cheating lead to disciplinary action
- **Contact:** yushintia@deu.ac.kr, office hours by email appointment

---

<!-- SLOT 4: The pain (Act 1 / MOTIVATE), zero jargon -->

# The Call That Froze

<div class="pain">

Four students are mid-way through a group project video call, screen
shared, everyone talking over each other about the slides. Without
warning, one student's screen freezes. Her camera stops, her voice cuts
out, and a small spinning circle appears where her face used to be.

Everyone reacts the same way: "restart it." She does, and thirty seconds
later she is back, apologizing, with no idea what actually happened.
Nobody on the call, including her, can explain what just froze, why
restarting fixed it, or what "it" even refers to: her phone, the app,
the internet, or all three.

</div>

<!-- notes: Do not use the word "computer engineering" yet. Let the shrug sit uncomfortably first. -->

---

# "Just Restart It" Is Not an Explanation

<div class="barchart">
<div class="bar-row">
  <div class="bar-label">What she can explain</div>
  <div class="bar-track"><div class="bar-fill short" style="width: 8%"></div></div>
  <div class="bar-value">"it froze, then it didn't"</div>
</div>
<div class="bar-row">
  <div class="bar-label">What actually happened, layer by layer</div>
  <div class="bar-track"><div class="bar-fill long" style="width: 100%"></div></div>
  <div class="bar-value">hardware, software, and network, all at once</div>
</div>
</div>

That gap between "it froze" and a real explanation is not a small one.
Closing it, one layer at a time, is this entire course.

<!-- notes: Let the size difference between the two bars sit for a second. -->

---

<!-- SLOT 5: Cost of not knowing -->

# What Else This Actually Costs

- A frozen device during an interview, a live demo, or an exam becomes a crisis instead of a two-minute fix, because nobody can diagnose it
- A team choosing tools for a project (which app, which service, which device) makes an expensive guess instead of an informed decision
- A graduate who cannot explain "what happens when you tap an icon" struggles in almost every later course in this major, which all assume this picture

<div class="why">
<strong>In industry:</strong> "walk me through what happens when you type
a URL and press enter" is one of the most common opening interview
questions in the entire tech industry, precisely because it tests this
whole-system view, not any single narrow skill.
</div>

---

# One Small Freeze, Many Possible Layers

<div class="appgrid">
<div class="app"><div class="name">Hardware layer</div><div class="desc">did a chip overheat, or run out of memory?</div></div>
<div class="app"><div class="name">Software layer</div><div class="desc">did the video-call app itself crash?</div></div>
<div class="app"><div class="name">Operating system layer</div><div class="desc">did the OS fail to share resources fairly?</div></div>
<div class="app"><div class="name">Network layer</div><div class="desc">did the internet connection simply drop?</div></div>
</div>

Any one of these four, alone, can cause the exact same frozen screen.
Without a map of the layers, there is no way to even guess correctly.

---

<!-- SLOT 6: Driving question -->

<!-- _class: section -->

# This Week's Question

<div class="driving-q">"What's actually inside the device in your hand, and how do its pieces fit together?"</div>

---

<!-- SLOT 7: Learning outcomes -->

# By the End of This Week, You Can

1. Name the major hardware and software layers inside any modern computer
2. Explain, in plain language, roughly what happens when you tap an app icon
3. Describe how this semester's fourteen remaining topics map onto those layers
4. State this course's five official teaching objectives and where each is covered

---

# This Course's Five Objectives

<div class="thread">Not just this week's goals. This is what the syllabus commits this whole course to.</div>

| # | Objective (from the syllabus) | Where |
|---|---|---|
| 1 | Explain the basic structure and operating principles of hardware and software | Previewed today, all semester |
| 2 | Understand how data and instructions are represented and processed | Weeks 3-4 |
| 3 | Describe the roles of system software, operating systems, and networks | Weeks 6-7, 9 |
| 4 | Survey computing fields, including databases, security, and multimedia | Weeks 11-12 |
| 5 | Introduce future technologies: AI, IoT, cloud, big data, mobile | Weeks 13-14 |

---

<!-- _class: section -->

# End of 차시 1
<div class="driving-q">Short break. 차시 2 starts with: what a "computer," precisely, even is.</div>

---

<!-- SLOT 8: Origin -->

# This Field Is Younger Than You Might Think

<div class="thread">You just felt the pain. Now: where did the idea of studying this, as its own field, come from?</div>

- **Through the 1960s:** building computers was electrical engineering, and writing programs for them was an entirely separate discipline, computer science, with little formal overlap between the two
- **1970s onward:** as computers became something every engineer needed to understand from both the hardware and the software side, "computer engineering" emerged as its own field, deliberately built at the seam between the two

<div class="why">
This course exists because of that same seam. A frozen video call cannot
be explained by hardware knowledge alone, or software knowledge alone.
It takes both, together, which is exactly this major's reason for
existing.
</div>

---

<!-- SLOT 9: Core concept -->

# Computer System: Definition

<div class="thread">One seam, one precise definition of what actually sits on top of it.</div>

> A **computer system** is the combination of **hardware** (the physical
> components that store and process information) and **software** (the
> instructions that tell hardware what to do), working together to
> process information.

- **Hardware:** the CPU, memory, storage, and input/output devices, the physical device you can hold
- **Software:** everything from the operating system to the video-call app itself, none of it physical, all of it stored as data on the hardware

Neither half does anything useful alone. A phone with no software is an
expensive paperweight; software with no hardware to run on does not
exist at all.

---

<!-- Act 3 / BUILD -->

# From an App Icon to the Physical Chip

<div class="thread">One definition, six concrete layers. This is the map for the whole semester.</div>

<div class="stack">
<div class="layer view"><span class="h">Application Software</span> <span class="s">the video-call app, KakaoTalk, a game: Week 6</span></div>
<div class="layer view"><span class="h">System Software / OS</span> <span class="s">shares the machine fairly between apps: Week 7</span></div>
<div class="layer logical"><span class="h">Programs &amp; Instructions</span> <span class="s">written in a programming language: Week 10</span></div>
<div class="layer logical"><span class="h">CPU</span> <span class="s">executes those instructions, one at a time, very fast: Week 4</span></div>
<div class="layer physical"><span class="h">Memory &amp; Storage</span> <span class="s">holds data and programs, briefly or permanently: Week 5</span></div>
<div class="layer physical"><span class="h">Logic Gates</span> <span class="s">tiny on/off switches, everything above is built from these: Week 3</span></div>
</div>

Every remaining week of this course zooms into exactly one of these six
layers, one at a time, from the bottom up.

---

# Demo, Step by Step: Tracing One Tap

<div class="thread">Six layers is abstract. Here is one real tap, walked through, layer by layer.</div>

**Step 1 of 4: You tap the video-call app's icon.**

The touchscreen (hardware, an input device) senses your finger and
sends a signal toward the operating system.

---

# Demo, Step by Step: Tracing One Tap

**Step 2 of 4: The operating system responds.**

The OS (Week 7) recognizes the tap, finds the app's program on storage,
and asks memory (Week 5) to make room for it while it runs.

---

# Demo, Step by Step: Tracing One Tap

**Step 3 of 4: The CPU takes over.**

The CPU (Week 4) reads the app's instructions from memory, one at a
time, executing each one: draw a button, check the camera, connect to
the network (Week 9).

---

# Demo, Step by Step: Tracing One Tap

**Step 4 of 4: You see the result.**

The screen (hardware, an output device) lights up the app's interface.
Everything in the frozen-call story two slides ago is one of these
exact four steps, going wrong somewhere in the chain.

---

# Case Study: Where the Freeze Actually Was

<div class="thread">The demo above is generic. Here is the frozen-call story, resolved with the vocabulary you just learned.</div>

Reframed with this week's layers, the original mystery has real,
answerable candidates instead of a shrug:

<div class="chip-row">
<span class="chip">CPU overloaded (Week 4)</span>
<span class="chip">Memory ran out (Week 5)</span>
<span class="chip">App itself crashed (Week 6)</span>
<span class="chip">Network connection dropped (Week 9)</span>
</div>

Restarting the device resets all four layers at once, which is exactly
why it so often "just works," without anyone needing to know which
layer actually failed.

---

# Who Actually Works at Each Layer

<div class="thread">Six layers, six kinds of jobs. This major touches all of them.</div>

<div class="appgrid">
<div class="app"><div class="name">Hardware engineer</div><div class="desc">designs the CPU, memory, and physical chips: bottom of the stack</div></div>
<div class="app"><div class="name">Systems / OS engineer</div><div class="desc">builds the software that shares one machine fairly</div></div>
<div class="app"><div class="name">Network engineer</div><div class="desc">keeps machines talking to each other reliably</div></div>
<div class="app"><div class="name">Application developer</div><div class="desc">builds the apps you actually tap and use</div></div>
<div class="app"><div class="name">Security analyst</div><div class="desc">protects every layer above from being misused</div></div>
<div class="app"><div class="name">AI / data engineer</div><div class="desc">builds the newest layer, Weeks 13-14's subject</div></div>
</div>

Every one of these roles exists because a real device, like the one that
froze on the call, has that many independent places something can go
wrong, and that many specialists trained to fix exactly one of them.

---

# Common Mistakes

- **"Hardware and software are unrelated fields":** neither does anything without the other, as the stack diagram just showed
- **"Computer engineering is just coding":** programming is one layer out of six; this course covers all of them
- **"You need to already know programming to start this major":** this course assumes zero prior experience, and Week 10 is where programming itself is introduced from scratch

---

# Check Yourself

1. Name one layer from today's stack that is hardware, and one that is software.
2. A friend's laptop is frozen. Using today's vocabulary, name two different layers that could each independently explain it.
3. Which role from the previous slide would you go to first if a video-call app itself, specifically, kept crashing, not the whole device?

---

# Answers

1. Hardware: CPU, memory, storage, or an input/output device. Software: the operating system, or any application.
2. Any two of: **CPU** overloaded, **memory** exhausted, the **application software** itself crashed, or the **network** connection dropped.
3. The **application developer**: the app itself is the layer at fault, not the hardware, OS, or network beneath it.

---

<!-- SLOT 14: Limits (Act 4 / CLOSE), becomes Week 2 slot 4 -->

# What Today's Map Cannot Do Yet

<div class="limits">
We now have a six-layer map of any computer system, and the vocabulary
to reason about it. But we still have no idea where any of this
actually started: who built the first computer, why, and how the field
grew from room-sized machines into the phone in your pocket. The map
exists; its history does not, yet.
</div>

---

<!-- SLOT 15: Bridge -->

# Next Week

Week 1 leaves **where all of this actually came from** unsolved. **Week
2, Computer History**, addresses it: the generations of computing
machines, how computers are classified, and the number systems that
make the whole stack from today possible.

---

<!-- SLOT 16: Summary -->

# Summary

- A computer system is hardware and software working together; neither does anything useful alone
- Six layers connect an app icon to a physical chip: application software, OS, programs, CPU, memory/storage, logic gates
- Every remaining week of this course studies exactly one of those six layers, from the bottom up
- **Reading:** Harris & Harris, Preface and Chapter 1
- **Prepare:** think of one moment your own device confused you, and bring it to Week 2

---

<!-- SLOT 17: Thank You -->
<!-- _class: end -->

# Thank You
