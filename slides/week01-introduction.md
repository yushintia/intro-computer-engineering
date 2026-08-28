---
marp: true
theme: shintia
paginate: true
footer: 'Department of Intelligent Computing'
---

<!-- SLOT 1: Title -->
<!-- _class: title -->

# Week 1: Introduction

<span class="subtitle">Introduction to Computer Engineering (400507-001)</span>

<div class="meta">
Yushintia Pramitarini, Ph.D · Dept. of Intelligent Computing · Thu [1-3] · 성파 701
</div>

<!--
notes: Welcome the class. This session is the course contract: what this
course covers, how it's graded, what's expected of you, and how the
semester runs. No technical content yet - that starts next week.
-->

---

<!-- SLOT 2: Where we are -->

# Where We Are

<div class="roadmap">
<div class="wk now"><div class="n">Wk 1</div><div class="t">Introduction</div></div>
<div class="wk"><div class="n">Wk 2</div><div class="t">Computer History</div></div>
<div class="wk"><div class="n">Wk 3</div><div class="t">Boolean Logic</div></div>
<div class="wk"><div class="n">Wk 4</div><div class="t">CPU &amp; Instructions</div></div>
<div class="wk"><div class="n">Wk 5</div><div class="t">Memory &amp; Storage</div></div>
<div class="wk"><div class="n">Wk 6</div><div class="t">Application Software · Quiz 1</div></div>
<div class="wk"><div class="n">Wk 7</div><div class="t">Operating Systems</div></div>
<div class="wk review"><div class="n">Wk 8</div><div class="t">Midterm Exam</div></div>
<div class="wk"><div class="n">Wk 9</div><div class="t">Computer &amp; Internet</div></div>
<div class="wk"><div class="n">Wk 10</div><div class="t">Programming Language</div></div>
<div class="wk"><div class="n">Wk 11</div><div class="t">Databases &amp; Security</div></div>
<div class="wk"><div class="n">Wk 12</div><div class="t">Computer Applications</div></div>
<div class="wk"><div class="n">Wk 13</div><div class="t">AI · Quiz 2</div></div>
<div class="wk"><div class="n">Wk 14</div><div class="t">Emerging Technologies</div></div>
<div class="wk review"><div class="n">Wk 15</div><div class="t">Final Exam</div></div>
</div>

<!-- notes: Point at the row. Say: "Fifteen weeks. Today's the odd one out
- it's about how this course works, not a topic. Weeks 8 and 15 are
exams; the other twelve each open one more part of the device in your
hand." -->

---

<!-- Course intro: why this course, briefly, before the contract -->

# Why This Course

<div class="thread">One idea, plain and simple.</div>

> Every phone, laptop, and game console you own is a computer system.
> This course explains what is inside it, and how the parts work
> together.

That is not a sales pitch. It is the whole point of this major. Later
courses, and many jobs in this field, assume you already understand
the basic shape of a computer system - hardware and software,
together. This is the course where you first learn to see what is
really happening inside the device in your hand.

"What happens when you tap an icon?" is a common interview question.
After this course, it stops being a mystery.

---

<!-- Running-example tease: premise only, no numbers, no teaching -->

# The Call That Froze

<div class="pain">

Four students are on a video call. They share a screen. They talk
about their project.

Suddenly, one student's screen freezes. Her camera stops. Her voice
stops too.

"Just restart it," someone says. She does. Thirty seconds later, she
is back. But no one on the call can explain what just happened.

</div>

<!-- notes: Ask: "Has this happened to you?" Let two or three students
answer. Do not explain the cause yet. This is a premise, not a lesson -
just let it sit. -->

---

<!-- Teaser / discussion prompt, framed as a question not answered today -->

# A Question We Will Not Answer Today

<div class="thread">Sit with this question. Week 2 starts to answer it.</div>

"Restart it" is not really an explanation. Something inside that
device caused the freeze, and something inside it fixed itself when
it restarted.

- What is actually inside the device that just froze?
- Is it one part, or many parts working together?

<!--
notes: A discussion prompt, not a lesson - do not answer it today. Let
the class sit with the question. This course spends the rest of the
semester answering it, one piece at a time, starting with where
computers came from in Week 2.
-->

---

<!-- SLOT 6: Driving question -->

<!-- _class: section -->

# This Course's Question

<div class="driving-q">"What is actually inside the device in your hand, and how do all of its parts work together?"</div>

---

# This Course's Five Goals

<div class="thread">Not just today's goals. This is the whole course, in five lines.</div>

| # | Goal (from the syllabus) | Where |
|---|---|---|
| 1 | Explain basic hardware and software structure | All semester |
| 2 | Understand how data and instructions work | Weeks 3-4 |
| 3 | Describe system software, OS, and networks | Weeks 6-7, 9 |
| 4 | Survey databases, security, and multimedia | Weeks 11-12 |
| 5 | Introduce AI, IoT, cloud, and mobile tech | Weeks 13-14 |

