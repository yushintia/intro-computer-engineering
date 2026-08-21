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

## 3. Application Software vs. System Software

These two kinds of software work together, but they do very
different jobs:

- **Application software** does one task *for the user*. Examples: a
  word processor writes documents, a browser shows web pages, a
  photo editor edits pictures, a media player plays music or video, a
  messaging app sends texts, a game entertains you.
- **System software** manages the computer *itself*. The main example
  is the **operating system (OS)**, covered in full next week. It
  shares memory, storage, and CPU time between every app that is
  running.

An easy test: if a normal user opens it on purpose, to do a specific
job, it is application software. If it runs quietly in the
background, managing the machine, it is system software.

---

## 4. How a File Becomes a Photo

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

## 5. Optional Reading: More Detail

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

## 6. Practice Problems (with Answers)

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
