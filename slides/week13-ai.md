---
marp: true
theme: shintia
paginate: true
footer: 'Department of Intelligent Computing'
---

<!-- SLOT 1: Title -->
<!-- _class: title -->

# Week 13: AI

<span class="subtitle">Introduction to Computer Engineering (400507-001)</span>

<div class="meta">
Yushintia Pramitarini, Ph.D · Dept. of Intelligent Computing · Thu [1-3] · 성파 701
</div>

<!--
notes: Ask everyone to open their phone's photo app. Ask: "Has this
app ever sorted your photos by person, on its own?" Let two students
answer. Do not explain how yet.
-->

---

<!-- SLOT 2: Where we are -->

# Where We Are

<div class="roadmap">
<div class="wk"><div class="n">Wk 1</div><div class="t">Introduction</div></div>
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
<div class="wk now"><div class="n">Wk 13</div><div class="t">AI · Quiz 2</div></div>
<div class="wk"><div class="n">Wk 14</div><div class="t">Emerging Technologies</div></div>
<div class="wk review"><div class="n">Wk 15</div><div class="t">Final Exam</div></div>
</div>

<!-- notes: Point at Week 13. Say: "Today we zoom into one fast-moving layer: AI." -->

---

<!-- SLOT 3: Recap + open wound -->

# Last Week, This Week

- **Last week delivered:** a survey of many real fields that use computers, from offices to entertainment.
- **Last week left broken:** one field changes faster than any other, and needs its own closer look.

---

<!-- SLOT 4: The pain (Act 1 / MOTIVATE), ZERO jargon -->

# The Folder That Knows Your Dog's Name

<div class="pain">

A student opens her phone's photo app.

The app has already sorted her photos into folders, one folder per person's face.

One folder is named after her little sister. But a photo of the family dog sits in that same folder.

She never told the app to do this. She never even asked it to sort her photos at all.

She has no idea how the app made this choice, right or wrong.

</div>

<!-- notes: Ask: "Has your phone ever guessed something about your photos, right or wrong?" Let two or three students answer. Do not explain yet. -->

---

<!-- SLOT 5: Cost of not knowing -->

# What This Actually Costs

- A photo app that guesses wrong can put private photos in the wrong place.
- A security camera that misreads a face can lock out the right person.
- Almost every job now touches some tool that makes guesses like this.

<div class="why">
<strong>In industry:</strong> "Explain how a recommendation or a face-matching tool decides" is now a common question, in many jobs, not only AI jobs.
</div>

---

# Where You Already Use AI

<div class="appgrid">
<div class="app"><div class="name">Photo app</div><div class="desc">Sorts photos by the faces it recognizes.</div></div>
<div class="app"><div class="name">Voice assistant</div><div class="desc">Turns your spoken words into text.</div></div>
<div class="app"><div class="name">Keyboard</div><div class="desc">Guesses the next word you will type.</div></div>
<div class="app"><div class="name">Streaming app</div><div class="desc">Recommends the next video or song.</div></div>
<div class="app"><div class="name">Spam filter</div><div class="desc">Guesses which emails you do not want.</div></div>
<div class="app"><div class="name">Maps app</div><div class="desc">Predicts traffic before you even drive.</div></div>
</div>

You already use AI every day, whether you noticed it or not.

---

<!-- SLOT 6: Driving question -->

<!-- _class: section -->

# This Week's Question

<div class="driving-q">"How does a computer 'learn' to recognize something, instead of being told an exact rule?"</div>

---

<!-- SLOT 7: Learning outcomes -->

# By the End of This Week, You Can

1. Explain what AI and machine learning mean, in plain words.
2. Describe how a computer learns from many examples.
3. Name AI tools you already use on your own phone.
4. List common mistakes AI still makes today.

---

<!-- SLOT 8: Origin -->

# Where This Idea Came From

<div class="thread">You just felt the pain. Where did the answer come from?</div>

