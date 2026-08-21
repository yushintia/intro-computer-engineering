# Week 15 Final Exam Review Guide

Introduction to Computer Engineering (400507-001) · Week 15
This guide has the same fifteen review questions as the Week 15
slides, with full worked answers. Use it to study for the final
exam. It covers Weeks 1 through 14. **The final exam is cumulative**
and worth **30%** of your grade, the same weight as the midterm.

The questions below lean toward Weeks 9-14, the material taught
after the midterm. Weeks 1-7 were already reviewed in the Week 8
midterm guide, so they appear here only as a quick refresh.

---

## Weeks 1-7: Quick Refresh

These weeks were the whole midterm. Here is one small check for
each half, just to keep them fresh before the final.

**Q1. Put these three CPU steps in order: decode, execute, fetch.**

> **Answer:** **Fetch → decode → execute.** The CPU first *fetches*
> the next instruction from memory. Then it *decodes* the
> instruction, working out what it means. Finally it *executes* the
> instruction, actually doing the action. This cycle repeats for
> every single instruction a program runs.

**Q2. True or false: memory (RAM) keeps its data with no power.**

> **Answer:** **False.** Memory (RAM) only holds data while the
> power stays on. It empties the moment power stops. **Storage**
> (a hard drive, or a phone's storage) is the part that keeps data
> even after the power is off. A device needs both: memory for
> speed while it works, and storage for keeping data long-term.

---

## Week 9: Computer & Internet

**Driving question:** "How do two separate machines find each
other and exchange information?"

**Q3. What does an IP address let one device do?**

> **Answer:** It lets one device find, and be found by, other
> devices on a network. Just like a street address lets mail reach
> the right house, an IP address lets data reach the right device.
> No two devices on the same network share the same address.

**Q4. In a browser and a website, which one asks the question:
client or server?**

> **Answer:** The **client** asks. The **server** holds and sends
> the answer. Your browser is a client: it sends a small request.
> A website lives on a server, somewhere else, and sends the
> answer back, broken into small packets.

---

## Week 10: Programming Language

**Driving question:** "What is a programming language, and why do
computers need one?"

**Q5. Name the three building blocks of any program.**

> **Answer:** **Sequence, loop, and decision.** A sequence is steps
> done one after another, in order. A loop repeats the same steps
> many times. A decision lets a program pick between two paths,
> like "skip this file" or "keep going." Every program, no matter
> how large, is built from just these three blocks.

**Q6. What does a translator (compiler or interpreter) do to
code?**

> **Answer:** It changes code a person wrote into signals only a
> chip can understand. A **compiler** translates all the code at
> once, before the program runs. An **interpreter** translates one
> line at a time, while the program runs. Either way, a person's
> readable code becomes something the CPU can actually execute.

---

## Week 11: Databases & Security

**Driving question:** How do programs store, find, and protect
data safely, long after they run?

**Q7. In a simple data table, what does one row usually hold?**

> **Answer:** **One record.** A row in a database table holds one
> complete item: one student, one product, or one order. Each
> column across that row holds one piece of information about it,
> like a name, a price, or a date. Many rows together make a full
> table of records.

**Q8. Name the short language people use to ask a database a
question.**

> **Answer:** **SQL** (Structured Query Language). SQL lets a
> person ask a database for exact data, such as "show me every
> order from this month." A database can hold millions of rows;
> SQL is how a person finds only the few rows they actually need.

**Q9. Name one simple way to keep your account safe from
strangers.**

> **Answer:** Use a strong, private password, and never share it
> with anyone else. Other good habits include not reusing the same
> password on many sites, and turning on extra login checks when a
> service offers them. Security protects the data a database
> stores, so both ideas from this week work together.

---

## Week 12: Computer Applications

**Driving question:** What are the many everyday jobs a single
computer can do, beyond the ones already studied?

**Q10. Give one example of application software used for
multimedia.**

> **Answer:** Sample answers: a photo editor, a music player, or a
> video-editing app. Multimedia software works with pictures,
> sound, and video, letting a person create or enjoy media on an
> ordinary computer or phone.

**Q11. Name one everyday task a mobile app helps you finish.**

> **Answer:** Sample answers: mobile banking, messaging a friend,
> navigating to a new place, or ordering food. A single phone runs
> many different apps, and each one applies the same hardware and
> software ideas from earlier weeks to one specific, everyday job.

---

## Week 13: AI

**Driving question:** How does a computer learn to make a
prediction, instead of just following fixed steps?

**Q12. What does an AI model need a lot of, before it predicts
well?**

> **Answer:** **Training data.** An AI model looks at many past
> examples first, and learns the pattern hidden inside them.
> More good, relevant data usually leads to better predictions.
> Poor or too little data leads to a poor, unreliable model.

**Q13. True or false: a trained AI model can still be wrong.**

> **Answer:** **True.** A trained model learns a pattern from past
> data, but it does not truly "understand" the world. It can
> still make mistakes on new examples that look different from
> what it was trained on. This is why people still check and
> question AI answers, instead of trusting them blindly.

---

## Week 14: Emerging Technologies

**Driving question:** What comes after today's tools, and why does
this field never really stop moving?

**Q14. Name one example of a new, still-changing technology.**

> **Answer:** Sample answers: the Internet of Things (everyday
> objects connected to a network), quantum computing, or wearable
> devices like a smartwatch. Each one builds on ideas from earlier
> in the course, applied to a technology that is still young.

**Q15. Why do computer engineers keep learning after this course
ends?**

> **Answer:** Technology keeps changing, fast. Today's newest idea
> will not stay newest for long. The layers this course taught —
> hardware, software, the OS, networks, programs, data — stay
> useful, but the exact tools built on top of them keep changing
> every year. Learning continues, well beyond this one course.

---

## Study Checklist

Before the final exam, make sure you can do each of these.

**Weeks 1-7 (already reviewed for the midterm):**
- [ ] Name a hardware part and a software part (Week 1).
- [ ] Put computer history generations in the right time order (Week 2).
- [ ] Fill in a truth table for AND, OR, and NOT gates (Week 3).
- [ ] Say the fetch, decode, execute cycle in order (Week 4).
- [ ] Explain the difference between memory and storage (Week 5).
- [ ] Give examples of application software and system software (Week 6).
- [ ] Explain what an operating system manages (Week 7).

**Weeks 9-14 (the newer half, weighted more heavily today):**
- [ ] Explain what an IP address does, and why every device needs one (Week 9).
- [ ] Explain the difference between a client and a server (Week 9).
- [ ] Name the three building blocks of any program (Week 10).
- [ ] Explain what a compiler or interpreter does (Week 10).
- [ ] Explain what a row and a column hold, in a data table (Week 11).
- [ ] Name what SQL is used for (Week 11).
- [ ] Name one good password or account-safety habit (Week 11).
- [ ] Give an example of multimedia and mobile application software (Week 12).
- [ ] Explain why AI models need training data (Week 13).
- [ ] Explain why a trained AI model can still be wrong (Week 13).
- [ ] Name one example of an emerging technology (Week 14).
