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
3. **Some requests get priority.** The video call needs smooth,
   steady sound. The OS gives its requests priority over the game
   download's disk requests, so your voice does not stutter.
4. **No app touches hardware directly.** The game download does not
   write to the disk by itself. It sends a request to the OS. The OS
   talks to the disk driver on the app's behalf.

This is why closing one frozen app usually saves the other four. The
OS was already keeping their memory and their CPU turns separate.

---

## 3. What the OS Manages: Three Jobs

Every operating system, no matter the brand, manages the same three
things:

1. **CPU time** — which process runs right now, and for how long.
2. **Memory** — how much space each process gets, and keeping that
   space private.
3. **Devices** — the screen, keyboard, disk, network card, and every
   other piece of hardware, reached only through a driver.

Each remaining week of this course builds outward from this idea:
Week 9 studies how machines talk to *each other*, once each machine
already manages itself well.

---

## 4. Optional Reading: More Detail

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

## 5. Practice Problems (with Answers)

Try each problem yourself before checking the answer.

**Problem 1.** Name the three things an operating system manages for
every running app.

> **Answer:** CPU time, memory, and devices (hardware like the
> screen, keyboard, disk, and network).

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
