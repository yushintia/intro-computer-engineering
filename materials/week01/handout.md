# Week 1 Handout: Introduction to Computer Engineering

Introduction to Computer Engineering (400507-001) · Week 1
This handout goes with the Week 1 slides. Keep it for the whole semester.

---

## 1. Glossary: Key Words

Simple, plain definitions. Read these before or after class.

| Word | Plain definition |
|---|---|
| **Device** | A phone, laptop, or tablet you use every day. |
| **Hardware** | The physical parts of a device. You can touch them. Example: screen, chip, battery. |
| **Software** | The instructions that tell hardware what to do. You cannot touch it. |
| **App** | A software program you open. Example: a game, a camera app, a video-call app. |
| **Computer system** | Hardware and software working together. Neither works alone. |
| **Operating system (OS)** | Special software that manages all apps and hardware together. Example: Windows, Android, iOS. |
| **CPU** | The chip that runs instructions. People call it the "brain" of the device. |
| **Memory (RAM)** | Space that holds data only while an app is running. It empties when power turns off. |
| **Storage** | Space that keeps data even when the power is off. Example: a hard drive, a phone's storage. |
| **Network** | The connection that lets devices talk to each other. Example: wifi, mobile data. |
| **Layer** | One level in a stack of parts. Each layer depends on the layer below it. |
| **Logic gate** | A tiny on/off switch inside a chip. Everything in a computer is built from these. |
| **Crash** | When an app suddenly stops working. |
| **Freeze** | When a screen or app stops responding, but does not fully close. |
| **Overheat** | When a device or chip gets too hot to work normally. |
| **Diagnose** | To figure out what is wrong, and why. |

---

## 2. The Frozen Call, Step by Step

This is the full version of the story from class. The slide version was
shortened. Read this at home if you want more detail.

Four students are in a group project video call. They share one
screen. Everyone is talking about the slides at the same time.

Suddenly, one student's screen freezes. Her camera stops. Her voice
cuts out. A small spinning circle appears where her face used to be.

Everyone says the same thing: "Just restart it." She restarts her
laptop. Thirty seconds later, she is back on the call. She apologizes,
but she has no idea what actually happened.

Nobody on the call can answer three simple questions:

1. What froze — her phone, the app, the internet, or all three?
2. Why did restarting fix it?
3. Could this happen again, and how would she know why?

This course exists to answer questions exactly like these. A frozen
screen can be caused by any of four different layers, and only one of
them is usually the real problem:

- **Hardware layer** — a chip got too hot, or ran out of working space.
- **Software layer** — the video-call app itself crashed.
- **Operating system layer** — the OS failed to share the device fairly between apps.
- **Network layer** — the internet connection dropped for a moment.

Restarting a device resets all four layers at the same time. That is
why "just restart it" often works, even when nobody knows which layer
actually failed. Over this semester, you will learn to look at each
layer separately, instead of guessing.

---

## 3. The Six Layers: App Icon to Chip

When you tap an app icon, six layers work together, from the top
(what you see) to the bottom (the physical chip):

1. **Application software** — the app itself, like a game or a video-call app.
2. **System software / OS** — shares the device fairly between all open apps.
3. **Programs & instructions** — the code the app is built from.
4. **CPU** — reads and runs those instructions, very fast, one at a time.
5. **Memory & storage** — holds the data and the program while it runs.
6. **Logic gates** — tiny on/off switches. Everything above is built from these.

Each remaining week of this course studies one of these six layers in
detail, starting from the bottom (logic gates, Week 3) and working
back up toward the top (application software, Week 6) and outward to
networks (Week 9) and programming (Week 10).

---

## 4. Optional Reading: More Detail

This section holds extra detail that was trimmed from the slides. It
is optional, but useful if you want to go deeper.

**Why "computer engineering" is its own field.** Before the 1970s,
building the physical computer (electrical engineering) and writing
programs for it (computer science) were separate, disconnected fields.
As computers became something every engineer needed to understand
from both sides, "computer engineering" formed as its own field, at
the seam between hardware and software. A frozen video call is a good
example of why that seam matters: explaining it needs both hardware
knowledge and software knowledge, not just one.

**Who works at each layer.** Real engineering jobs map onto the six
layers above:

- **Hardware engineer** — designs the CPU, memory, and physical chips.
- **Systems / OS engineer** — builds the software that shares one machine fairly.
- **Network engineer** — keeps machines talking to each other reliably.
- **Application developer** — builds the apps people actually use.
- **Security analyst** — protects every layer above from misuse.
- **AI / data engineer** — builds one of the newest layers, covered in Weeks 13-14.

**Why this matters in industry.** "Walk me through what happens when
you type a URL and press enter" is a very common interview question
in the tech industry. It is popular because it tests whether a
candidate understands the whole system, not just one narrow skill.
The same idea applies to "what happens when you tap an app icon" —
this course's whole first week.

---

## 5. Practice Problems (with Answers)

Try each problem yourself before checking the answer.

**Problem 1.** Name two things you can touch on your phone, and two
things you cannot touch.

> **Answer:** Touchable (hardware): screen, chip, battery, camera.
> Not touchable (software): the OS, an app, a photo file.

**Problem 2.** A friend says: "My laptop is just slow, I don't know
why." Name three different layers that could each explain this alone.

> **Answer:** Any three of: CPU overloaded, memory full, storage
> almost full, too many apps running, network connection is slow.

**Problem 3.** True or false: "A phone with no software installed can
still run apps." Explain your answer in one sentence.

> **Answer:** False. Hardware with no software cannot do anything
> useful; software is required to make hardware work.

**Problem 4.** Put these four layers in order, from what you see
first (top) to the physical chip (bottom): CPU, application software,
operating system, logic gates.

> **Answer:** Application software → operating system → CPU → logic
> gates.

**Problem 5.** A video-call app crashes, but the rest of the laptop
still works fine (other apps still run). Which single layer is most
likely responsible?

> **Answer:** The application software layer — the app itself, not
> the OS, CPU, or network.

**Problem 6.** Explain, in your own words and in two sentences or
less, why restarting a frozen device often fixes the problem.

> **Answer (sample):** Restarting resets every layer of the device at
> once. Whichever layer had the problem — hardware, software, OS, or
> a temporary network issue — starts fresh.
