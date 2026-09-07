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
Yushintia Pramitarini, Ph.D · Dept. of Intelligent Computing · Thu [1-3] · Seongpa Hall 701
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

<div class="cardlist">
<div class="card"><div class="h">Memory vs. Storage</div><div class="d">Explain the difference between memory (RAM) and storage.</div></div>
<div class="card"><div class="h">Unsaved Work</div><div class="d">Say why unsaved work disappears when the power stops.</div></div>
<div class="card"><div class="h">Storage Types</div><div class="d">Name common kinds of storage, like SSD and HDD.</div></div>
<div class="card"><div class="h">Tracing Save</div><div class="d">Trace what happens inside a laptop when you click Save.</div></div>
</div>

---

<!-- Key Words Today, session 1 -->

# Key Words Today

- **Memory (RAM)** — space that holds data only while a program runs.
- **Storage** — space that keeps data even when the power is off.
- **Volatile** — loses its data as soon as power stops.
- **Save** — copy data from memory into storage.

<!-- notes: Read each word aloud. Ask students to repeat it once. -->

---

<!-- Try-It preview, closes session 1 -->

# Coming Up: Worksheet Part A

<div class="thread">Next, you will sort real examples.</div>

- In **[Worksheet Part A](materials/week05/worksheet.html)**, you sort data as memory, storage, or both.
- Example: "An open, unsaved document." Which one is that?
- You will work with a partner. A guess is fine for now.

<!-- notes: Tell students to sit next to a partner for the next part. No prep needed. -->

---

<!-- Key Words Today, session 2 -->

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

# Why One Kind of Memory Is Never Enough

<div class="thread">The stack above hides a hard trade-off. Here it is, in plain words.</div>

- The fastest memory technology is tiny, and expensive to make bigger.
- The cheapest, biggest storage technology is slow to read and write.
- No single technology is fast, huge, cheap, and permanent, all at once.

Real computers solve this by stacking several kinds of memory together,
fastest and smallest closest to the CPU, slowest and biggest farthest away.

---

# The Memory Hierarchy: Four Rungs

<div class="thread">Four different tools, each doing a different job.</div>

- **Registers** — tiny storage built directly into the CPU chip; holds the exact value the CPU is using this instant.
- **Cache** — a small, very fast memory next to the CPU; holds copies of data the CPU used recently.
- **RAM (Memory)** — holds the whole running program and its data.
- **Secondary storage** — keeps everything permanently, even powered off.

---

# Diagram: The Memory Hierarchy Ladder

<div class="thread">Follow one request as it climbs down the ladder.</div>

<div class="pipeline">
<div class="stage"><div class="h">Registers</div><div class="s">fastest, a few bytes, inside the CPU</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Cache</div><div class="s">very fast, a few MB, next to the CPU</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">RAM</div><div class="s">fast, several GB, on the motherboard</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Secondary Storage</div><div class="s">slower, huge, permanent</div></div>
</div>

Each step down trades speed for size: bigger and cheaper, but slower to reach.

---

# Case Study: Tracing Minjun's Laptop, Right Now

<div class="thread">All four rungs, working at once, inside one ordinary laptop.</div>

- A loop counter inside his word processor's code sits in a **register**.
- A webpage he just reloaded appears instantly from **cache**.
- His open, unsaved essay text sits in **RAM**.
- His already-saved photos from last weekend sit on his **SSD**.

All four are active at the same moment, each holding a different kind of data.

---

# Speed, Size, and Cost Across the Ladder

| Rung | Speed | Typical Size | Cost per Byte |
|---|---|---|---|
| Registers | Fastest | A few bytes | Highest |
| Cache | Very fast | A few MB | Very high |
| RAM | Fast | Several GB | Medium |
| Secondary storage | Slowest | TB-scale | Lowest |

*Values are rounded for teaching purposes, not exact hardware specifications.*

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

# RAM vs ROM: Two Different Jobs

<div class="thread">Both live inside a laptop. They do opposite jobs.</div>

- **RAM (Random Access Memory)** — fast, volatile working memory. It holds whatever program you are running right now, and can be rewritten constantly.
- **ROM (Read-Only Memory)** — non-volatile memory. It holds fixed instructions written once, at the factory, and is rarely or never rewritten afterward.

RAM changes every second you use your laptop. ROM barely ever changes at all.

---

# What Each One Actually Stores

<div class="thread">Same laptop, two very different kinds of content.</div>

- **RAM stores:** the operating system in use, every open app, and your document's in-progress data.
- **ROM stores:** the tiny startup program, called firmware, that runs the instant you press the power button, before the operating system has even loaded.

Without ROM's firmware, a laptop would not know how to start loading anything at all.

---

# Case Study: What Survives Minjun's Power Cut

<div class="thread">Back to the essay that vanished. Now widen the picture.</div>

- **His essay, in RAM:** gone completely. RAM is volatile.
- **His laptop's firmware, in ROM:** untouched. ROM is non-volatile.