<div class="cardlist">
<div class="card"><div class="h">1950</div><div class="d">Alan Turing asked a simple question: "Can a machine think?"</div></div>
<div class="card"><div class="h">1956</div><div class="d">A small workshop at Dartmouth first used the words "artificial intelligence."</div></div>
<div class="card"><div class="h">For decades after</div><div class="d">Computers were too slow, with too little data, to do much.</div></div>
<div class="card"><div class="h">2010s onward</div><div class="d">Far more data and much faster chips made today's AI possible.</div></div>
</div>

<div class="why">
AI is an old idea. It only recently became powerful enough to use every day.
</div>

---

<!-- SLOT 9: Core concept -->

# Artificial Intelligence: Definition

<div class="thread">One idea, one clear definition.</div>

> **Artificial intelligence (AI)** is software that learns patterns from examples, not fixed, hand-written rules.

- **Machine learning** is the main way AI learns today.
- Show it many examples, and it finds the pattern by itself.

---

# Rules vs. Learning: Two Ways to Build Software

<div class="thread">One idea, before we name more words.</div>

- **Old rule-based software:** a programmer writes every rule by hand.
  Example: "if it has pointy ears and whiskers, call it a cat."
- Real photos break simple rules like this all the time.
- **AI software:** show it 10,000 labeled cat photos, and let it learn.

<div class="why">
AI does not follow a rule a person wrote. It builds its own, from examples.
</div>

---

<!-- NEW: Key Words Today, 차시 1 -->

# Key Words Today

- **Artificial intelligence (AI)** — software that learns patterns from examples.
- **Machine learning** — the main way AI learns today, from many examples.
- **Data** — information a computer can store and learn from.
- **Pattern** — something that repeats, and so can be recognized.
- **Rule-based software** — old-style software, where a person writes every rule.

<!-- notes: Read each word aloud. Ask students to repeat it once. Ask: "Which word did you already know?" -->

---

<!-- NEW: Try-It preview, closes 차시 1 -->

# Coming Up: Worksheet Part A

<div class="thread">Next, you will practice using these words.</div>

- In **[Worksheet Part A](materials/week13/worksheet.html)**, you sort everyday phone features into "AI" or "not AI."
- Example: a clock app that just shows the time. Is that AI?
- You will work with a partner. A guess is fine for now.

<!-- notes: Tell students to sit next to a partner for the next part. No prep needed. -->

---

<!-- _class: section -->

# End of 차시 1
<div class="driving-q">Short break. 차시 2: how a computer actually learns from examples.</div>

---

<!-- NEW: Key Words Today, 차시 2 -->

# Key Words Today

- **Training** — showing a computer many labeled examples, so it can learn.
- **Label** — the correct answer attached to one example, like "cat" or "dog."
- **Model** — what an AI builds after training; its learned pattern.
- **Prediction** — the model's best guess about something new.
- **Accuracy** — how often a model's guess turns out correct.

<!-- notes: Read each word aloud. Say: "You will use all five words in the next slides." -->

---

<!-- Act 3 / BUILD -->

# How a Computer "Learns" From Examples

<div class="thread">Let's open up "training," one plain step at a time.</div>

- You show the computer thousands of labeled photos: "cat" or "dog."
- It looks for patterns common in "cat" photos, and different in "dog" photos.
- It builds a **model**: its own internal guess at what makes a cat a cat.

---

# Training: Practice Before the Real Test

<div class="thread">Training happens once. Then the model gets used many times.</div>

- Training uses many examples, often for a long time, on powerful computers.
- After training, the model is ready. It no longer needs the answer key.
- It can now guess on a brand-new photo, one it has never seen.

---

# Making a Prediction: New Photo, Best Guess

<div class="thread">Back to the folder that knew your dog's name.</div>

- You show the photo app a brand-new photo of a face.
- The trained model compares it to patterns it learned before.
- It picks the closest match: a folder, a name, its best guess.
- A wrong guess is not a lie. It is just a wrong best guess.

---

# AI Cheat Sheet

<div class="thread">Five words, one line each, before you practice.</div>

