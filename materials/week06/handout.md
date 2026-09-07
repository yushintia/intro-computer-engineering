# Week 6 Handout: Application Software

Introduction to Computer Engineering (400507-001) · Week 6
This handout goes with the Week 6 slides. Keep it for Quiz 1 and the final exam.

---

## 1. Glossary: Key Words

Simple, plain definitions. Read these before or after class.

| Word | Plain definition |
|---|---|
| **Application software (app)** | A program that helps a user do one specific task. Example: a photo editor, a game. |
| **System software** | Software that manages the whole computer. Example: the operating system. |
| **Killer app** | An app so useful, people buy the device just to use it. |
| **User** | The person using an app to get something done. |
| **Category** | A group of apps that do a similar kind of task. |
| **Interface** | The screen and buttons an app shows to a user. |
| **Request** | When an app asks the OS for something it needs, like memory. |
| **Resource** | Memory, storage, or CPU time that an app needs to run. |
| **Decode** | To turn stored data back into a picture, sound, or text. |
| **Render** | To draw something on a screen so a person can see it. |
| **Install** | To add a new app onto a device before using it. |
| **Update** | To replace an app with a newer, improved version. |
| **Utility software** | System software that keeps the machine healthy, without being the OS itself. Example: antivirus, disk cleanup. |
| **Spreadsheet software** | Apps for organizing numbers into rows, columns, and formulas. |
| **Communication software** | Apps for messaging, calling, and video chatting. |
| **Educational software** | Apps built for studying, practicing, and taking quizzes. |
| **Entertainment software** | Games and streaming apps, built purely to entertain. |
| **Productivity software** | Calendars, to-do lists, and note-taking apps. |
| **Navigation software** | Maps and route-finding apps. |
| **Source code** | Instructions in a human-readable programming language, written by a programmer. |
| **Compiler** | A program that translates all of a source code file into machine instructions once, in advance. |
| **Interpreter** | A program that translates and runs source code line by line, each time the program runs. |
| **Compiled** | Translated into a runnable program file once, in advance. |
| **Interpreted** | Translated and run line by line, with no separate translation step beforehand. |
| **Software license** | The set of rules that says how a program may be used, copied, changed, or shared. |
| **Proprietary** | A license where the company keeps the source code private; usually paid, and not legally modifiable. |
| **Open-source** | A license where the source code is public; anyone may read, modify, and often redistribute it. |
| **Freeware** | A license that is free to use, but keeps the source code private and disallows modification. |
| **Software distribution** | How a finished program gets from its developer onto the device that will run it. |
| **App store** | An online service that delivers programs instantly, over the internet, to a registered device. |

---

## 2. A Perfect Photo, Locked Away

This is the full version of the story from class. The slide version was
shortened. Read this at home if you want more detail.

You take a photo on your phone. It saves right away. Later, you can
find the file again, exactly where you left it. This part works
perfectly. It is exactly what Week 5 (Memory & Storage) promised:
data that is kept, and can be found again.

But imagine, just for a moment, that your phone had no photo app
installed at all. The file is still there. Every byte is safe. But
you cannot open it. You cannot see the picture. You cannot crop it,
brighten it, or send it to a friend.

The data was never the problem. Something else was missing: a
program built to read that exact kind of file, and turn it into a
picture you can actually see and use. That program is **application
software**.

This is the whole idea behind Week 6: stored data only becomes
useful once the right app decodes it and shows it to a real person.

---

## 3. Application vs. System Software, Plus a Third Face: Utility Software

These kinds of software work together, but they do very different
jobs:

- **Application software** does one task *for the user*. Examples: a
  word processor writes documents, a browser shows web pages, a
  photo editor edits pictures, a media player plays music or video, a
  messaging app sends texts, a game entertains you.
- **System software** manages the computer *itself*. The main example
  is the **operating system (OS)**, covered in full next week. It
  shares memory, storage, and CPU time between every app that is
  running.
