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
| **Memory hierarchy** | The stack of memory types, from registers down to secondary storage, trading speed for size. |
| **Register** | Tiny storage built directly into the CPU chip; holds the exact value the CPU is using this instant. |
| **Cache** | A small, very fast memory next to the CPU that holds copies of recently used data. |
| **Secondary storage** | The formal name for HDD/SSD-type storage: permanent, and the biggest, slowest rung of the hierarchy. |
| **Cache hit** | The CPU asks for data, and it is already sitting in cache. |
| **Cache miss** | The CPU asks for data that is not in cache, and must wait for slower RAM instead. |
| **ROM (Read-Only Memory)** | Non-volatile memory that holds fixed instructions written once, at the factory, and rarely rewritten. |
| **Firmware** | The tiny startup program, stored in ROM, that runs the instant a device is powered on. |
| **Bit** | A single `1` or `0`; the smallest possible unit of data. |
| **Kilobyte (KB), Megabyte (MB), Gigabyte (GB), Terabyte (TB)** | Increasingly large groups of bytes, each roughly a thousand times bigger than the last. |
| **Powers of 2 vs. powers of 10** | Two different counting systems for the same unit names: memory sizes are technically powers of 2 (1 KB = 1,024 bytes); storage is usually advertised in powers of 10 (1 KB = 1,000 bytes). |
| **Access time** | How long a memory or storage device takes to locate a requested piece of data, and begin delivering it. |
| **Throughput** | How much data a device can transfer per second, once the transfer has already started. |
| **Clock speed** | Measured in GHz; how many basic timing cycles the CPU can execute every second. It says nothing about memory or storage speed. |
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

## 4. The Memory Hierarchy: Four Rungs

No single memory technology can be fast, huge, cheap, and permanent
all at once. Real computers solve this by stacking several kinds of
memory together, fastest and smallest closest to the CPU, slowest and
biggest farthest away. This stack is called the **memory hierarchy**:

1. **Registers** — tiny storage built directly into the CPU chip;
   holds the exact value the CPU is using this instant. Fastest, but
   only a few bytes.
2. **Cache** — a small, very fast memory next to the CPU; holds
   copies of data the CPU used recently. Very fast, a few MB.
3. **RAM (Memory)** — holds the whole running program and its data.
   Fast, several GB.
4. **Secondary storage** — keeps everything permanently, even
   powered off. Slowest, but TB-scale and cheapest per byte.

Each step down trades speed for size: bigger and cheaper, but slower
to reach. On one ordinary laptop, all four rungs are active at the
same moment: a loop counter sits in a register, a just-reloaded
webpage appears from cache, an open unsaved essay sits in RAM, and
last weekend's photos sit on the SSD (secondary storage).

---

## 5. Cache: Why It Exists, and Hits vs. Misses

The CPU can execute billions of instructions every second, but RAM
cannot supply new data anywhere near that fast. **Cache memory** is a
small, very fast memory placed between the CPU and RAM to close that
gap, storing copies of the data the CPU is most likely to need again
soon. Cache does not replace RAM; it catches the CPU's most common
requests before they ever reach it.

Every request to cache ends one of two ways:

- **Cache hit:** the requested data is already sitting in cache. The
  CPU gets it almost instantly.
- **Cache miss:** the data is not in cache. The CPU must wait for the
  much slower RAM, and a copy is then stored in cache for next time.

**Worked example.** Suppose a cache hit takes about 1 nanosecond, and
a cache miss takes about 100 nanoseconds. If 9 out of every 10
requests are hits:

(9 × 1 ns + 1 × 100 ns) ÷ 10 requests ≈ **10.9 ns average**

That average sits far closer to the hit speed than the miss speed,
which is exactly why designers work hard to keep the hit rate high. A
high hit rate is what actually makes a computer feel fast.

---

## 6. RAM vs. ROM: Two Different Jobs

Both RAM and ROM live inside a laptop, and both hold data, but they do
opposite jobs:

- **RAM (Random Access Memory)** — fast, volatile working memory. It
  holds the operating system in use, every open app, and your
  document's in-progress data. It changes every second you use your
  laptop.
