# Week 7 Handout: Operating Systems

Introduction to Computer Engineering (400507-001) · Week 7
This handout goes with the Week 7 slides. Keep it for the midterm.

---

## 1. Glossary: Key Words

Simple, plain definitions. Read these before or after class.

| Word | Plain definition |
|---|---|
| **Operating system (OS)** | Software that manages a computer's hardware, and shares it fairly among running programs. |
| **Process** | One program while it is running. |
| **Multitask** | Run many programs at almost the same time. |
| **Manage** | Decide how something is used, and by whom. |
| **Fair share** | Every app gets a turn, not just the loudest one. |
| **Scheduler** | The OS part that picks which process runs next. |
| **Time slice** | A short turn of CPU time given to one process. |
| **Switch** | The OS changes from running one process to another, very fast. |
| **Memory space** | The private area of memory one process can use. |
| **Crash** | A program stops working, often from using memory it should not. |
| **Device driver** | Software that lets the OS talk to one piece of hardware. |
| **Request** | An app asks the OS for something, like memory or the screen. |
| **Queue** | A line of processes, waiting for their turn. |
| **Priority** | How important a request is. It decides who goes first. |
| **Process management** | How the OS creates, schedules, and eventually ends every running program (process). |
| **Memory management** | How the OS decides how much memory each running process gets, and keeps one process from touching another's memory. |
| **File management** | How the OS organizes stored data into named files and folders, and tracks exactly where each one physically lives in storage. |
| **Device management** | How the OS communicates with hardware, through device drivers, on behalf of every running process. |
| **Resource management** | One of the OS's three goals: sharing the CPU, memory, and devices fairly among running programs. |
| **User interface** | One of the OS's three goals: giving a person a way to actually control the machine. |
| **Program execution** | One of the OS's three goals: loading a program into memory, and starting it running. |
| **Batch OS** | Runs a queued stack of jobs with no user interaction, one after another. |
| **Time-sharing OS** | Splits CPU time among many users or tasks, so each one feels instant. Most everyday laptops and phones behave this way. |
| **Real-time OS** | Must respond within a strict, guaranteed time limit, or the whole system fails. |
| **Distributed OS** | Spreads one job's work across many separate machines, working together as one system. |
| **DOS era** | Early operating systems (1960s-70s) that gave users a blank text prompt; every action had to be typed. |
| **GUI era** | Beginning in 1984, graphical operating systems let users click icons and drag windows instead of typing commands. |
| **Modern era** | Today's operating systems, which respond to touch and voice and constantly sync with the cloud. |
| **Round-robin** | A scheduling approach that gives every process an equal time slice, in a fixed rotating order, then repeats. |

---

## 2. Five Apps, One Fair Machine, Step by Step

This is the full version of the story from class. The slide version was
shortened. Read this at home if you want more detail.

You open five apps at once: a browser, a music player, a video call, a
word processor, and a game downloading in the background. Your laptop
has only one CPU, and only so much memory. Nobody told any single app
to wait its turn.

Without an operating system, the first app to start would simply grab
everything. It would never let go. The other four would freeze
forever, doing nothing at all.

The operating system fixes this, every second, without you noticing:

1. **The scheduler gives each process a time slice.** The browser
   runs for a tiny slice of time. Then the OS switches to the music
   app. Then the video call. Then back to the browser. This happens
   so fast, it feels like all five run at once.
2. **Each process gets its own memory space.** The music app cannot
   see or touch the video call's memory, and the video call cannot
   touch the music app's memory. If one app crashes, it does not take
   the others down with it.
3. **The OS tracks exactly where every file lives.** When the word
   processor saves its document, the OS records exactly which spot on
   the SSD holds those bytes, under the file's name, so the document
   can be found again by name later, never by memory address.
4. **Some requests get priority.** The video call needs smooth,
   steady sound. The OS gives its requests priority over the game
   download's disk requests, so your voice does not stutter.
5. **No app touches hardware directly.** The game download does not
   write to the disk by itself. It sends a request to the OS. The OS
   talks to the disk driver on the app's behalf.

This is why closing one frozen app usually saves the other four. The
OS was already keeping their memory and their CPU turns separate.

---

## 3. What the OS Manages: Four Jobs

Every operating system, no matter the brand, performs the same four
core management jobs:

1. **Process management**: how the OS creates, schedules, and
   eventually ends every running program, called a **process**.
   Example: opening a browser creates a new process; closing it ends
   that process and frees whatever resources it was using.