- **Utility software** is a third face of system software: it keeps
  the machine healthy, without being the OS itself. Examples:
  antivirus scanners, disk cleanup tools, file compression tools.
  Like the OS, utility software manages the machine. Unlike the OS,
  it usually runs only when a user chooses to run it, rather than
  running constantly in the background.

An easy test: if a normal user opens it on purpose, to do a specific
job, it is application software. If it runs quietly in the
background, managing the machine itself, it is the OS. If it is a
system program a user runs on purpose to maintain the machine (not to
do a personal task like writing or browsing), it is utility software.

---

## 4. Extended App Categories

Beyond the everyday list (word processor, web browser, photo editor,
media player, messaging app, game), application software splits
further by function:

- **Spreadsheet** — organizing numbers into rows, columns, and formulas.
- **Communication** — messaging, calling, and video chatting with others.
- **Educational** — apps built for studying, practicing, and taking quizzes.
- **Entertainment** — games and streaming apps, built purely to entertain.
- **Productivity** — calendars, to-do lists, and note-taking apps.
- **Navigation** — maps and route-finding apps.

Classifying by function is exactly how app stores organize millions
of apps: comparing two word processors makes sense, but comparing a
word processor to a game does not. Job postings often ask for skill
with "spreadsheet software" or "communication tools," by category, not
by brand name.

---

## 5. From Source Code to Running Program

Every app started as text, typed by a person. A programmer writes
**source code**: instructions in a human-readable programming
language. That source code must be translated into a form the CPU can
actually execute before it becomes a running program, using either a
**compiler** or an **interpreter**:

- **Compiled** — the entire source code is translated into machine
  instructions once, in advance, producing a program file you can run
  directly, again and again.
- **Interpreted** — the source code is translated and run line by
  line, each time the program runs, with no separate translation step
  beforehand.

Week 10 returns to this in far more depth, once you have written code
of your own.

---

## 6. Software Licensing

A **software license** is the set of rules that says how a program may
be used, copied, changed, or shared. Most software falls into one of
three common models:

- **Proprietary** — the company keeps the source code private; you
  usually pay to use it, and cannot legally modify it.
- **Open-source** — the source code is published publicly; anyone may
  read, modify, and often redistribute it.
- **Freeware** — free to use, but the source code stays private, and
  modification is not allowed.

**"Free" vs. "open-source"** are easy to mix up. Freeware means no
cost to use; the source code is still hidden. Open-source means the
source code is public and modifiable; it may or may not also be free
of cost. "Free" describes a price. "Open-source" describes access to
the code. They answer two different questions. Licensing shapes more
than price: it decides whether you can legally copy software for a
friend, whether a company or a community fixes bugs, and whether you
can see and trust exactly what a program does.

---

## 7. Software Distribution

**Software distribution** is how a finished program gets from its
developer onto the device that will run it. Decades ago, software
shipped physically, on floppy disks and then CDs, bought in a store.
Today, an **app store** delivers the same kind of program instantly,
over the internet, to any registered device.

Installing an app is a specific set of steps, not magic: the device
downloads the program's files from a server, those files are copied
onto secondary storage (recall Week 5), and the operating system
registers the new program so it appears as an icon you can open. An
**update** simply repeats the install process with newer files,
replacing the old version already on storage — that is why an update
still needs a network connection and free storage space, exactly like
a first-time install.

---

## 8. How a File Becomes a Photo

When you open a photo, three things happen in order:

1. **In storage:** the photo is only bytes — `1`s and `0`s. It is not
   a picture yet, just data sitting still.
2. **The app opens it:** the photo app reads those bytes and decodes
   them into color and shape information.
3. **The screen renders it:** the app draws the actual photo on
   screen. Now you can see it, crop it, or share it.

The same three steps happen for every file type: a music app decodes
audio bytes into sound, a word processor decodes text bytes into
words on a page.

---

## 9. Optional Reading: More Detail

This section holds extra detail that was trimmed from the slides. It
is optional, but useful if you want to go deeper.

