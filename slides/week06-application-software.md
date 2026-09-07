---
marp: true
theme: shintia
paginate: true
footer: 'Department of Intelligent Computing'
---

<!-- SLOT 1: Title -->
<!-- _class: title -->

# Week 6: Application Software

<span class="subtitle">Introduction to Computer Engineering (400507-001)</span>

<div class="meta">
Yushintia Pramitarini, Ph.D · Dept. of Intelligent Computing · Thu [1-3] · Seongpa Hall 701
</div>

<!--
notes: Ask everyone to look at their phone's home screen. Ask: "Which
icon did you tap most today?" Collect two or three answers. Say:
"Today we ask what that icon actually is." Also remind students:
"Quiz 1 is today, near the end of class."
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
<div class="wk now"><div class="n">Wk 6</div><div class="t">Application Software · Quiz 1</div></div>
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

<!-- notes: Point at Week 6. Say: "Today we zoom into the layer you touch the most: the app itself." -->

---

<!-- SLOT 3: Recap + open wound -->

# Last Week, This Week

- **Last week delivered:** we saw how memory and storage let a computer keep data and get it back later.
- **Last week left broken:** data can be kept and retrieved, but nothing yet turns it into something a person can actually use.

---

<!-- SLOT 4: The pain (Act 1 / MOTIVATE), ZERO jargon -->

# A Perfect Photo, Locked Away

<div class="pain">

You take a photo on your phone. It saves. You can find the file
later. It is kept safely, just like last week's lesson promised.

But imagine your phone had no photo app at all. No way to open that
file. No way to see the picture. No way to crop it, or send it to a
friend.

The file is still there, perfectly saved. But it is just data,
sitting still. It is not a photo yet, not to you. Something is
missing.

</div>

<!-- notes: Ask: "What is missing here? The data is safe, so what's the problem?" Let two students answer. Do not say "app" yet. -->

---

<!-- SLOT 5: Cost of not knowing -->

# What This Actually Costs

- Without this layer, you cannot write an essay, edit a photo, or send a message.
- Every job you will ever do uses application software, not raw stored data.
- Confusing "an app" with "the operating system" causes real mistakes in tech interviews.

<div class="why">
<strong>In industry:</strong> "App developer" is one of the most common
job titles in tech. Companies expect every graduate to know exactly
what application software does, and does not, do.
</div>

---

<!-- SLOT 6: Driving question -->

<!-- _class: section -->

# This Week's Question

<div class="driving-q">"What is application software, and how does it turn stored data into something you can use?"</div>

---

<!-- SLOT 7: Learning outcomes -->

# By the End of This Week, You Can

<div class="cardlist">
<div class="card"><div class="h">Application vs. System</div><div class="d">Define application software and tell it apart from system software.</div></div>
<div class="card"><div class="h">App Categories</div><div class="d">Name common categories of application software you use daily.</div></div>
<div class="card"><div class="h">Data to Usefulness</div><div class="d">Explain how an app turns stored data into something useful.</div></div>
<div class="card"><div class="h">Dependence on the OS</div><div class="d">Explain why every app still depends on the operating system.</div></div>
</div>

---

<!-- SLOT 8: Origin -->

# Where This Idea Came From

<div class="thread">You just felt the pain. Where did the answer come from?</div>

- **1950s-60s:** each computer ran one custom program, written by a specialist, for one single task.
- **1979:** *VisiCalc*, a spreadsheet program, let ordinary people use a computer for their own work.

<div class="why">
People called VisiCalc the first "killer app." It sold computers by
itself. It proved software could serve a normal user, not only an
expert.
</div>

---

<!-- SLOT 9: Core concept -->

# Application Software: Definition

<div class="thread">One idea, one clear definition.</div>

> **Application software** is a program that helps a user do one
> specific task, like writing, browsing, or editing photos.

- It is different from **system software** (the OS), which manages the computer itself.
- A photo app is application software. The operating system is not.

---

<!-- NEW: Key Words Today, session 1 -->

# Key Words Today

- **Application software (app)** — a program that helps you do one task.
- **System software** — software that manages the whole computer, like the OS.
- **Killer app** — an app so useful, people buy the device just for it.
- **User** — the person using an app to get something done.

<!-- notes: Read each word aloud. Ask students to repeat it once. Ask: "Which apps on your phone match this definition?" -->