- **ROM (Read-Only Memory)** — non-volatile memory. It holds the tiny
  startup program, called **firmware**, written once at the factory
  and rarely or never rewritten afterward. Without ROM's firmware, a
  laptop would not even know how to start loading anything.

ROM is not the same thing as secondary storage (HDD/SSD): both are
non-volatile, but ROM is small, fixed at the factory, and almost never
rewritten by a user, while secondary storage is large and meant to be
rewritten constantly, every time you save a file.

---

## 7. Measuring Data: Bits, Bytes, and Units

- **Bit** — a single `1` or `0`. The smallest possible unit of data
  (recall Week 3's Boolean logic).
- **Byte** — a group of 8 bits. The basic unit computers use to
  measure most everyday data. One typed letter of text takes up
  roughly one byte.

| Unit | Roughly Holds |
|---|---|
| Kilobyte (KB) | A short paragraph of text |
| Megabyte (MB) | One photo |
| Gigabyte (GB) | A short movie |
| Terabyte (TB) | Thousands of movies |

Each step up is about a thousand times bigger than the step before.

**Powers of 2 vs. powers of 10.** Computers naturally count in
binary, so memory sizes are technically powers of 2 (1 KB = 1,024
bytes). Storage is usually advertised using powers of 10, since it
produces bigger, rounder-looking numbers (1 KB = 1,000 bytes).
Neither convention is "wrong"; they are just two different counting
systems, used in two different places.

**Why your "256GB" drive shows less than 256GB.** A manufacturer's
256 GB uses powers of 10: 256 × 10⁹ = 256,000,000,000 bytes. Your
operating system reports storage using powers of 2 (1 "GB" = 2³⁰
bytes), so that exact same drive shows as roughly **238 GB** in your
file explorer. No data is missing — it is the same bytes, counted two
different ways.

---

## 8. Speed Beyond Clock Speed: Access Time and Throughput

Week 4 introduced **clock speed**, measured in gigahertz (GHz): how
many basic timing cycles the CPU can execute every second. A higher
clock speed lets the CPU do more work per second, but it says nothing
about how fast memory or storage can keep up with it.

Two other numbers describe that separately:

- **Access time** — how long a memory or storage device takes to
  locate a requested piece of data, and begin delivering it. Ranges
  from a fraction of a nanosecond for registers, up to several
  milliseconds for a spinning hard disk drive.
- **Throughput** — how much data a device can transfer per second,
  once the transfer has already started, usually measured in MB/s or
  GB/s.

Access time is how long you wait to merge onto a highway. Throughput
is how fast traffic moves once you are already on it. A device can be
slow to start (poor access time) but fast once moving (good
throughput), or the reverse. A higher-GHz laptop is not automatically
faster overall: slow storage or too little RAM can still bottleneck
even a fast CPU.

---

## 9. Optional Reading: More Detail

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

## 10. Practice Problems (with Answers)

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

**Problem 7.** Put these four rungs of the memory hierarchy in order,
from fastest to slowest: RAM, Registers, Secondary storage, Cache.

> **Answer:** Registers → Cache → RAM → Secondary storage.

**Problem 8.** A cache hit takes about 1 ns, and a cache miss takes
about 100 ns. If 9 out of 10 requests are hits, what is the
approximate average request time?

> **Answer:** (9 × 1 ns + 1 × 100 ns) ÷ 10 ≈ 10.9 ns.

**Problem 9.** True or false: "ROM is just another name for storage,
like an SSD." Explain your answer in one sentence.

> **Answer:** False. ROM is small, fixed at the factory, and almost
> never rewritten, while secondary storage (SSD/HDD) is large and
> meant to be rewritten constantly.

**Problem 10.** A drive is advertised as 256GB but shows as about
238GB in the file explorer. Explain why in one or two sentences.

> **Answer:** The manufacturer counts using powers of 10 (1 GB =
> 1,000,000,000 bytes), while the operating system counts using
> powers of 2 (1 GB = 2³⁰ bytes). No data is missing; it is the same
> bytes counted two different ways.

**Problem 11.** Explain the difference between access time and
throughput, in one or two sentences.

> **Answer:** Access time is how long a device takes to locate data
> and begin delivering it. Throughput is how much data flows per
> second once the transfer has already started. They measure
> different things.