Every one of these five goals is built, piece by piece, starting from
the frozen call you just heard about.

---

<!-- _class: section -->

# End of 차시 1
<div class="driving-q">Short break. Next: the course contract - what's covered, how you're graded, and what's expected of you.</div>

---

# Course Description

<div class="thread">From the official syllabus.</div>

This course introduces the fundamentals of computer engineering: how
hardware and software work, separately and together, and how they
connect to networks, data, and modern applications like AI. You do
not need to write code for this course. By the end, you will be able
to explain, in plain terms, what is happening inside every device you
use.

---

# Learning Objectives

<div class="thread">The official course objectives, from the syllabus - what you'll be able to do by Week 15.</div>

By the end of this course, you can:

<style scoped>
.cardlist { gap: 10px; margin-top: 6px; }
.cardlist .card { padding: 8px 18px; }
.cardlist .card .h { font-size: 17px; margin-bottom: 2px; }
.cardlist .card .d { font-size: 15px; line-height: 1.25; }
</style>

<div class="cardlist">
<div class="card"><div class="h">Hardware &amp; Software</div><div class="d">Explain the basic structure of computer hardware and software.</div></div>
<div class="card"><div class="h">CPU Processing</div><div class="d">Describe how a CPU processes data and instructions.</div></div>
<div class="card"><div class="h">OS, Networks &amp; Internet</div><div class="d">Explain how operating systems, networks, and the internet connect devices.</div></div>
<div class="card"><div class="h">Databases &amp; Multimedia</div><div class="d">Describe the basics of databases, security, and multimedia.</div></div>
<div class="card"><div class="h">AI, IoT &amp; Mobile</div><div class="d">Recognize the basics of AI, IoT, cloud, and mobile technology.</div></div>
</div>

---

# Prerequisites

<div class="thread">What this course assumes you already have.</div>

No prerequisite course is needed. Here is why:

- **You already use devices.** Phones, laptops, game consoles. You are
  already an expert user.
- **You already troubleshoot.** You restart devices. You close apps.
  You check your signal. These are early versions of ideas in this
  course.
- **You are curious.** That is the only real requirement.

This course does not expect you to know how to code. By the end, you
will understand hardware and software, at least the basics.

---

# Textbooks

<div class="thread">One primary text. One optional reference.</div>

- **Primary:** Harris & Harris, *Digital Design and Computer
  Architecture* (RISC-V ed.), 2021
- **Reference:** Tanenbaum & Austin, *Structured Computer
  Organization*, 6th ed.
- **Also:** these lecture slides themselves are a listed course
  reference

---

# How This Course Runs

<div class="thread">What to expect from a 3-period block, every week.</div>

Each week has three class periods (차시), about 50 minutes each:

<div class="cardlist">
<div class="card"><div class="h">A short lecture</div><div class="d">New words and ideas, explained simply, always starting from a real device you already own.</div></div>
<div class="card"><div class="h">A recap</div><div class="d">What last week delivered, and what it left unsolved.</div></div>
<div class="card"><div class="h">In-class activities</div><div class="d">Worksheets, discussion, and pair work, with answers discussed right after.</div></div>
<div class="card"><div class="h">Some weeks, a short quiz</div><div class="d">Week 6 and Week 13, to check your understanding before the midterm and final.</div></div>
</div>

You will talk in this class, not just listen.

---

# Weekly Schedule

<div class="thread">One line per week - the full walkthrough.</div>

| Wk | Topic | Wk | Topic |
|---|---|---|---|
| 1 | Introduction (today) | 9 | Computer & Internet |
| 2 | Computer History | 10 | Programming Language |
| 3 | Boolean Logic | 11 | Databases & Security - **Assignment 2** |
| 4 | CPU & Instructions - **Assignment 1** | 12 | Computer Applications |
| 5 | Memory & Storage | 13 | AI - **Quiz 2** |
| 6 | Application Software - **Quiz 1** | 14 | Emerging Technologies |
| 7 | Operating Systems | 15 | **Final Exam** (Wks 9-14) |
| 8 | **Midterm Exam** (Wks 1-7) | | |

---

<!-- _class: section -->

# End of 차시 2
<div class="driving-q">Short break. Next: grading, assignments, and policy.</div>

---

# Grading

<div class="thread">Five components, 100% total.</div>

| Component | Weight |
|---|---|
| Attendance | 10% |
| Midterm (Wk 8) | 30% |
| Final (Wk 15) | 30% |
| Assignments (×2) | 10% |
| In-class items | 20% |

<div class="why">
<strong>Grade distribution guideline:</strong> A ≤30%, B ≤40%, C-F ≤30%
of the class. This may shift after the add/drop period, based on final
enrollment.
</div>