---

<!-- NEW: Try-It preview, closes session 1 -->

# Coming Up: Worksheet Part A

<div class="thread">Next, you will practice using these words.</div>

- In **[Worksheet Part A](materials/week06/worksheet.html)**, you sort real programs into app or system software.
- Example: "a web browser" — is that an app, or system software?
- You will work with a partner. A guess is fine for now.

<!-- notes: Tell students to sit next to a partner for the next part. No prep needed. -->

---

<!-- NEW: Key Words Today, session 2 -->

# Key Words Today

- **Category** — a group of apps that do a similar kind of task.
- **Interface** — the screen and buttons an app shows to a user.
- **Request** — when an app asks the OS for something it needs.
- **Resource** — memory, storage, or CPU time an app needs to run.

<!-- notes: Read each word aloud. Say: "You will use all four words in the next slides." -->

---

<!-- Act 3 / BUILD -->

# What Is Software, Really?

<div class="thread">Before splitting software into types, nail down what it even is.</div>

> **Software** is the set of instructions and data a computer follows.
> **Hardware** is the physical machine that carries those instructions out.

- Software has no physical shape; it is code, sitting somewhere in memory or storage.
- Every layer this course has covered so far, logic gates, the CPU, memory, exists so software has something to run on.

---

# A Laptop With No Software At All

<div class="thread">Strip everything away. What is left?</div>

Imagine a brand-new laptop with every chip and drive installed, but
absolutely no software loaded onto it at all, not even firmware.

- The screen would never light up.
- The keyboard would never respond.
- Powerful hardware, completely useless, with nothing telling it what to do.

---

# Software vs Hardware: Quick Contrast

| | Hardware | Software |
|---|---|---|
| What it is | Physical parts (CPU, RAM, disk) | Instructions and data |
| Can you touch it? | Yes | No |
| Wears out how? | Physically, over years of use | Never wears out, but can become outdated |

---

# Software Needs Hardware, Hardware Needs Software

<div class="thread">Neither one is useful alone.</div>

- Hardware without software cannot do anything at all: it just sits there.
- Software without hardware has nowhere to run: it is only an idea.
- Every device you use is this exact partnership, working together.

---

# Application vs. System Software

<div class="thread">Back to the locked photo. What was actually missing?</div>

<div class="stack">
<div class="layer view"><span class="h">Application Software</span> <span class="s">does one task for you: a photo app, a browser, a game</span></div>
<div class="layer logical"><span class="h">System Software / OS</span> <span class="s">manages the whole machine: shares memory, storage, CPU: Week 7</span></div>
</div>

The photo file was safe. The app to open it was missing, not the OS.

---

# System Software vs Application Software: Full Definitions

<div class="thread">Two categories, doing two very different jobs.</div>

> **System software** manages the computer itself: the operating
> system, device drivers, and utility programs that keep the machine running.
> **Application software** helps a user do one specific task: writing,
> browsing, editing photos, playing a game.

- System software examples: Windows, macOS, a printer driver, a disk-cleanup utility.
- Application software examples: a word processor, a browser, a photo editor, a game.

---

# Utility Software: A Third Face of System Software

<div class="thread">Not every system program is the OS itself.</div>

- **Utility software** is system software that keeps the machine healthy, without being the OS.
- Examples: antivirus scanners, disk cleanup tools, file compression tools.
- Like the OS, utility software manages the machine. Unlike the OS, it usually runs only when you choose to run it.

---

# Same Task, Different Layer

<div class="thread">Watch one everyday action move between the two layers.</div>

<div class="pipeline">
<div class="stage"><div class="h">You click "Open"</div><div class="s">the app (application software) makes the request</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">OS finds the file</div><div class="s">system software locates it in storage</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">App displays it</div><div class="s">back to application software, showing the result</div></div>
</div>

One action, two layers, cooperating without you ever noticing the handoff.

---

# Worked Example: Sorting Minjun's Laptop Programs

<div class="thread">Real programs, sorted into their real layer.</div>

| Program | Layer |
|---|---|
| Windows | System software |
| Antivirus | System software (utility) |
| Web browser | Application software |
| Word processor | Application software |

Every icon on his desktop belongs to exactly one of these two layers.

---

# Everyday App Categories

<div class="thread">You already use several categories, every single day.</div>

