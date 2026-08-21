---
marp: true
theme: shintia
paginate: true
footer: 'Department of Intelligent Computing'
---

<!-- SLOT 1: Title -->
<!-- _class: title -->

# Week 3: Boolean Logic

<span class="subtitle">Introduction to Computer Engineering (400507-001)</span>

<div class="meta">
Yushintia Pramitarini, Ph.D · Dept. of Intelligent Computing · Thu [1-3] · 성파 701
</div>

<!--
notes: Ask everyone to hold up their phone. Ask: "Does your phone ever
say yes or no to you?" Examples: low battery warning, wifi connected
or not. Collect two or three answers. Do not explain yet.
-->

---

<!-- SLOT 2: Where we are -->

# Where We Are

<div class="roadmap">
<div class="wk"><div class="n">Wk 1</div><div class="t">Introduction</div></div>
<div class="wk"><div class="n">Wk 2</div><div class="t">Computer History</div></div>
<div class="wk now"><div class="n">Wk 3</div><div class="t">Boolean Logic</div></div>
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

<!-- notes: Point at Week 3. Say: "Today we zoom into one layer: the tiny switches at the bottom of every chip." -->

---

<!-- SLOT 3: Recap + open wound -->

# Last Week, This Week

- **Last week delivered:** we saw how computers evolved. Huge early machines became the small chips in your laptop today.
- **Last week left broken:** we still do not know how those chips represent anything, as simply as on and off.

---

<!-- SLOT 4: The pain (Act 1 / MOTIVATE), ZERO jargon -->

# How Does a Switch Say "Yes"?

<div class="pain">

Your laptop is full of tiny switches. Each switch is only ever on or
off. Nothing else.

But your laptop does much more than that. It warns you when the
battery is low. It locks the screen when you walk away. It decides
things.

How can a machine made only of on/off switches ever decide anything
at all? Think about deciding whether to bring an umbrella. You check:
is it raining? Do I already have one at home? Somehow your mind turns
two yes/no answers into one decision. Can a switch do that too?

</div>

<!-- notes: Ask: "Has anyone thought about how a phone 'knows' the battery is low?" Let two students answer. Do not explain yet. -->

---

<!-- SLOT 5: Cost of not knowing -->

# What This Actually Costs

- Without this, "CPU" and "instructions" next week make no sense at all.
- You cannot read even the simplest circuit diagram in a textbook.
- Every chip inside every device you own is built from exactly this idea.

<div class="why">
<strong>In industry:</strong> Hardware and firmware interviews often
start with a truth table or a small logic circuit. Companies expect
every computer engineering graduate to read one on sight.
</div>

---

# Where Logic Gates Hide

<div class="thread">This is not just chip theory. It is everywhere already.</div>

<div class="appgrid">
<div class="app"><div class="name">Traffic light</div><div class="desc">Checks: is the timer done AND is the crossing clear?</div></div>
<div class="app"><div class="name">Washing machine</div><div class="desc">Checks: is the door closed AND is water full?</div></div>
<div class="app"><div class="name">Elevator</div><div class="desc">Checks: is a floor button pressed AND are doors closed?</div></div>
<div class="app"><div class="name">Thermostat</div><div class="desc">Checks: is the room cold OR is a timer set?</div></div>
<div class="app"><div class="name">Smoke detector</div><div class="desc">Checks: NOT enough clean air, so it must alarm.</div></div>
<div class="app"><div class="name">Game controller</div><div class="desc">Checks: is a button pressed, true or false, right now?</div></div>
</div>

---

<!-- SLOT 6: Driving question -->

<!-- _class: section -->

# This Week's Question

<div class="driving-q">"How do simple on/off switches let a computer decide between true and false?"</div>

---

<!-- SLOT 7: Learning outcomes -->

# By the End of This Week, You Can

1. Explain what a Boolean value is, and why computers use only two.
2. Read the truth table for an AND, OR, or NOT gate.
3. Combine gates to model a simple everyday decision.
4. Trace one decision inside a real device back to logic gates.

---

<!-- SLOT 8: Origin -->

# Where This Idea Came From

<div class="thread">You just felt the pain. Where did the answer come from?</div>

- **1854:** George Boole, a mathematician, wanted to write logical
  reasoning as math. He wrote a book called *The Laws of Thought*.
