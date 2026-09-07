---
marp: true
theme: shintia
paginate: true
footer: 'Department of Intelligent Computing'
---

<!-- SLOT 1: Title -->
<!-- _class: title -->

# Week 7: Operating Systems

<span class="subtitle">Introduction to Computer Engineering (400507-001)</span>

<div class="meta">
Yushintia Pramitarini, Ph.D · Dept. of Intelligent Computing · Thu [1-3] · Seongpa Hall 701
</div>

<!--
notes: Ask everyone to look at their laptop or phone. Ask: "How many
apps are open right now?" Collect two or three numbers out loud. Say:
"One chip. Many apps. Who decides who goes first?"
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
<div class="wk now"><div class="n">Wk 7</div><div class="t">Operating Systems</div></div>
<div class="wk review"><div class="n">Wk 8</div><div class="t">Midterm Exam</div></div>
<div class="wk"><div class="n">Wk 9</div><div class="t">Computer &amp; Internet</div></div>
<div class="wk"><div class="n">Wk 10</div><div class="t">Programming Language</div></div>
<div class="wk"><div class="n">Wk 11</div><div class="t">Databases &amp; Security</div></div>
<div class="wk"><div class="n">Wk 12</div><div class="t">Computer Applications</div></div>
<div class="wk"><div class="n">Wk 13</div><div class="t">AI · Quiz 2</div></div>
<div class="wk"><div class="n">Wk 14</div><div class="t">Emerging Technologies</div></div>
<div class="wk review"><div class="n">Wk 15</div><div class="t">Final Exam</div></div>
</div>

<!-- notes: Point at Week 7. Say: "Today we zoom into one layer: the software that shares your machine between apps." -->

---

<!-- SLOT 3: Recap + open wound -->

# Last Week, This Week

- **Last week delivered:** we saw real apps, like browsers and word processors, that let people do real tasks.
- **Last week left broken:** apps exist, but nothing coordinates which app runs when, or shares the machine fairly.

---

<!-- SLOT 4: The pain (Act 1 / MOTIVATE), ZERO jargon -->

# Too Many Apps, One Machine

<div class="pain">

You open five apps at once. A browser, a music player, a video call,
a word processor, and a game downloading in the background.

Your laptop has only one chip. It has only so much space to hold
things while they run. Nobody told any app to wait its turn.

If one app grabs everything, the other four freeze. How does your
laptop decide who goes first, and share fairly among all five?

</div>

<!-- notes: Ask: "Have you ever had one app freeze the rest of your laptop?" Let two or three students answer. Do not explain yet. -->

---

<!-- SLOT 5: Cost of not knowing -->

# What This Actually Costs

- Without this, you cannot explain why your laptop slows down at all.
- One crashing app could take down your whole machine, with nothing to stop it.
- Windows, macOS, Android, and Linux all depend on this exact idea.

<div class="why">
<strong>In industry:</strong> "How does an OS share the CPU?" is a
common interview question for systems and mobile engineering jobs.
</div>

---

<!-- SLOT 6: Driving question -->

<!-- _class: section -->

# This Week's Question

<div class="driving-q">"How does one operating system share one machine fairly among many running apps?"</div>

---

<!-- SLOT 7: Learning outcomes -->

# By the End of This Week, You Can

<div class="cardlist">
<div class="card"><div class="h">What an OS Does</div><div class="d">Explain what an operating system does, in plain words.</div></div>
<div class="card"><div class="h">Sharing CPU Time</div><div class="d">Describe how the OS shares CPU time between many apps.</div></div>
<div class="card"><div class="h">Private Memory</div><div class="d">Explain why each app gets its own private memory space.</div></div>
<div class="card"><div class="h">Tracing a Request</div><div class="d">Trace one app's request to the OS, and back.</div></div>
</div>

---

<!-- SLOT 8: Origin -->

# Where This Idea Came From

<div class="thread">You just felt the pain. Where did the answer come from?</div>

- **1950s-60s:** early computers ran one program at a time. People waited in long lines for their turn.
- **1960s:** researchers built "time-sharing" systems, so many people could use one computer together.
- **1969:** Bell Labs built Unix. Its ideas still run inside phones and laptops today.