<div class="appgrid">
<div class="app"><div class="name">Word processor</div><div class="desc">Write and edit documents.</div></div>
<div class="app"><div class="name">Web browser</div><div class="desc">View pages on the internet.</div></div>
<div class="app"><div class="name">Photo editor</div><div class="desc">View, crop, and edit pictures.</div></div>
<div class="app"><div class="name">Media player</div><div class="desc">Play music or video files.</div></div>
<div class="app"><div class="name">Messaging app</div><div class="desc">Send texts, photos, and calls.</div></div>
<div class="app"><div class="name">Game</div><div class="desc">Entertainment you directly control.</div></div>
</div>

Each app does one job well, instead of trying to do everything.

---

# Software Classification: Grouping by What It Does

<div class="thread">Beyond system vs. application, apps split further by function.</div>

<div class="cardlist">
<div class="card"><div class="h">Word Processing</div><div class="d">Writing and editing text documents.</div></div>
<div class="card"><div class="h">Spreadsheet</div><div class="d">Organizing numbers into rows, columns, and formulas.</div></div>
<div class="card"><div class="h">Media</div><div class="d">Playing or editing music, video, and photos.</div></div>
<div class="card"><div class="h">Communication</div><div class="d">Messaging, calling, and video chatting with others.</div></div>
</div>

---

# More Categories You Use Every Day

<div class="thread">The list keeps going.</div>

<div class="cardlist">
<div class="card"><div class="h">Educational</div><div class="d">Apps built for studying, practicing, and taking quizzes.</div></div>
<div class="card"><div class="h">Entertainment</div><div class="d">Games and streaming apps, built purely to entertain.</div></div>
<div class="card"><div class="h">Productivity</div><div class="d">Calendars, to-do lists, and note-taking apps.</div></div>
<div class="card"><div class="h">Navigation</div><div class="d">Maps and route-finding apps.</div></div>
</div>

---

# Worked Example: Sorting Minjun's Home Screen

<div class="thread">One phone, several categories, all at once.</div>

- A spreadsheet app for his part-time job's schedule: **spreadsheet**.
- A maps app for finding the bus stop: **navigation**.
- A study app for flashcards before this course's quiz: **educational**.
- A messaging app for his group project: **communication**.

Classifying by function is exactly how app stores organize millions of apps for you.

---

# Why Classification Matters

<div class="thread">Not just tidiness. It changes how you evaluate software.</div>

- Comparing two word processors makes sense; comparing a word processor to a game does not.
- Job postings often ask for skill with "spreadsheet software" or "communication tools," by category, not by brand name.
- Understanding categories helps you pick the right tool for a task, instead of forcing one app to do everything.

---

# Every App Still Needs the OS

<div class="thread">An app cannot work fully alone. Here is why.</div>

<div class="pipeline">
<div class="stage"><div class="h">App opens</div><div class="s">asks OS for memory</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">App reads a file</div><div class="s">asks OS to reach storage</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">App runs</div><div class="s">asks OS for CPU time</div></div>
</div>

An app makes requests. The OS decides how to share the machine. More
on sharing fairly, next week.

---

<!-- NEW: Try-It hand-off, Worksheet Part A -->

# Try It: Worksheet Part A

<div class="thread">Now you practice. Work with a partner.</div>

- Open **[Worksheet Part A](materials/week06/worksheet.html)**.
- Sort each program into "application software" or "system software."
- You have about 15 minutes. Ask your partner before you ask me.

<!-- notes: Hand out Worksheet Part A. Walk around and help pairs. After 15 minutes, ask 2-3 pairs to share one answer. -->

---

<!-- NEW: Key Words Today, session 3 -->

# Key Words Today

- **Decode** — turn stored data back into a picture, sound, or text.
- **Render** — draw something on screen so a person can see it.
- **Install** — add a new app onto a device before using it.
- **Update** — replace an app with a newer, improved version.

<!-- notes: Read each word aloud. Say: "You will see these words in Worksheet Part B." -->

---

# How Is Software Actually Made?

<div class="thread">Every app you use started as text, typed by a person.</div>

> A programmer writes **source code**: instructions in a human-readable
> programming language. That source code must be turned into a form
> the CPU can actually execute before it becomes a running program.

---

# Diagram: From Source Code to Running Program