That is exactly why, after he plugs his laptop back in, it still knows
how to turn on and start loading the operating system again, even
though his essay did not survive.

---

# Common Confusion: Isn't Storage the Same as ROM?

<div class="thread">Both keep data with no power. That is where the similarity ends.</div>

- **ROM** is small, fixed at the factory, and almost never rewritten by a user.
- **Secondary storage (HDD/SSD)** is large, and meant to be rewritten constantly, every time you save a file.

Both are non-volatile. Only one of them is meant for your everyday files.

---

# Why Cache Exists

<div class="thread">Week 4's CPU is faster than this week's RAM can keep up with.</div>

The CPU can execute billions of instructions every second, but RAM
cannot supply new data anywhere near that fast. This growing speed gap
would leave the CPU waiting constantly. **Cache** is a small, extremely
fast memory placed between the CPU and RAM to close that gap.

---

# Cache Memory: Definition

<div class="thread">One clear definition, one clear job.</div>

> **Cache memory** is a small, very fast memory that stores copies of
> the data or instructions the CPU is most likely to need again soon,
> so the CPU rarely has to wait on slower RAM.

Cache does not replace RAM. It sits in front of RAM, catching the CPU's
most common requests before they ever reach it.

---

# Hit or Miss?

<div class="thread">Every single request to cache ends one of two ways.</div>

- **Cache hit:** the CPU asks for data, and it is already sitting in cache. The CPU gets it almost instantly.
- **Cache miss:** the data is not in cache. The CPU must wait for RAM, which is much slower, and a copy is then stored in cache for next time.

A high hit rate is what actually makes a computer feel fast.

---

# Case Study: Reopening the Same Browser Tab

<div class="thread">Same action, twice. Two very different speeds.</div>

- **First time Minjun opens a tab:** cache miss. Nothing is cached yet, so the browser must load everything from RAM and storage. It feels a little slow.
- **He closes it, then reopens it seconds later:** cache hit. The same data is still sitting in cache, so it appears almost instantly.

---

# How Much Do Hits Actually Save?

<div class="thread">A small example, with real numbers.</div>

Suppose a cache hit takes about **1 nanosecond**, and a cache miss takes
about **100 nanoseconds**. If 9 out of every 10 requests are hits:

(9 × 1 ns + 1 × 100 ns) ÷ 10 requests ≈ **10.9 ns average**

That average sits far closer to the hit speed than the miss speed. This
is exactly why designers work hard to keep the hit rate high.

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

# HDD vs SSD: Two Different Technologies

<div class="thread">Both are secondary storage. They store data in completely different ways.</div>

- **HDD (Hard Disk Drive)** — magnetic storage. Data is written as magnetized spots on a spinning metal disk, called a platter.
- **SSD (Solid-State Drive)** — flash storage. Data is written directly into memory chips, with no spinning parts at all.

---

# How Each One Actually Works

<div class="thread">One has moving parts. The other has none.</div>

- **HDD:** a motor spins the platter thousands of times a minute; a moving arm swings to the right spot to read or write, much like a tiny record player.
- **SSD:** an electrical signal reads or writes transistors directly, like flipping switches, with nothing to spin up or move into place.

That single difference is why SSDs are faster, quieter, and tougher when dropped.

---

# Capacity vs Speed, Roughly

<div class="thread">Rough, illustrative comparison, not exact benchmark numbers.</div>

<div class="barchart">
<div class="bar-row">
  <div class="bar-label">HDD — Typical Speed</div>
  <div class="bar-track"><div class="bar-fill risk-high" style="width: 25%"></div></div>
  <div class="bar-value">slower to read/write</div>
</div>
<div class="bar-row">
  <div class="bar-label">SSD — Typical Speed</div>
  <div class="bar-track"><div class="bar-fill risk-low" style="width: 90%"></div></div>
  <div class="bar-value">much faster to read/write</div>
</div>
<div class="bar-row">
  <div class="bar-label">HDD — Cost per GB</div>
  <div class="bar-track"><div class="bar-fill risk-low" style="width: 85%"></div></div>
  <div class="bar-value">cheaper for the same size</div>
</div>
<div class="bar-row">
  <div class="bar-label">SSD — Cost per GB</div>
  <div class="bar-track"><div class="bar-fill risk-high" style="width: 35%"></div></div>
  <div class="bar-value">pricier for the same size</div>
</div>
</div>

*Bar lengths are teaching approximations, not measured benchmark results.*

---

# Case Study: Minjun Upgrades His Laptop

<div class="thread">One decision, two different storage needs.</div>

- He wants his operating system and apps to open quickly: he chooses an **SSD** as his main drive.
- He also has years of old family photos he rarely opens: he adds a large, cheap **external HDD** just to archive them.

One laptop, two storage technologies, each doing the job it is best at.

---

# Why HDDs Haven't Disappeared

<div class="thread">If SSDs are faster, why does anyone still buy a spinning disk?</div>