<div class="why">
Sharing one machine fairly was not obvious at all. It took years of
careful design to get right.
</div>

---

<!-- SLOT 9: Core concept -->

# Operating System: Definition

<div class="thread">One idea, one clear definition.</div>

> An **operating system (OS)** is software that manages a computer's
> hardware, and shares it fairly among running programs.

- The OS decides which program runs next.
- The OS decides how memory is divided.
- Every app reaches hardware only through the OS, never on its own.

---

<!-- NEW: Key Words Today, session 1 -->

# Key Words Today

- **Operating system (OS)** — software that manages hardware and shares it between apps.
- **Process** — one program while it is running.
- **Multitask** — run many programs at almost the same time.
- **Manage** — decide how something is used, and by whom.
- **Fair share** — every app gets a turn, not just the loudest one.

<!-- notes: Read each word aloud. Ask students to repeat it once. Ask: "Which of these words did you already know?" -->

---

<!-- NEW: Try-It preview, closes session 1 -->

# Coming Up: Worksheet Part A

<div class="thread">Next, you will practice using these words.</div>

- In **[Worksheet Part A](materials/week07/worksheet.html)**, you sort everyday laptop problems by cause.
- Example: "My laptop feels slow with ten tabs open." Is that CPU or memory?
- You will work with a partner. A guess is fine for now.

<!-- notes: Tell students to sit next to a partner for the next part. No prep needed. -->

---

<!-- NEW: Key Words Today, session 2 -->

# Key Words Today

- **Scheduler** — the OS part that picks which process runs next.
- **Time slice** — a short turn of CPU time given to one process.
- **Switch** — the OS changes from running one process to another, very fast.
- **Memory space** — the private area of memory one process can use.
- **Crash** — a program stops working, often from using memory it should not.

<!-- notes: Read each word aloud. Say: "You will use all five words in the next slides." -->

---

<!-- Act 3 / BUILD -->

# What an Operating System Actually Sets Out to Do

<div class="thread">One definition, three underlying goals.</div>

Every operating system, no matter how old or new, exists to achieve three goals at once:

- **Manage resources** — share the CPU, memory, and devices fairly.
- **Provide a user interface** — let a person actually control the machine.
- **Execute programs** — load and run the software a user asks for.

---

# Three Goals, One Job

<div class="cardlist">
<div class="card"><div class="h">Resource Management</div><div class="d">Share CPU time, memory, and devices among every running program.</div></div>
<div class="card"><div class="h">User Interface</div><div class="d">Give a person a way to actually control the machine.</div></div>
<div class="card"><div class="h">Program Execution</div><div class="d">Load a program into memory, and start it running.</div></div>
</div>

---

# Worked Example: Three Goals, One Ordinary Laptop

<div class="thread">Back to Minjun's five open apps. All three goals, at once.</div>

- **Resource management:** the OS juggles his browser, music, and video call, so none of them freeze the others.
- **User interface:** the desktop icons and taskbar he clicks are literally how he controls all of this.
- **Program execution:** double-clicking any of those icons is the OS loading and starting a program.

---

# Is Every Program on the Laptop "the OS"?

<div class="thread">A quick, important distinction from last week.</div>

No. The operating system is one specific piece of system software (Week
6). The browser, the music player, and every other app Minjun opens are
application software, built on top of the OS, not part of it.

---

# What the OS Actually Manages

<div class="thread">One busy machine. Three separate jobs to manage.</div>

<div class="appgrid">
<div class="app"><div class="name">CPU time</div><div class="desc">Which process runs right now.</div></div>
<div class="app"><div class="name">Memory</div><div class="desc">How much space each process gets.</div></div>
<div class="app"><div class="name">Devices</div><div class="desc">The screen, keyboard, disk, network.</div></div>
</div>

Every app asks the OS first. No app touches hardware directly.

---

# Sharing the CPU: One Chip, Many Turns

<div class="thread">Five apps, one CPU. How does everyone get a turn?</div>

<div class="pipeline">
<div class="stage"><div class="h">Browser</div><div class="s">runs for one time slice</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Music app</div><div class="s">runs for one time slice</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Video call</div><div class="s">runs for one time slice</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Back to browser</div><div class="s">and repeat, very fast</div></div>
</div>