2. **Memory management**: how the OS decides how much memory each
   running process gets, and keeps one process from touching
   another's memory. Example: a browser and a music player each get
   separate memory, so a bug in one cannot corrupt the other.
3. **File management**: how the OS organizes stored data into named
   files and folders, and tracks exactly where each one physically
   lives in storage. Example: saving an essay as `essay_draft.docx`
   inside a Documents folder lets the OS remember exactly which spot
   on the SSD holds those bytes, so the file can be found again by
   name, never by memory address.
4. **Device management**: how the OS communicates with hardware,
   through device drivers, on behalf of every running process.
   Example: when a browser needs to display a video, device
   management hands the finished pixels to the screen's driver.

A single double-click shows all four jobs at once: opening a photo
file creates a new process (process management), gives that process
its own private space (memory management), locates the exact bytes of
that photo on the SSD (file management), and sends the finished image
to the screen (device management).

Each remaining week of this course builds outward from this idea:
Week 9 studies how machines talk to *each other*, once each machine
already manages itself well.

---

## 4. Three Goals of Every Operating System

Underneath its four management jobs, every operating system, no
matter how old or new, exists to achieve three goals at once:

- **Resource management**: share the CPU, memory, and devices fairly
  among running programs.
- **User interface**: let a person actually control the machine.
- **Program execution**: load and run the software a user asks for.

On one ordinary laptop, all three happen together: resource
management juggles a browser, music, and video call so none of them
freeze the others; the desktop icons and taskbar a user clicks are
literally the user interface; and double-clicking any of those icons
is the OS loading and starting a program (program execution).

---

## 5. Four Types of Operating Systems

Not every OS is built for the same situation:

- **Batch**: runs a queued stack of jobs with no user interaction,
  one after another. Example: a bank processing millions of overnight
  transactions.
- **Time-sharing**: splits CPU time among many users or tasks, so
  each one feels instant. Most everyday laptops and phones behave
  this way.
- **Real-time**: must respond within a strict, guaranteed time
  limit, or the whole system fails. Example: a car's anti-lock
  braking system, reacting in milliseconds.
- **Distributed**: spreads one job's work across many separate
  machines, working together as one system. Example: a streaming
  service's video, spread across many data-center machines. Week 9
  explores this in depth.

---

## 6. A Short History of the Operating System

- **DOS era (1960s-70s):** early operating systems gave users a blank
  text prompt. Every action, opening a file, running a program, had
  to be typed out exactly, with no icons and no mouse at all.
- **GUI era (1984):** graphical operating systems let users click
  icons and drag windows instead of typing commands. This single
  shift is why computers became usable by people with no technical
  training at all.
- **Modern era (today):** operating systems respond to touch and
  voice, constantly sync with the cloud, and run on phones, laptops,
  and watches alike, often the same OS family across every one of
  them.

---

## 7. Five Major Operating System Families

Five families dominate today's devices, each built around one
clearly differentiating idea:

- **Windows**, built for broad hardware compatibility: it runs on an
  enormous variety of PC hardware, from many different manufacturers.
- **macOS**: built by Apple exclusively for Apple's own hardware,
  letting the operating system and the machine be tuned tightly
  together.