Even though SSDs are faster, HDDs still cost far less per gigabyte for
very large amounts of data. That is why HDDs remain common for backups,
archives, and the huge data centers behind cloud storage.

---

# The Smallest Units: Bit and Byte

<div class="thread">Every number in this course eventually reduces to these two units.</div>

- **Bit** — a single `1` or `0`. The smallest possible unit of data (recall Week 3's Boolean logic).
- **Byte** — a group of 8 bits. The basic unit computers use to measure most everyday data.

One typed letter of text takes up roughly one byte.

---

# Scaling Up: KB, MB, GB, TB

<div class="thread">Same idea, bigger and bigger groups of bytes.</div>

| Unit | Roughly Holds |
|---|---|
| Kilobyte (KB) | A short paragraph of text |
| Megabyte (MB) | One photo |
| Gigabyte (GB) | A short movie |
| Terabyte (TB) | Thousands of movies |

Each step up is about a thousand times bigger than the step before it.

---

# Powers of 2 vs Powers of 10

<div class="thread">The same word, "kilobyte," secretly means two slightly different numbers.</div>

- Computers naturally count in binary, so memory sizes are technically **powers of 2**: 1 KB = 1,024 bytes.
- Storage is usually advertised using **powers of 10**, because it produces bigger, rounder-looking numbers: 1 KB = 1,000 bytes.

Neither convention is "wrong." They are just two different counting systems, used in two different places.

---

# Why Your "256GB" Drive Shows Less Than 256GB

<div class="thread">A very common, very confusing moment for every new laptop owner.</div>

- **Manufacturer's 256 GB** uses powers of 10: 256 × 10⁹ bytes = 256,000,000,000 bytes.
- **Your operating system** reports storage using powers of 2 (1 "GB" = 2³⁰ bytes), so that exact same drive shows as roughly **238 GB** in your file explorer.

No data is missing. It is the same bytes, counted two different ways.

---

# Clock Speed, Revisited

<div class="thread">Week 4 introduced this number. This week asks what it can, and cannot, tell you.</div>

**Clock speed**, measured in gigahertz (GHz), is how many basic timing
cycles the CPU can execute every second. A higher clock speed lets the
CPU do more work per second, but it says nothing about how fast memory
or storage can keep up with it.

---

# Access Time: How Long Until the First Byte Arrives

<div class="thread">The first of two very different performance numbers.</div>

> **Access time** is how long a memory or storage device takes to
> locate a requested piece of data, and begin delivering it.

Access time ranges from a fraction of a nanosecond for registers, up to
several milliseconds for a spinning hard disk drive.

---

# Throughput: How Much Data Flows, Once It's Moving

<div class="thread">The second performance number, measuring something different.</div>

> **Throughput** is how much data a device can transfer per second,
> once the transfer has already started, usually measured in MB/s or GB/s.

Access time is how long you wait to merge onto a highway. Throughput is
how fast traffic moves once you are already on it. They are not the same number.

---

# Access Time Across the Whole Ladder

<div class="thread">The hierarchy from earlier, now with real performance numbers attached.</div>

| Rung | Rough Access Time |
|---|---|
| Registers | Under 1 nanosecond |
| Cache | A few nanoseconds |
| RAM | Tens of nanoseconds |
| SSD | Tens of microseconds |
| HDD | Several milliseconds |

*Figures are rounded, illustrative orders of magnitude, not exact specifications.*

---

# Case Study: Copying Minjun's Photos to a USB Drive

<div class="thread">Clock speed, access time, and throughput, all in one everyday action.</div>

- His CPU's **clock speed** issues the copy instructions almost instantly.
- The USB drive's **access time** causes a brief pause before any data starts moving at all.
- The USB drive's **throughput** then decides how many minutes the whole folder actually takes to finish copying.

Three different numbers, three different jobs, inside one simple file copy.

---

# Speed Isn't Everything: A Quick Reality Check

<div class="thread">A few beliefs students bring in that this week should correct.</div>

- **"A higher GHz laptop is always faster overall":** Not necessarily. Slow storage or too little RAM can bottleneck even a fast CPU.
- **"Throughput and access time are the same thing":** Wrong. A device can be slow to start (poor access time) but fast once moving (good throughput), or the reverse.
- **"The SSD speed on the box is what I'll always get":** Real-world speed also depends on file size, how full the drive already is, and what else is running.

---

<!-- Try-It hand-off, Worksheet Part A -->

# Try It: Worksheet Part A

<div class="thread">Now you practice. Work with a partner.</div>

- Open **[Worksheet Part A](materials/week05/worksheet.html)**.
- Sort each example: memory, storage, or both.
- You have about 15 minutes. Ask your partner before you ask me.

<!-- notes: Hand out Worksheet Part A. Walk around and help pairs. After 15 minutes, ask 2-3 pairs to share one answer. -->

---

<!-- Key Words Today, session 3 -->

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