<div class="thread">Two different roads to the same destination.</div>

<div class="pipeline">
<div class="stage"><div class="h">Source code</div><div class="s">written by a programmer, human-readable</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Compiler or interpreter</div><div class="s">translates it into instructions the CPU understands</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Running program</div><div class="s">the app you actually open and use</div></div>
</div>

---

# Compiled vs Interpreted, Briefly

<div class="thread">Two ways to do that translation step.</div>

- **Compiled:** the entire source code is translated into machine instructions once, in advance, producing a program file you can run directly, again and again.
- **Interpreted:** the source code is translated and run line by line, each time the program runs, with no separate translation step beforehand.

Week 10 returns to this in far more depth, once you have written code of your own.

---

# Worked Example: Behind Minjun's Photo App

<div class="thread">A team of programmers, long before Minjun ever opened the app.</div>

- Developers wrote the photo app's source code, function by function.
- A compiler translated that source code into a program file.
- That program file is exactly what Minjun's app store delivers to his phone, ready to run.

---

# Software Licensing: Who's Allowed to Do What?

<div class="thread">Installing software is never truly free of rules.</div>

> A **software license** is the set of rules that says how a program
> may be used, copied, changed, or shared.

---

# Three Common Licensing Models

<div class="thread">Most software you use falls into one of these three.</div>

- **Proprietary** — the company keeps the source code private; you usually pay to use it, and cannot legally modify it.
- **Open-source** — the source code is published publicly; anyone may read, modify, and often redistribute it.
- **Freeware** — free to use, but the source code stays private, and modification is not allowed.

---

# Common Confusion: "Free" vs "Open-Source"

<div class="thread">These two words get mixed up constantly.</div>

- **Freeware** means no cost to use. The source code is still hidden.
- **Open-source** means the source code is public and modifiable. It may or may not also be free of cost.

"Free" describes a price. "Open-source" describes access to the code. They answer two different questions.

---

# Worked Example: Minjun Picks a Photo Editor

<div class="thread">Three real choices, three different licenses.</div>

| Option | License | Trade-off |
|---|---|---|
| Paid photo editor | Proprietary | Polished, supported, costs money |
| Free community editor | Open-source | No cost, customizable, community support only |
| Ad-supported photo app | Freeware | No cost, but shows ads, code stays hidden |

---

# Why Licensing Matters Beyond the Price Tag

<div class="thread">Licensing shapes far more than what you pay.</div>

- It decides whether you can legally copy the software for a friend.
- It decides whether a company or a community fixes bugs.
- It decides whether you can see, and trust, exactly what the program does.

---

# Software Changes Everyday Life

<div class="thread">Application software doesn't just run on a device. It reshapes daily routines.</div>

Beyond writing documents and editing photos, application software has
quietly rebuilt how people navigate, receive care, and learn, often
without anyone calling it a big deal.

---

# Worked Example: Three Everyday Shifts

<div class="thread">Life before this software, and life after it.</div>

| Task | Before | After (with software) |
|---|---|---|
| Getting somewhere new | Paper maps, asking strangers | A navigation app gives turn-by-turn directions |
| Seeing a doctor | Always an in-person visit | A telehealth app allows a video consultation from home |
| Studying a subject | Only in-person classrooms | An e-learning platform delivers lessons and quizzes online |

---

# Worked Example: This Very Course

<div class="thread">You don't have to look far to find e-learning software in action.</div>

This course itself distributes its worksheets and self-check quizzes as
software, files a browser renders on your screen. The photo-app case
study from earlier in this deck is also how your e-learning materials
reach you: stored data, decoded and rendered into something you can read.

---

# Software Distribution: How Programs Actually Reach You

<div class="thread">A finished program is useless until it reaches a real device.</div>

> **Software distribution** is how a finished program gets from its
> developer onto the device that will run it.

---

# From Big Box Software to App Stores

<div class="thread">Distribution itself has changed enormously.</div>

- **Decades ago:** software shipped physically, on floppy disks, then CDs, bought in a store.
- **Today:** an app store delivers the same program instantly, over the internet, to any registered device.

---

# What "Installing" an App Actually Does

<div class="thread">Installing is not magic. It is a specific set of steps.</div>

- The device downloads the program's files from a server.
- Those files are copied onto secondary storage (recall Week 5).
- The operating system registers the new program, so it appears as an icon you can open.