**Where "apps" came from.** In the 1950s and 1960s, computers were
rare and expensive. Each one usually ran a single custom program,
written by a trained specialist, for one specific task. There was no
idea yet of an ordinary person picking an "app" off a shelf.

That changed in 1979, with a program called **VisiCalc**, the first
spreadsheet program, built for the Apple II computer. For the first
time, an ordinary person — an accountant, a small business owner —
could use a computer directly for their own real work, with no
programming knowledge at all. People started buying the Apple II
computer *just to run VisiCalc*. This made VisiCalc history's first
"killer app": an app so useful, it sold the hardware by itself.

**Why every app still needs the OS.** No app runs completely alone.
When an app opens, it asks the operating system for memory to hold
its data. When it reads a file, it asks the OS to reach into storage.
When it runs its instructions, it asks the OS for CPU time. The app
makes requests; the OS decides how to share the machine fairly among
every app that is running at once. That sharing problem is exactly
what Week 7 studies.

**Why this matters in industry.** "App developer" and "software
engineer" are some of the most common job titles in the tech
industry. Interviewers often ask candidates to explain the
difference between application software and system software, because
it shows whether a candidate understands where their own code will
actually run.

---

## 10. Practice Problems (with Answers)

Try each problem yourself before checking the answer.

**Problem 1.** Name two examples of application software, and one
example of system software.

> **Answer:** Application software (any two): a web browser, a photo
> editor, a word processor, a game, a messaging app. System software:
> the operating system.

**Problem 2.** True or false: "A file's data being safely stored
means a user can already use it." Explain your answer in one
sentence.

> **Answer:** False. Stored data still needs an app to decode it and
> show it to the user before it becomes usable.

**Problem 3.** A friend says: "My phone has more storage than ever,
so it should feel faster with more apps installed." Explain why this
is not always true.

> **Answer:** More installed apps can use more memory and CPU time,
> which can slow the device down, even with plenty of storage space.

**Problem 4.** Put these three steps in order: "the app renders the
photo on screen," "the photo file sits in storage as bytes," "the app
decodes the bytes into color and shape."

> **Answer:** The photo file sits in storage as bytes → the app
> decodes the bytes into color and shape → the app renders the photo
> on screen.

**Problem 5.** Name one resource that an app requests from the
operating system every time it runs.

> **Answer:** Any one of: memory, storage access, or CPU time.

**Problem 6.** Explain, in your own words and in two sentences or
less, why VisiCalc is called the first "killer app."

> **Answer (sample):** VisiCalc was so useful that people bought the
> Apple II computer just to run it. It proved that one great app
> could sell the hardware underneath it.

**Problem 7.** A friend's antivirus program is not application
software and not the OS itself. What is it, and why?

> **Answer:** Utility software. It keeps the machine healthy (in this
> case, scanning for threats), but it is not the OS itself, and it
> usually runs only when chosen, not constantly like the OS.

**Problem 8.** Name the extended app category (spreadsheet,
communication, educational, entertainment, productivity, or
navigation) that best fits a maps app used to find a bus stop.

> **Answer:** Navigation.

**Problem 9.** Explain the difference between compiled and
interpreted code, in one or two sentences.

> **Answer:** Compiled code is translated into machine instructions
> once, in advance, producing a program file that runs directly.
> Interpreted code is translated and run line by line, each time the
> program runs.

**Problem 10.** A friend says: "This app is freeware, so it must be
open-source too." Explain why this is not necessarily true.

> **Answer:** Freeware only means the app is free to use; its source
> code can still be private and unmodifiable. Open-source specifically
> means the source code is public and can be modified, which is a
> separate question from price.

**Problem 11.** Why does updating an app still require a network
connection and free storage space, just like installing it the first
time?

> **Answer:** An update repeats the install process with newer files,
> downloading them and writing them to storage in place of the old
> version, so it needs the same network access and storage space as a
> first install.