<div class="chip-row">
<span class="chip">AI: learns patterns from examples</span>
<span class="chip">Machine learning: the main way AI learns</span>
<span class="chip">Training: showing many labeled examples</span>
<span class="chip">Model: the pattern an AI learns</span>
<span class="chip">Prediction: the model's best guess</span>
</div>

---

# Practice Together: Trace One Guess

<div class="thread">Let's do one example, out loud, as a class.</div>

You open the photo app. It shows you a new photo.

1. **Training** already happened, long before today, on thousands of photos.
2. The trained **model** looks at your new photo's patterns.
3. It compares those patterns to what it learned before.
4. It picks its best guess, its **prediction**, and sorts the photo.

<!-- notes: Ask the class to name which word matches each numbered step. -->

---

<!-- NEW: Try-It hand-off, Worksheet Part A -->

# Try It: Worksheet Part A

<div class="thread">Now you practice. Work with a partner.</div>

- Open **[Worksheet Part A](materials/week13/worksheet.html)**.
- Sort each phone feature into "AI" or "not AI," and say why.
- You have about 15 minutes. Ask your partner before you ask me.

<!-- notes: Hand out Worksheet Part A. Walk around and help pairs. After 15 minutes, ask 2-3 pairs to share one answer. -->

---

<!-- _class: section -->

# End of 차시 2
<div class="driving-q">Short break. 차시 3: where AI gets it wrong, then today's Quiz 2.</div>

---

<!-- NEW: Key Words Today, 차시 3 -->

# Key Words Today

- **Bias** — when a model's training examples are not fair or complete.
- **Error** — a case when a model's best guess is wrong.
- **Deepfake** — a fake photo or video, made by AI, that looks real.
- **Privacy** — keeping your personal data safe from misuse.

<!-- notes: Read each word aloud. Say: "You will see these words in Worksheet Part B." -->

---

# Where AI Can Get It Wrong

<div class="thread">AI is not magic. It is only as good as its training.</div>

- If training photos show mostly one type of face, the model learns that type best.
- This is called **bias**: the model is less fair to people it saw less.
- A wrong guess is not random. It often traces back to unfair training data.

---

# Big Idea: Learning From Examples Has Limits

<div class="thread">Zoom out for a moment before the case study.</div>

- AI can only recognize patterns it has already seen in training.
- A totally new situation can confuse even a very good model.
- This is why AI still makes strange, sometimes funny, mistakes today.

<div class="why">
A model that has never seen snow can still misread a snowy photo.
</div>

---

<!-- SLOT N-2: Worked example -->

# Case Study: The Folder That Knew Your Dog's Name (1/2)

<div class="thread">Back to the frozen moment. Now you have the words.</div>

Here is what likely happened, back in slot 4.

- The photo app's **model** was trained on thousands of labeled family photos.
- It learned patterns: fur, shapes, and colors near the family's faces.
- Your dog's photo matched some of those patterns, by pure coincidence.

---

# Case Study: The Folder That Knew Your Dog's Name (2/2)

<div class="thread">The rest of the story, in today's words.</div>

- The model's **prediction** was still wrong: a dog is not your sister.
- This is a normal AI **error**, not a broken app.
- You can fix it: tell the app "no," and it can learn from your correction.

---

# Who Works With AI

<div class="thread">Real jobs, built on exactly today's ideas.</div>

<div class="appgrid">
<div class="app"><div class="name">AI / ML engineer</div><div class="desc">Builds and trains models.</div></div>
<div class="app"><div class="name">Data scientist</div><div class="desc">Studies data for useful patterns.</div></div>
<div class="app"><div class="name">Data labeler</div><div class="desc">Labels examples used for training.</div></div>
<div class="app"><div class="name">AI ethics reviewer</div><div class="desc">Checks models for bias and fairness.</div></div>
<div class="app"><div class="name">Product manager</div><div class="desc">Decides where AI should help users.</div></div>
<div class="app"><div class="name">Security analyst</div><div class="desc">Guards the data used for training.</div></div>
</div>