<!-- notes: Assignment 1 is due Week 4. Assignment 2 is due Week 11.
Quiz 1 is Week 6. Quiz 2 is Week 13. -->

---

# Assignments

<div class="thread">Two assignments and two quizzes, spaced across the semester.</div>

| Item | When | Counts toward |
|---|---|---|
| Assignment 1 | Due Week 4 | Assignments (10%) |
| Quiz 1 | Week 6 | In-class items (20%) |
| Assignment 2 | Due Week 11 | Assignments (10%) |
| Quiz 2 | Week 13 | In-class items (20%) |
| Midterm Exam | Week 8 | Midterm (30%) |
| Final Exam | Week 15 | Final (30%) |

---

# Feedback Policy

<div class="thread">From the syllabus, verbatim.</div>

> Assignments graded within one week with rubric and model answers;
> exam item-analysis shared with weak-topic guidance and individual
> review on request.

In plain terms: you will know what you got wrong, and why, quickly
enough for it to still matter for the next assignment or exam. If a
grade surprises you, email the professor - a short one-on-one review
is always available, and clears up more than a rubric alone can.

---

# Attendance & Late Work

<div class="thread">Concrete rules, stated once, so nobody is surprised later.</div>

<div class="cardlist">
<div class="card"><div class="h">Attendance</div><div class="d">is 10% of your grade and is recorded every session.</div></div>
<div class="card"><div class="h">Late arrival</div><div class="d">arriving within 15 minutes of the start is on-time; after that, you're marked late. Three lates equal one absence.</div></div>
<div class="card"><div class="h">Can't attend?</div><div class="d">Email the professor <em>before</em> the session to be marked excused - unexcused absences aren't eligible for makeup credit.</div></div>
<div class="card"><div class="h">Late work</div><div class="d">loses 10% of that assignment's grade per day late, up to 3 days. No credit after 3 days, unless arranged with the professor in advance.</div></div>
</div>

---

# Academic Integrity

<div class="thread">Same principle as attendance: stated once, plainly.</div>

- **Academic integrity:** submit your own work. Copying another
  student's work, having someone else complete it for you, or
  submitting unattributed AI-generated work as your own is a
  violation.
- **First violation:** zero credit on that assignment or exam, plus a
  formal report. **Repeat violation:** may result in failing the
  course, per university policy.
- If anything here is unclear, ask - now is the cheapest time to ask.

---

# Support for Students with Disabilities

<div class="thread">From the syllabus's accommodations section.</div>

- **Hearing-impaired:** front-row seating, lecture material files
  provided where possible, urgent notices given in writing
- **Mobility-impaired:** extended exam time
- **Other documented conditions:** extended exam time, materials
  provided in advance, enlarged exam copies, or other reasonable
  accommodation based on need

Contact the professor early, and the Disability Student Support
Center or Academic Affairs Team, so accommodations are ready before
you need them.

---

# Contact

<div class="thread">How to reach the professor.</div>

- **Email:** yushintia@deu.ac.kr
- **Office hours:** by email appointment
- Email is the fastest way to reach the professor outside of class.
  Please allow 1-2 business days for a reply, and put the course code
  or your name in the subject line so nothing gets lost.
- Questions about grading, accommodations, or anything confusing in
  this contract are always welcome - it's easier to ask early than to
  untangle a problem in Week 14.

---

<!-- SLOT N+1: Limits (Act 4 / CLOSE), reused verbatim in Week 2's slot 3
recap and echoed in its slot 4 pain slide - see SPINE.md's
orientation-variant note -->

# What Today Doesn't Give You Yet

<div class="limits">
You now know how this course runs, how you're graded, and what's
expected of you. You still do not know what is actually inside the
device that just froze on that call, or how it works. Knowing the
rules of the course is not the same as understanding what's inside
your own phone.
</div>

---

<!-- SLOT N+2: Bridge -->

# Next Week

Week 1 leaves **what's actually inside your device** unanswered.
**Week 2, Computer History**, begins to answer it: who built the
first computer, why, and how computing grew from room-sized machines
into the device now in your hand.

---

<!-- SLOT N+3: Summary -->

# Summary

- This course: how hardware and software work, separately and
  together, so you can explain what's happening inside your own
  device.
- Grading: Attendance 10%, Midterm 30%, Final 30%, Assignments 10%,
  In-class items 20%.
- Assignment 1 due Week 4, Assignment 2 due Week 11. Quiz 1 in Week 6,
  Quiz 2 in Week 13.
- Primary text: Harris & Harris (RISC-V ed., 2021). Contact:
  yushintia@deu.ac.kr.
- **Prepare:** think of one time your device confused you. Bring it to
  Week 2.

---

<!-- SLOT N+4: Thank You -->
<!-- _class: end -->

# Thank You