Switching is so fast, it feels like everything runs at once. This is
called **multitasking**.

---

# Sharing Memory: Every App Gets Its Own Space

<div class="thread">The CPU takes turns. Memory works a bit differently.</div>

- Each process gets its own private area of memory.
- One app cannot see or change another app's memory.
- If an app tries anyway, the OS stops it right away.

This keeps one crashing app from crashing every other app too.

---

# Four Jobs, Looked at More Closely

<div class="thread">The appgrid earlier named three. Here is the fourth, and all four in depth.</div>

Every operating system performs four core management jobs, each worth
its own definition: process management, memory management, file
management, and device management.

---

# Process Management: Definition

<div class="thread">The first of the four jobs.</div>

> **Process management** is how the OS creates, schedules, and
> eventually ends every running program, called a **process**.

Example: opening a browser creates a new process. Closing it ends that
process, and frees whatever resources it was using.

---

# Memory Management: Definition

<div class="thread">The second of the four jobs.</div>

> **Memory management** is how the OS decides how much memory each
> running process gets, and keeps one process from touching another's memory.

Example: Minjun's browser and his music player each get separate
memory. A bug in one cannot corrupt the other.

---

# File Management: Definition

<div class="thread">The third of the four jobs, and a brand-new one this week.</div>

> **File management** is how the OS organizes stored data into named
> files and folders, and tracks exactly where each one physically lives in storage.

Example: Minjun saves his essay as `essay_draft.docx` inside a
Documents folder. The OS remembers exactly which spot on his SSD holds
those bytes, so he can find the file again by name, never by memory address.

---

# Device Management: Definition

<div class="thread">The fourth of the four jobs.</div>

> **Device management** is how the OS communicates with hardware,
> through device drivers, on behalf of every running process.

Example: when Minjun's browser needs to display a video, device
management hands the finished pixels to the screen's driver.

---

# One Click, Four Jobs at Once

<div class="thread">Every one of the four jobs, inside one ordinary click.</div>

Minjun double-clicks a photo file. In that single instant:

- **Process management** creates a new process for the photo viewer.
- **Memory management** gives that process its own private space.
- **File management** locates the exact bytes of that photo on the SSD.
- **Device management** sends the finished image to the screen.

---

<!-- NEW: Try-It hand-off, Worksheet Part A -->

# Try It: Worksheet Part A

<div class="thread">Now you practice. Work with a partner.</div>

- Open **[Worksheet Part A](materials/week07/worksheet.html)**.
- Decide: is each scenario about CPU time, memory, or a device?
- You have about 15 minutes. Ask your partner before you ask me.

<!-- notes: Hand out Worksheet Part A. Walk around and help pairs. After 15 minutes, ask 2-3 pairs to share one answer. -->

---

<!-- NEW: Key Words Today, session 3 -->

# Key Words Today

- **Device driver** — software that lets the OS talk to one piece of hardware.
- **Request** — an app asks the OS for something, like memory or the screen.
- **Queue** — a line of processes, waiting for their turn.
- **Priority** — how important a request is. It decides who goes first.

<!-- notes: Read each word aloud. Say: "These words tie everything together today." -->

---

# Talking to Hardware: Always Through the OS

<div class="thread">Apps never touch hardware directly. The OS stands in between.</div>

- A **device driver** lets the OS talk to one piece of hardware.
- Example: a printer driver, a screen driver, a wifi driver.
- An app sends a **request** to the OS. The OS talks to the driver.

Without the right driver, the OS cannot use that hardware at all.

---

# Four Types of Operating Systems, Part One

<div class="thread">Not every OS is built for the same situation.</div>

- **Batch** — runs a queued stack of jobs with no user interaction, one after another.
- **Time-sharing** — splits CPU time among many users or tasks, so each one feels instant. Most everyday laptops and phones behave this way.

---

# Four Types of Operating Systems, Part Two

<div class="thread">The other two types, built for very different pressures.</div>

- **Real-time** — must respond within a strict, guaranteed time limit, or the whole system fails.
- **Distributed** — spreads one job's work across many separate machines, working together as one system. Week 9 explores this in depth.

---

# Worked Example: One Type, One Real System

<div class="thread">Four abstract categories, four concrete machines.</div>