- **Linux / UNIX lineage**: traces back to UNIX, and is open-source
  (recall Week 6's licensing concept). That openness is why it
  quietly powers most of the world's servers and cloud data centers.
- **Mobile OS (Android and iOS)**: built around touch input and a
  single home screen of apps, not a desktop of overlapping windows.
- **Embedded OS**: built to run just one dedicated job forever,
  inside devices like a car's dashboard or a washing machine, not to
  run arbitrary apps a user installs later.

---

## 8. The Scheduler and Round-Robin

The **scheduler** is the specific part of the OS that decides which
process runs next, and for how long. Every time-slice switch is a
decision the scheduler makes, dozens of times per second.

One common scheduling approach is **round-robin**: give every process
an equal time slice, in a fixed rotating order, then repeat. No
process is favored over another just because it asked first.

**Worked example.** Three processes, ten milliseconds each:

| Time | Process Running |
|---|---|
| 0-10ms | Browser |
| 10-20ms | Music |
| 20-30ms | Video call |
| 30-40ms | Browser (again) |

In just 40 milliseconds, every process has already had a turn, and
the rotation starts again. Without a scheduler enforcing turns, one
greedy process could simply keep running forever, freezing every
other app on the machine.

---

## 9. Optional Reading: More Detail

This section holds extra detail that was trimmed from the slides. It
is optional, but useful if you want to go deeper.

**Why this took decades to build well.** Early computers, before the
1960s, ran exactly one program at a time. A person handed in a stack
of punched cards, then waited, sometimes for hours, for their turn.
Researchers in the 1960s built "time-sharing" systems, so many people
could use one expensive computer together. In 1969, a small team at
Bell Labs built Unix. Its core ideas, processes, scheduling, and
private memory, still run inside Windows, macOS, Android, iOS, and
Linux today.

**How scheduling decisions get made.** A real scheduler does not just
take turns in a simple circle. It also looks at **priority**: some
requests matter more right now than others. A video call's audio
request usually gets higher priority than a background file download,
because a half-second delay in sound is very noticeable, but a
half-second delay in a download is not.

**Why memory protection matters for security, not just stability.**
Keeping each process's memory private is not only about preventing
crashes. It also stops one app from reading another app's private
data, like a password typed into a different window. This idea,
memory protection, is a foundation for computer security, covered
again in Week 11.

**Why this matters in industry.** "Explain how an operating system
schedules processes" is a very common interview question for systems,
backend, and mobile engineering roles. It tests whether a candidate
understands what is really happening underneath a "simple" multitasking
laptop or phone.

---

## 10. Practice Problems (with Answers)

Try each problem yourself before checking the answer.

**Problem 1.** Name the four core management jobs an operating
system performs for every running app.

> **Answer:** Process management, memory management, file
> management, and device management.

**Problem 2.** A friend says: "My laptop runs ten apps at the exact
same instant." Explain, in one or two sentences, why this is not
quite true.

> **Answer:** The CPU actually runs one process at a time. The OS
> switches between processes so fast, using short time slices, that
> it only feels like everything runs at once.

**Problem 3.** True or false: "One app can read another app's private
memory, if it tries hard enough." Explain your answer.

> **Answer:** False, under normal operation. Each process gets its
> own private memory space, and the OS blocks other processes from
> reaching it.

**Problem 4.** A video call app and a file download are both running.
The call's audio suddenly gets priority over the download. Why might
the OS do this?

> **Answer:** A short delay in audio is very noticeable to a person,
> but a short delay in a download usually is not. The scheduler can
> give the more time-sensitive request priority.

**Problem 5.** Explain, in your own words, why an app cannot write
directly to your laptop's disk by itself.

> **Answer:** Apps do not touch hardware directly. An app sends a
> request to the OS, and the OS talks to the disk through its device
> driver on the app's behalf.

**Problem 6.** One app crashes, but every other open app keeps
running fine. Using this week's ideas, explain why the crash did not
spread.

> **Answer (sample):** Each process has its own private memory space.
> The crashing app's problem stayed inside its own memory, so it could
> not damage the other apps' separate memory spaces.

**Problem 7.** You save a file as `notes.docx`. A week later, you
open it by typing its name, and it appears instantly. Which of the
four OS jobs made this possible, and what does that job do?

> **Answer:** File management. It organizes stored data into named
> files and folders, and tracks exactly where each one physically
> lives in storage, so it can be found again by name.

**Problem 8.** Name the three underlying goals every operating system
sets out to achieve, and explain how double-clicking an icon
demonstrates one of them.

> **Answer:** Resource management, providing a user interface, and
> program execution. Double-clicking an icon is the user interface
> (control) triggering program execution (loading and running the
> software).

**Problem 9.** A car's anti-lock braking system must react within a
strict, guaranteed time limit, or it fails completely. Which of the
four OS types is this, and why?

> **Answer:** Real-time. It must respond within a strict, guaranteed
> time limit, or the whole system fails.

**Problem 10.** Put these in order, earliest to most recent: the GUI
era, the modern era, the DOS era.

> **Answer:** DOS era → GUI era (1984) → Modern era.

**Problem 11.** Name the OS family most likely running on a server
behind a favorite app, and explain why in one sentence.

> **Answer:** Linux/UNIX. Its open-source lineage is why it quietly
> powers most of the world's servers and cloud data centers.

**Problem 12.** Using round-robin scheduling with three processes,
Browser, Music, and Video call, each getting a 10ms time slice
(Browser 0-10ms, Music 10-20ms, Video call 20-30ms, Browser again
30-40ms), which process runs from 40-50ms?

> **Answer:** Music. The rotation repeats in the same fixed order.
