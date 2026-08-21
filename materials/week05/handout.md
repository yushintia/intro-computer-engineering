# Week 5 Handout: Memory & Storage

Introduction to Computer Engineering (400507-001) · Week 5
This handout goes with the Week 5 slides. Keep it for the whole semester.

---

## 1. Glossary: Key Words

Simple, plain definitions. Read these before or after class.

| Word | Plain definition |
|---|---|
| **Memory (RAM)** | Space that holds data only while a program runs. It empties when power turns off. |
| **Storage** | Space that keeps data even when the power is off. Example: a hard drive, a phone's storage. |
| **Volatile** | Loses its data as soon as power stops. RAM is volatile. |
| **Non-volatile** | Keeps its data even with no power. Storage is non-volatile. |
| **Save** | The action that copies data from memory into storage. |
| **Hard disk drive (HDD)** | An older kind of storage. It uses a spinning disk to read and write data. |
| **Solid-state drive (SSD)** | A newer kind of storage. It uses memory chips, with no moving parts. |
| **USB drive** | A small, portable storage device you plug in and carry around. |
| **Cloud storage** | Storage space kept on someone else's computer, reached over the internet. |
| **Byte** | A small unit that measures how much data fits in memory or storage. |
| **Speed** | How fast a part can read or write data. |
| **Crash** | When a program or device suddenly stops working. |
| **Auto-save** | A feature that saves your work automatically, again and again. |
| **Backup** | A second copy of a file, kept somewhere safe in case the first is lost. |
| **Restart** | Turning a device off, then on again. |

---

## 2. Minjun's Essay, Step by Step

This is the full version of the story from class. The slide version was
shortened. Read this at home if you want more detail.

Minjun sits down to write a long essay. He opens a word processor and
starts typing. For two hours, he writes, deletes, and rewrites
sentences. He never clicks the Save button, not even once.

Every single word he types goes straight into memory (RAM). Nothing
he writes reaches storage yet. Memory is fast, so his laptop feels
smooth and responsive the whole time. But memory is also volatile: it
only holds data while the power stays on.

Suddenly, his laptop battery dies. The screen goes black in an
instant. The moment the power stops, memory empties completely. Every
word Minjun typed disappears at that exact second.

He plugs in his charger and turns the laptop back on. His word
processor opens again, showing a blank, untitled document. There is
nothing to recover, because there was never a saved copy anywhere in
storage. Two hours of work are simply gone.

Now compare this to what would have happened if Minjun had clicked
Save partway through. Clicking Save tells the computer: "copy
whatever is in memory right now into storage." Storage is
non-volatile, so that copy would have survived the power cut. When he
turned the laptop back on, his document would open with everything he
had saved, up to the last time he clicked Save. Only the unsaved part
would be lost.

This is why word processors and other apps often nag you to save
often, and why many apps now include auto-save: a feature that copies
your work from memory into storage every few seconds, without you
asking.

---

## 3. Memory and Storage in Context

Every computer, from a phone to a laptop, uses both memory and
storage, because each one is good at a different job:

- **Memory (RAM)** sits close to the CPU (Week 4). It is very fast,
  but small and relatively expensive. It only holds data while a
  program is actively running.
- **Storage** sits further from the CPU. It is slower than memory,
  but much bigger and cheaper. It keeps data safely, with or without
  power.

Modern devices usually contain more than one kind of storage:

- **Hard disk drive (HDD):** an older technology. A spinning magnetic
  disk stores data, and an arm reads and writes it. Cheap and big, but
  slower, and it can be damaged by drops or shocks.
- **Solid-state drive (SSD):** a newer technology. Data is stored in
  memory chips, with no moving parts. Faster and sturdier than an
  HDD, but usually more expensive for the same amount of space.
- **USB drive:** small, portable storage, similar technology to an
  SSD, built to be carried between devices.
- **Cloud storage:** your files are stored on a computer owned by a
  company, somewhere else, and you reach them over the internet.

No single part can be fast, huge, cheap, and permanent all at once.
Every device mixes memory and several kinds of storage to balance
these trade-offs.

---

## 4. Optional Reading: More Detail

This section holds extra detail that was trimmed from the slides. It
is optional, but useful if you want to go deeper.

**Why the memory/storage split exists.** In the 1940s and 1950s,
early computers already had a way to hold data temporarily while
working, using technology that was fast but needed constant power.
Permanent storage existed too, in the form of punch cards and paper
tape, but reading them was extremely slow, one card at a time. Neither
option alone was good enough: computers needed something fast to work
with, and something separate and reliable to keep results in. In
1956, IBM built the RAMAC 305, generally considered the first
computer with a hard disk drive. It was roughly the size of two
refrigerators and could store about 5 megabytes, tiny by today's
standards, but revolutionary at the time: for the first time, a
computer could jump directly to any piece of stored data, instead of
reading through a whole stack of cards in order.

**Why this matters in industry.** "What is the difference between RAM
and storage, and why does my computer need both?" is a common
interview and exam question in computing fields. It tests whether a
candidate understands a basic trade-off that shapes nearly every
piece of hardware: speed versus permanence. The same idea explains
why phones, laptops, servers, and even smartwatches all include both
kinds of space, not just one.

**A note on "deleting" a file.** Deleting a file from storage does
not always erase it instantly. Many systems just mark the space as
reusable, and the old data can sometimes still be recovered until
something else is saved over it. This is a big reason why simply
deleting a file is not considered a safe way to protect private data.

---

## 5. Practice Problems (with Answers)

Try each problem yourself before checking the answer.

**Problem 1.** Name one thing that memory (RAM) does, and one thing
that storage does.

> **Answer:** Memory holds the data and program a CPU is using right
> now, while the program runs. Storage keeps files safely, even when
> the power is off.

**Problem 2.** True or false: "A phone with no storage can still save
photos permanently." Explain your answer in one sentence.

> **Answer:** False. Without storage, there is nowhere non-volatile to
> keep the photo, so it would disappear when the power turns off.

**Problem 3.** A friend says: "SSDs and HDDs do the exact same job, so
it does not matter which one I buy." Is this true? Explain briefly.

> **Answer:** Not quite. Both are storage and both keep data with no
> power, but SSDs are faster and sturdier, while HDDs are usually
> cheaper for large amounts of space. The right choice depends on the
> need.

**Problem 4.** Put these three in order, from fastest to slowest:
**HDD, RAM, SSD.**

> **Answer:** RAM → SSD → HDD.

**Problem 5.** You are writing a document and the app crashes,
closing without warning. When you reopen it, most of your work is
still there, except the last two sentences. What likely happened?

> **Answer:** The app has auto-save, which had already copied most of
> the work from memory into storage. Only the part typed after the
> last auto-save was still in memory, and was lost in the crash.

**Problem 6.** Explain, in your own words and in two sentences or
less, why unsaved work disappears when a laptop suddenly loses power,
but saved files do not.

> **Answer (sample):** Unsaved work lives only in memory, which needs
> constant power to keep its data. Saved files live in storage, which
> keeps its data even with no power at all.
