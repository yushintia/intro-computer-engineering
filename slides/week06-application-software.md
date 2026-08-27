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
Yushintia Pramitarini, Ph.D · Dept. of Intelligent Computing · Thu [1-3] · 성파 701
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

<!-- NEW: Key Words Today, 차시 1 -->

# Key Words Today

- **Application software (app)** — a program that helps you do one task.
- **System software** — software that manages the whole computer, like the OS.
- **Killer app** — an app so useful, people buy the device just for it.
- **User** — the person using an app to get something done.

<!-- notes: Read each word aloud. Ask students to repeat it once. Ask: "Which apps on your phone match this definition?" -->

---

<!-- NEW: Try-It preview, closes 차시 1 -->

# Coming Up: Worksheet Part A

<div class="thread">Next, you will practice using these words.</div>

- In **[Worksheet Part A](materials/week06/worksheet.html)**, you sort real programs into app or system software.
- Example: "a web browser" — is that an app, or system software?
- You will work with a partner. A guess is fine for now.

<!-- notes: Tell students to sit next to a partner for the next part. No prep needed. -->

---

<!-- _class: section -->

# End of 차시 1
<div class="driving-q">Short break. 차시 2: app categories, and how every app needs the OS.</div>

---

<!-- NEW: Key Words Today, 차시 2 -->

# Key Words Today

- **Category** — a group of apps that do a similar kind of task.
- **Interface** — the screen and buttons an app shows to a user.
- **Request** — when an app asks the OS for something it needs.
- **Resource** — memory, storage, or CPU time an app needs to run.

<!-- notes: Read each word aloud. Say: "You will use all four words in the next slides." -->

---

<!-- Act 3 / BUILD -->

# Application vs. System Software

<div class="thread">Back to the locked photo. What was actually missing?</div>

<div class="stack">
<div class="layer view"><span class="h">Application Software</span> <span class="s">does one task for you: a photo app, a browser, a game</span></div>
<div class="layer logical"><span class="h">System Software / OS</span> <span class="s">manages the whole machine: shares memory, storage, CPU: Week 7</span></div>
</div>

The photo file was safe. The app to open it was missing, not the OS.

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

<!-- _class: section -->

# End of 차시 2
<div class="driving-q">Short break. 차시 3: a worked example, more practice, then Quiz 1.</div>

---

<!-- NEW: Key Words Today, 차시 3 -->

# Key Words Today

- **Decode** — turn stored data back into a picture, sound, or text.
- **Render** — draw something on screen so a person can see it.
- **Install** — add a new app onto a device before using it.
- **Update** — replace an app with a newer, improved version.

<!-- notes: Read each word aloud. Say: "You will see these words in Worksheet Part B." -->

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