---

# Worked Example: Minjun Downloads an App

<div class="thread">One tap, several steps, all in the background.</div>

- He taps "Install" on an app store listing.
- His phone downloads the program's files over the network.
- The files are written to his phone's storage, and the OS adds an icon to his home screen.

---

# Updates: The Same Process, Repeated

<div class="thread">Recall the vocabulary word from Key Words Today.</div>

An **update** simply repeats the install process with newer files,
replacing the old version already on storage. That is why an update
still needs a network connection and free storage space, exactly like a first-time install.

---

<!-- SLOT N-2: Worked example -->

# Case Study: A File Becomes a Photo

<div class="thread">Same idea, real device. Back to "What's Actually Inside Your Laptop."</div>

- **In storage:** the photo is only bytes, `1`s and `0`s. Not a picture yet.
- **Photo app opens it:** the app decodes those bytes into color and shape.
- **Screen renders it:** now you see the actual photo, and can edit it.

This is what "turning data into something useful" really means.

---

<!-- SLOT N-1: Common mistakes -->

# Common Mistakes

- **"Apps and the OS are the same thing":** Wrong. The OS manages the machine; an app does one task for you.
- **"More installed apps make a computer faster":** Wrong. Apps use memory and storage; too many can slow it down.
- **"An app runs all by itself":** Wrong. Every app depends on the OS for memory, storage, and CPU time.

---

<!-- NEW: Try-It hand-off, Worksheet Part B -->

# Try It: Worksheet Part B

<div class="thread">More practice. New scenarios.</div>

- Open **[Worksheet Part B](materials/week06/worksheet.html)**.
- Match each everyday task to the app category that does it best.
- You have about 15 minutes. Then we discuss answers together.

<!-- notes: Hand out Worksheet Part B. After 15 minutes, go through the answer key as a class. Ask for volunteers first. -->

---

<!-- SLOT N: Check yourself -->

# Check Yourself

1. Name one thing an app does that the OS itself does not do.
2. A photo file exists, but no photo app is installed. Can you view it?
3. Give one example of application software you used today.

---

# Answers

1. An app does one specific task for a user, like writing or editing.
2. No. The raw file needs an app to decode and show it as a picture.
3. Any real app: a browser, a messaging app, a game, and so on.

---

<!-- NEW: Quiz 1 logistics, before the self-check quiz hand-off -->

# Quiz 1 Today

Quiz 1 is now: closed-book, covers Weeks 1-6, about 15 minutes.

<!-- notes: Collect phones and notes before handing out Quiz 1. Give a clear 15-minute time limit. Collect papers when time is up. -->

---

<!-- NEW: Self-check quiz hand-off -->

# Self-Check Quiz

<div class="thread">After Quiz 1, one more check, on your own.</div>

- Take the **[Week 6 Quiz](materials/week06/quiz.html)** (5-8 short questions).
- This quiz is not graded. It just checks your understanding.
- About 10 minutes. Check your own answers at the end.

<!-- notes: Hand out the self-check quiz only after Quiz 1 is collected. Give students 10 minutes, then let them self-check. -->

---

<!-- SLOT N+1: Limits (Act 4 / CLOSE), becomes Week 7 slot 4 -->

# What Apps Cannot Do Alone

<div class="limits">
Apps now turn stored data into something useful. But your laptop runs
many apps at once. Something must decide which app runs when, and
share the machine fairly among them. We do not have that yet.
</div>

---

<!-- SLOT N+2: Bridge -->

# Next Week

Week 6 leaves **sharing one machine among many running apps**
unsolved. **Week 7, Operating Systems**, addresses it: how one
program manages every other program, fairly.

---

<!-- SLOT N+3: Summary -->

# Summary

- Application software does one task for a user; system software manages the machine.
- Apps decode stored data (photos, documents, files) into something you can actually use.
- Every app still depends on the OS for memory, storage, and CPU time.
- **Reading:** Tanenbaum & Austin, Chapter 1 (software overview section).
- **Handout:** [materials/week06/handout.md](materials/week06/handout.html), glossary and the full worked example.
- **Prepare:** List three apps you used today. Bring the list to Week 7.

---

<!-- SLOT N+4: Thank You -->
<!-- _class: end -->

# Thank You
