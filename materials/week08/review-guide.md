# Week 8 Midterm Review Guide

Introduction to Computer Engineering (400507-001) · Week 8
This guide has the same ten review questions as the Week 8 slides,
with full worked answers. Use it to study for the midterm. It covers
Weeks 1 through 7.

---

## Week 1: Introduction

**Driving question:** "What is inside the device in your hand? How do
its parts work together?"

**Q1. Name one hardware part and one software part of a laptop.**

> **Answer:** Hardware is a part you can touch: the CPU, memory, the
> screen, or the battery. Software is a set of instructions you
> cannot touch: the operating system, or an app. A device needs both.
> Hardware alone cannot do anything useful without software to tell
> it what to do.

---

## Week 2: Computer History

**Driving question:** How did computers change from huge machines
into the small chip inside your device?

**Q2. Put these in time order: transistors, vacuum tubes, integrated
circuits.**

> **Answer:** Vacuum tubes → transistors → integrated circuits.
> Vacuum tubes came first. They were large, hot, and broke often.
> Transistors replaced them: smaller, cooler, and more reliable.
> Integrated circuits then packed many transistors onto one small
> chip. Each step made computers smaller, faster, and cheaper.

---

## Week 3: Boolean Logic

**Driving question:** "How do simple on/off switches let a computer
decide between true and false?"

**Q3. An AND gate has inputs true and false. What is the output?**

> **Answer:** **False.** An AND gate only outputs true when *every*
> input is true. One false input is enough to make the whole gate
> output false.

**Q4. An OR gate has inputs false and true. What is the output?**

> **Answer:** **True.** An OR gate outputs true when *at least one*
> input is true. Only both inputs false gives a false output.

---

## Week 4: CPU & Instructions

**Driving question:** How does a CPU turn one instruction into one
action?

**Q5. Put these three steps in order: decode, execute, fetch.**

> **Answer:** **Fetch → decode → execute.** The CPU first *fetches*
> the next instruction from memory. Then it *decodes* the
> instruction, working out what it means. Finally it *executes* the
> instruction, actually doing the action.

**Q6. True or false: a simple CPU runs many instructions at the exact
same instant.**

> **Answer:** **False.** A simple, single-core CPU runs one
> instruction at a time, one after another, very fast. It only looks
> like many things happen "at once" because each step is so quick.

---

## Week 5: Memory & Storage

**Driving question:** Where does a computer keep data, while it runs
and after power stops?

**Q7. Which one keeps data with no power: memory or storage?**

> **Answer:** **Storage** keeps data even when the power is off.
> Examples: a hard drive, or a phone's storage. **Memory (RAM)**
> only holds data while the power is on, and it empties when power
> stops.

**Q8. A laptop loses unsaved work after a power cut. What failed to
keep it?**

> **Answer:** **Memory (RAM).** Unsaved work lives in memory while
> you work on it. Memory needs constant power to hold data, so a
> power cut erases anything not yet saved to storage.

---

## Week 6: Application Software

**Driving question:** What turns raw hardware into something a person
can actually use?

**Q9. Give one example of application software, and one of system
software.**

> **Answer:** **Application software:** a game, a camera app, or a
> video-call app — something you open to do a task. **System
> software:** the operating system — software that manages the
> device itself, not a specific task.

---

## Week 7: Operating Systems

**Driving question:** How does one machine share itself fairly
between many running programs?

**Q10. Two apps are open at once. What decides which one uses the
CPU right now?**

> **Answer:** **The operating system.** It shares the CPU, memory,
> and other hardware fairly between every open app, switching
> between them so each one gets a turn.

---

## Study Checklist

Before the midterm, make sure you can do each of these:

- [ ] Name a hardware part and a software part (Week 1).
- [ ] Explain the six layers, from app icon to physical chip (Week 1).
- [ ] Put computer history generations in the right time order (Week 2).
- [ ] Explain why computers got smaller and cheaper over time (Week 2).
- [ ] Fill in a truth table for AND, OR, and NOT gates (Week 3).
- [ ] Combine two gates to model one everyday decision (Week 3).
- [ ] Say the fetch, decode, execute cycle in order (Week 4).
- [ ] Explain why a simple CPU runs one instruction at a time (Week 4).
- [ ] Explain the difference between memory and storage (Week 5).
- [ ] Explain why a device needs both memory and storage (Week 5).
- [ ] Give examples of application software and system software (Week 6).
- [ ] Explain what an operating system manages (Week 7).