- **1937:** Claude Shannon, a student, noticed something huge: Boole's
  true/false math matches on/off electrical switches, exactly.

<div class="why">
Shannon's idea connected math to real circuits. It is the reason a
chip full of switches can "think" in true and false at all.
</div>

---

<!-- SLOT 9: Core concept -->

# Boolean Value: Definition

<div class="thread">One idea, one clear definition.</div>

> A **Boolean value** is a value that can only be **true** or
> **false**. Nothing in between.

- Computers store this as a **bit**: `1` means true (on), `0` means false (off).
- A raining/not-raining check is a Boolean value. So is on/off battery.

---

# Why Only Two Values?

<div class="thread">Why not use three states, or ten?</div>

- A switch is easy to build: it is clearly **on**, or clearly **off**.
- Electricity is noisy. Ten close voltage levels are hard to tell apart.
- Two states, far apart, are almost never confused. That makes chips reliable.

<div class="why">
This is why every chip, in every device, still uses only true and
false, on and off, even today.
</div>

---

<!-- NEW: Key Words Today, 차시 1 -->

# Key Words Today

- **Boolean value** — a value that is only true or false, never in between.
- **Bit** — a `1` or a `0`. The smallest piece of data a computer stores.
- **True / false** — the two, and only two, Boolean values.
- **On / off** — the everyday words for `1` and `0` inside a switch.
- **Gate** — a tiny circuit that takes true/false inputs and gives one true/false answer.

<!-- notes: Read each word aloud. Ask students to repeat it once. Ask: "Which of these words did you already know?" -->

---

<!-- NEW: Try-It preview, closes 차시 1 -->

# Coming Up: Worksheet Part A

<div class="thread">Next, you will practice using these words.</div>

- In **[Worksheet Part A](materials/week03/worksheet.html)**, you turn everyday decisions into true/false questions.
- Example: "Should I bring an umbrella?" becomes two true/false checks.
- You will work with a partner. A guess is fine for now.

<!-- notes: Tell students to sit next to a partner for the next part. No prep needed. -->

---

<!-- _class: section -->

# End of 차시 1
<div class="driving-q">Short break. 차시 2: the three gates that build every decision.</div>

---

<!-- NEW: Key Words Today, 차시 2 -->

# Key Words Today

- **AND gate** — true only when **both** inputs are true.
- **OR gate** — true when **at least one** input is true.
- **NOT gate** — flips one input: true becomes false, false becomes true.
- **Truth table** — a table showing every input and the matching output.
- **Circuit** — gates connected together to make one decision.

<!-- notes: Read each word aloud. Say: "You will use all five words in the next slides." -->

---

# What Is a Truth Table?

<div class="thread">One skill, used on every gate today.</div>

- A **truth table** lists every possible input, and the matching output.
- Read it row by row, left to right: inputs first, output last.
- If a gate has two inputs, it needs exactly four rows to show every case.

---

<!-- Act 3 / BUILD -->

# The AND Gate: Both Must Be True

<div class="thread">Back to the umbrella. Part one of the decision.</div>

**Bring umbrella = "It is raining" AND "I have none at home."**

| Raining? | No umbrella at home? | Bring umbrella? |
|---|---|---|
| No | No | No |
| No | Yes | No |
| Yes | No | No |
| Yes | Yes | **Yes** |

An AND gate says yes only when every single input says yes.

---

# The NOT Gate: Flip It

<div class="thread">Where did "no umbrella at home" come from?</div>

**"No umbrella at home" = NOT "I have an umbrella at home."**

| I have an umbrella at home? | No umbrella at home? |
|---|---|
| Yes | No |
| No | **Yes** |

A NOT gate has one input. It always gives the opposite answer back.

<!-- notes: Ask: "If the input is true, what does NOT give back?" Wait for "false" from the class. -->

---

# The OR Gate: Either Is Enough

<div class="thread">A second decision, same everyday world.</div>

**Get wet = "It is raining" OR "The sprinklers are on."**

| Raining? | Sprinklers on? | Get wet? |
|---|---|---|
| No | No | No |
| No | Yes | **Yes** |
| Yes | No | **Yes** |
| Yes | Yes | **Yes** |

An OR gate says yes if even one input says yes. Only both false stays false.

---

# Gate Cheat Sheet

<div class="thread">Three gates, three rules. Keep this in mind for the worksheet.</div>