| Type | Real Example |
|---|---|
| Batch | A bank processing millions of overnight transactions |
| Time-sharing | Minjun's own laptop, juggling five open apps |
| Real-time | A car's anti-lock braking system, reacting in milliseconds |
| Distributed | A streaming service's video, spread across many data-center machines |

---

# A Short History of the Operating System

<div class="thread">From typed commands to touch and voice.</div>

<div class="timeline">
<div class="pt"><div class="dot"></div><div class="y">1960s-70s</div><div class="d">DOS-style systems: users type text commands, one line at a time</div></div>
<div class="pt"><div class="dot"></div><div class="y">1984</div><div class="d">Graphical OS arrives: windows, icons, and a mouse replace typed commands</div></div>
<div class="pt"><div class="dot"></div><div class="y">2007</div><div class="d">Touch-based mobile OS begins reaching everyday pockets</div></div>
<div class="pt"><div class="dot"></div><div class="y">Today</div><div class="d">Modern OS blends touch, voice, and constant cloud connection</div></div>
</div>

---

# The DOS Era: Typing Every Instruction

<div class="thread">The first stop on the timeline above.</div>

Early operating systems like DOS gave users a blank text prompt. Every
action, opening a file, running a program, had to be typed out exactly,
with no icons and no mouse at all.

---

# The GUI Era: Pointing Instead of Typing

<div class="thread">The second stop on the timeline above.</div>

Graphical operating systems let users click icons and drag windows
instead of typing commands. This single shift is why computers became
usable by people with no technical training at all.

---

# The Modern Era: Touch, Voice, and the Cloud

<div class="thread">The most recent stop on the timeline above.</div>

Today's operating systems respond to touch and voice, constantly sync
with the cloud, and run on phones, laptops, and watches alike, often
the same OS family across every one of them.

---

# Worked Example: Minjun's Own Family Timeline

<div class="thread">The whole history above, inside one family.</div>

His grandfather's first computer ran a DOS-style system, typed command
by command. Minjun's own laptop runs a modern graphical OS, and he
barely remembers a time before touchscreens. Three generations, three
very different ways of talking to the same idea: an operating system.

---

# Major Operating System Families Today

<div class="thread">Different devices, different needs, different OS families.</div>

Five families dominate today's devices, and each one is built around
one clearly differentiating idea.

---

# Windows

<div class="thread">One differentiating fact.</div>

Windows is built for broad hardware compatibility: it runs on an
enormous variety of PC hardware, from many different manufacturers, not
just one.

---

# macOS

<div class="thread">One differentiating fact.</div>

macOS is built by Apple exclusively for Apple's own hardware, which
lets the operating system and the machine be tuned tightly together.

---

# Linux / UNIX Lineage

<div class="thread">One differentiating fact.</div>

Linux traces back to UNIX, and is open-source (recall Week 6's
licensing concept). That openness is exactly why it quietly powers most
of the world's servers and cloud data centers.

---

# Mobile OS: Android and iOS

<div class="thread">One differentiating fact.</div>

Android and iOS are built around touch input and a single home screen
of apps, not a desktop of overlapping windows like Windows or macOS.

---

# Embedded OS

<div class="thread">One differentiating fact.</div>

An embedded OS is built to run just one dedicated job forever, inside
devices like a car's dashboard or a washing machine, not to run
arbitrary apps a user installs later.

---

# Choosing the Right OS Family for the Job

<div class="thread">Five families, matched to five real devices.</div>

- Minjun's gaming desktop: **Windows**, for its huge hardware and game support.
- Minjun's phone: **Android** or **iOS**, built around touch.
- The server behind his favorite app: almost certainly **Linux**.
- The washing machine in his dorm: a tiny **embedded OS**, doing exactly one job.

---

# The Scheduler: Who Goes Next?

<div class="thread">A word from Key Words Today, now given its own definition.</div>

> The **scheduler** is the specific part of the OS that decides which
> process runs next, and for how long.

Every time-slice switch you saw earlier in this deck is a decision the
scheduler makes, dozens of times per second.

---

# Round-Robin: One Fair Way to Take Turns

<div class="thread">One common scheduling approach, in plain words.</div>