---

<!-- SLOT N-1: Common mistakes -->

# Common Mistakes

<div class="cardlist">
<div class="card"><div class="h">"AI always tells the truth"</div><div class="d">Wrong. It gives its best guess, not a fact.</div></div>
<div class="card"><div class="h">"AI understands like a person does"</div><div class="d">Wrong. It only matches learned patterns.</div></div>
<div class="card"><div class="h">"More data always means a fair model"</div><div class="d">Wrong. Unfair data still teaches unfair patterns.</div></div>
<div class="card"><div class="h">"AI mistakes are random"</div><div class="d">Wrong. They usually trace back to the training data.</div></div>
</div>

---

<!-- NEW: Try-It hand-off, Worksheet Part B -->

# Try It: Worksheet Part B

<div class="thread">More practice. New scenarios.</div>

- Open **[Worksheet Part B](materials/week13/worksheet.html)**.
- Decide whether each scenario shows bias, an error, or neither.
- You have about 15 minutes. Then we discuss answers together.

<!-- notes: Hand out Worksheet Part B. After 15 minutes, go through the answer key as a class. Ask for volunteers first. -->

---

<!-- SLOT N: Check yourself -->

# Check Yourself

1. What is the difference between AI and old rule-based software?
2. Why can a trained model still guess wrong on a new photo?
3. What is bias, in an AI model's training data?

---

# Answers

1. Old software follows fixed rules; AI learns patterns from many examples.
2. A guess is only a pattern match, not a certain fact; new cases can differ.
3. Bias is unfair or incomplete training data, so guesses stay unfair too.

---

<!-- NEW: Quiz 2 logistics, before the self-check quiz hand-off -->

# Quiz 2 Today

Quiz 2 is today, closed-book, about 15 minutes, covering Weeks 9-13.

---

<!-- NEW: Self-check quiz hand-off -->

# Self-Check Quiz

<div class="thread">One more check, on your own. Not the same as Quiz 2.</div>

- Take the **[Week 13 Quiz](materials/week13/quiz.html)** (5-8 short questions).
- This quiz is not graded. It just checks your understanding.
- About 10 minutes. Check your own answers at the end.

<!-- notes: Hand out the ungraded self-check quiz after Quiz 2 is collected. Give students 10 minutes. Then read the answer key aloud, or let students self-check. -->

---

# Quick Recap: Today in Four Words

<div class="thread">Before we close, one more look at the whole picture.</div>

<div class="chip-row">
<span class="chip">AI: learns from examples</span>
<span class="chip">Training: many labeled examples</span>
<span class="chip">Model: the learned pattern</span>
<span class="chip">Bias: unfair training data</span>
</div>

---

<!-- SLOT N+1: Limits (Act 4 / CLOSE), becomes Week 14 slot 4 -->

# What Today's AI Cannot Do Yet

<div class="limits">
AI is powerful today, but today's AI is only one stop on a much
longer road. It cannot truly understand the world like a person. It
only matches patterns it saw in training. New tools, and new limits,
are being built right now.
</div>

---

<!-- SLOT N+2: Bridge -->

# Next Week

Week 13 leaves **how AI itself might keep changing** unsolved. **Week 14,
Emerging Technologies**, addresses it: what other new technology comes next.

---

<!-- SLOT N+3: Summary -->

# Summary

- AI learns patterns from examples, instead of following only fixed rules.
- Training shows a model many labeled examples; then it makes predictions.
- AI already lives in your phone: photos, voice, keyboard, recommendations.
- Bias and errors trace back to training data, not "AI going rogue."
- **Reading:** Tanenbaum & Austin, chapter on modern computing trends.
- **Handout:** [materials/week13/handout.md](materials/week13/handout.html), glossary and the full training walkthrough.
- **Prepare:** Think of one AI tool that surprised you. Bring it to Week 14.

---

<!-- SLOT N+4: Thank You -->
<!-- _class: end -->

# Thank You