| Gate | Rule | Everyday word |
|---|---|---|
| AND | True only if **every** input is true | "both", "all" |
| OR | True if **at least one** input is true | "either", "any" |
| NOT | Flips the one input it gets | "not", "no" |

---

# Practice Together: Fill the Table

<div class="thread">One example, as a class, before you work alone.</div>

**Turn on porch light = "It is dark" AND "Someone is home."**

| Dark? | Someone home? | Light on? |
|---|---|---|
| No | No | ? |
| No | Yes | ? |
| Yes | No | ? |
| Yes | Yes | ? |

<!-- notes: Ask the class to call out each "?" together. Fill it in live: No, No, No, Yes. Confirm it matches the AND rule. -->

---

<!-- NEW: Try-It hand-off, Worksheet Part A -->

# Try It: Worksheet Part A

<div class="thread">Now you practice. Work with a partner.</div>

- Open **[Worksheet Part A](materials/week03/worksheet.html)**.
- Fill in the truth table for each small AND/OR/NOT scenario.
- You have about 15 minutes. Ask your partner before you ask me.

<!-- notes: Hand out Worksheet Part A. Walk around and help pairs. After 15 minutes, ask 2-3 pairs to share one answer. -->

---

<!-- _class: section -->

# End of 차시 2
<div class="driving-q">Short break. 차시 3: combining gates, then a real chip.</div>

---

<!-- NEW: Key Words Today, 차시 3 -->

# Key Words Today

- **Combine** — connect two or more gates so one feeds the next.
- **Input** — a true/false value going into a gate.
- **Output** — the true/false answer a gate gives back.
- **Warning / alert** — a message a device shows after a logic decision.

<!-- notes: Read each word aloud. Say: "These words tie everything together today." -->

---

# Combining Two Gates: A Warm-Up

<div class="thread">One gate feeds another. Try a small chain first.</div>

**Skip the umbrella = NOT ("Raining" OR "Forecast says rain later").**

<div class="pipeline">
<div class="stage"><div class="h">Raining? / Forecast rain?</div><div class="s">OR gate</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Flip the answer</div><div class="s">NOT gate: skip umbrella</div></div>
</div>

The OR gate's output becomes the NOT gate's only input.

---

# Combining Gates: The Full Umbrella Decision

<div class="thread">Now put all three gates together.</div>

**Bring umbrella = ("Raining" OR "Forecast says rain later") AND
(NOT "Already carrying one").**

<div class="pipeline">
<div class="stage"><div class="h">Raining? / Forecast rain?</div><div class="s">OR gate</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Already carrying one?</div><div class="s">NOT gate</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Both true?</div><div class="s">AND gate: bring umbrella</div></div>
</div>

Real circuits chain small gates like this, one feeding the next.

---

# Big Idea: Simple Gates, Big Decisions

<div class="thread">Zoom out for a moment before the next case study.</div>

- One gate only makes one small true/false choice.
- Chain enough gates together, and the decisions get much more complex.
- A modern chip connects **billions** of gates this same simple way.

<div class="why">
Every app, every warning, every button on your laptop traces back to
gates like the three you just learned.
</div>

---

<!-- SLOT N-2: Worked example -->

# Case Study: A Real Warning Inside Your Laptop (1/2)

<div class="thread">Same idea, real device. Back to "What's Actually Inside Your Laptop."</div>

**Show low-battery warning = "Battery below 20%" AND NOT "Charger plugged in."**

<div class="pipeline">
<div class="stage"><div class="h">Charger plugged in?</div><div class="s">NOT gate</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Battery below 20%?</div><div class="s">AND gate</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Warning</div><div class="s">shows on your screen</div></div>
</div>

---

# Case Study: A Real Warning Inside Your Laptop (2/2)

<div class="thread">Trace three real runs through the same small circuit.</div>

- Battery 15%, no charger: **both true → warning shows.**
- Battery 15%, charger plugged in: NOT flips true to false → **no warning.**
- Battery 50%, no charger: first input already false → **no warning.**

Millions of gates like this run at once, deep inside the chip.

---

# Who Designs These Circuits

<div class="thread">Real jobs, built on exactly today's ideas.</div>