One common scheduling approach is **round-robin**: give every process
an equal time slice, in a fixed rotating order, then repeat. No process
is favored over another just because it asked first.

---

# Case Study: Three Processes, Ten Milliseconds Each

<div class="thread">Round-robin, traced through real time.</div>

<div class="pipeline">
<div class="stage"><div class="h">Browser</div><div class="s">0-10ms</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Music</div><div class="s">10-20ms</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Video call</div><div class="s">20-30ms</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Browser again</div><div class="s">30-40ms</div></div>
</div>

In just 40 milliseconds, every process has already had a turn, and the rotation starts again.

---

# Why Fairness Matters

<div class="thread">The whole reason a scheduler exists at all.</div>

Without a scheduler enforcing turns, one greedy process could simply
keep running forever, freezing every other app on the machine. A fair
scheduler is exactly what keeps one busy download from freezing your
music or your video call.

---

<!-- SLOT N-2: Worked example -->

# Case Study: Five Apps, One Fair Machine

<div class="thread">Back to your five open apps. Now you have the words.</div>

Here is what the OS does, every second, without you noticing:

<div class="chip-row">
<span class="chip">Browser: waits for its time slice</span>
<span class="chip">Music app: keeps its own memory</span>
<span class="chip">Video call: gets priority for smooth sound</span>
<span class="chip">Game download: uses the disk driver</span>
</div>

No app ever touches the chip, memory, or disk on its own. The OS decides.

---

<!-- SLOT N-1: Common mistakes -->

# Common Mistakes

- **"Multitasking means apps run at the exact same time":** Wrong. The CPU switches fast, one process at a time.
- **"More open apps always means less speed":** Not always true. An idle app barely uses the CPU.
- **"An app can just take the memory it wants":** Wrong. The OS controls every single request.

---

<!-- NEW: Try-It hand-off, Worksheet Part B -->

# Try It: Worksheet Part B

<div class="thread">More practice. New scenarios.</div>

- Open **[Worksheet Part B](materials/week07/worksheet.html)**.
- Decide which OS job explains each scenario, and why.
- You have about 15 minutes. Then we discuss answers together.

<!-- notes: Hand out Worksheet Part B. After 15 minutes, go through the answer key as a class. Ask for volunteers first. -->

---

<!-- SLOT N: Check yourself -->

# Check Yourself

1. Name two things the operating system manages.
2. Why does one app never see another app's memory?
3. Your laptop runs five apps with only one CPU. How is that possible?

---

# Answers

1. Any two of: CPU time, memory, and devices.
2. The OS gives each process its own private memory space.
3. The OS switches between apps very fast, using short time slices.

---

<!-- NEW: Self-check quiz hand-off -->

# Self-Check Quiz

<div class="thread">One more check, on your own.</div>

- Take the **[Week 7 Quiz](materials/week07/quiz.html)** (5-8 short questions).
- This quiz is not graded. It just checks your understanding.
- About 10 minutes. Check your own answers at the end.

<!-- notes: Hand out the quiz. Give students 10 minutes. Then read the answer key aloud, or let students self-check. -->

---

<!-- SLOT N+1: Limits (Act 4 / CLOSE), becomes Week 9 slot 4 -->

# What One Machine Still Cannot Do

<div class="limits">
One machine now runs well by itself. It shares its CPU, memory, and
devices fairly among many apps. But it is still completely alone. It
is unable to talk to any other machine at all.
</div>

---

<!-- SLOT N+2: Bridge -->

# Next Week

Week 7 leaves **talking to other machines** unsolved. **Week 9,
Computer & Internet**, addresses it: how machines connect and share
data with each other.

---

<!-- SLOT N+3: Summary -->

# Summary

- The OS manages CPU time, memory, and devices, for every open app.
- It shares the machine fairly, one short turn at a time.
- Every app request goes through the OS, never straight to hardware.
- **Reading:** Tanenbaum & Austin, the chapter on operating systems.
- **Handout:** [materials/week07/handout.md](materials/week07/handout.html), glossary and the full worked example.
- **Prepare:** Think about how your phone and laptop share files. Bring an example to Week 9.
- **Note:** Midterm next week (Weeks 1-7). Review your notes before class.

---

<!-- SLOT N+4: Thank You -->
<!-- _class: end -->

# Thank You