<div class="appgrid">
<div class="app"><div class="name">Hardware engineer</div><div class="desc">Designs the chip's physical gates and connections.</div></div>
<div class="app"><div class="name">Firmware engineer</div><div class="desc">Writes the low-level code closest to the hardware.</div></div>
<div class="app"><div class="name">Chip designer</div><div class="desc">Plans how millions of gates fit on one chip.</div></div>
<div class="app"><div class="name">Embedded / IoT engineer</div><div class="desc">Builds small devices that sense and decide, like a thermostat.</div></div>
<div class="app"><div class="name">Robotics engineer</div><div class="desc">Uses gates to make quick sensor-based decisions.</div></div>
<div class="app"><div class="name">Test engineer</div><div class="desc">Checks that every gate follows its truth table, exactly.</div></div>
</div>

---

<!-- SLOT N-1: Common mistakes -->

# Common Mistakes (1/2)

- **Mixing up AND and OR:** AND needs every input true. OR needs only one.
- **Forgetting NOT flips the value:** NOT never passes a value through unchanged.
- **Thinking a gate "thinks":** a gate only follows one fixed rule, every time.

---

# Common Mistakes (2/2)

- **Trusting daily English "or":** in daily talk, "or" can mean "not both." In logic, OR always allows both true.
- **Assuming one broken gate breaks everything:** a real chip has millions of gates. One part can fail alone.
- **Skipping the truth table:** guessing the output by eye leads to mistakes. Always check row by row.

---

<!-- NEW: Try-It hand-off, Worksheet Part B -->

# Try It: Worksheet Part B

<div class="thread">More practice. New scenarios.</div>

- Open **[Worksheet Part B](materials/week03/worksheet.html)**.
- Build a small truth table for each combined decision.
- You have about 15 minutes. Then we discuss answers together.

<!-- notes: Hand out Worksheet Part B. After 15 minutes, go through the answer key as a class. Ask for volunteers first. -->

---

<!-- SLOT N: Check yourself -->

# Check Yourself

1. An AND gate has inputs true and false. What is the output?
2. An OR gate has inputs false and false. What is the output?
3. A NOT gate has input true. What is the output?

---

# Answers

1. **False.** AND needs every input to be true. One false input is enough to fail.
2. **False.** OR needs at least one true input. Both false gives false.
3. **False.** NOT always flips the value: true becomes false.

---

<!-- NEW: Self-check quiz hand-off -->

# Self-Check Quiz

<div class="thread">One more check, on your own.</div>

- Take the **[Week 3 Quiz](materials/week03/quiz.html)** (5-8 short questions).
- This quiz is not graded. It just checks your understanding.
- About 10 minutes. Check your own answers at the end.

<!-- notes: Hand out the quiz. Give students 10 minutes. Then read the answer key aloud, or let students self-check. -->

---

# Quick Recap: Today in Three Gates

<div class="thread">Before we close, one more look at the whole picture.</div>

<div class="chip-row">
<span class="chip">Boolean value: only true or false</span>
<span class="chip">AND: every input true</span>
<span class="chip">OR: at least one input true</span>
<span class="chip">NOT: flips the input</span>
<span class="chip">Combined gates: build one decision</span>
</div>

---

<!-- SLOT N+1: Limits (Act 4 / CLOSE), becomes Week 4 slot 4 -->

# What Gates Cannot Do Yet

<div class="limits">
Gates can now decide true or false, one decision at a time. But a
gate cannot remember what happened before. It cannot follow a list of
steps, one after another. That is a **program**. We do not have that
yet.
</div>

---

<!-- SLOT N+2: Bridge -->

# Next Week

Week 3 leaves **following a sequence of steps** unsolved. Gates decide
one thing at a time, but nothing links their decisions together.
**Week 4, CPU & Instructions**, addresses it: how a chip runs a
program, one instruction at a time.

---

<!-- SLOT N+3: Summary -->

# Summary

- A Boolean value is only ever true or false, stored as a bit: 1 or 0.
- AND needs every input true. OR needs one. NOT flips its single input.
- Combined gates model real decisions, from umbrellas to battery warnings.
- **Reading:** Harris & Harris, Chapter 2 (sections on Boolean algebra and logic gates).
- **Handout:** [materials/week03/handout.md](materials/week03/handout.html), glossary and the full worked example.
- **Prepare:** Think of one on/off decision your own phone makes. Bring it to Week 4.

---

<!-- SLOT N+4: Thank You -->
<!-- _class: end -->

# Thank You
