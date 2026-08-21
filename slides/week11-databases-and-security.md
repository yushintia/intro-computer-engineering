---
marp: true
theme: shintia
paginate: true
footer: 'Department of Intelligent Computing'
---

<!-- SLOT 1: Title -->
<!-- _class: title -->

# Week 11: Databases & Security

<span class="subtitle">Introduction to Computer Engineering (400507-001)</span>

<div class="meta">
Yushintia Pramitarini, Ph.D · Dept. of Intelligent Computing · Thu [1-3] · 성파 701
</div>

<!--
notes: Ask everyone: "Where does an app keep your data after you close
it?" Wait for a few guesses. It is OK if no one is sure yet.
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
<div class="wk now"><div class="n">Wk 11</div><div class="t">Databases &amp; Security</div></div>
<div class="wk"><div class="n">Wk 12</div><div class="t">Computer Applications</div></div>
<div class="wk"><div class="n">Wk 13</div><div class="t">AI · Quiz 2</div></div>
<div class="wk"><div class="n">Wk 14</div><div class="t">Emerging Technologies</div></div>
<div class="wk review"><div class="n">Wk 15</div><div class="t">Final Exam</div></div>
</div>

<!-- notes: Point at Week 11. Say: "Today we learn where a program keeps its data, and how it protects it." -->

---

<!-- SLOT 3: Recap + open wound -->

# Last Week, This Week

- **Last week delivered:** we can now write exact steps: sequence, loop, and decision.
- **Last week left broken:** a program had no place to keep its data.

---

<!-- SLOT 4: The pain (Act 1 / MOTIVATE), ZERO jargon -->

# Where Does Mia's Program Keep Data?

<div class="pain">

Mia's program can now rename all 200 photos. It uses the steps she
learned last week: sequence, loop, and decision.

But once the program stops, everything it knew is gone. The old
names, the new names, and which photo is done all disappear.

Next time, Mia must start all over again.

She needs some place to keep this information safely, and find it
again later.

</div>

<!-- notes: Ask: "Where do you think your phone keeps your photos after you close the app?" Let two or three students guess. -->

---

<!-- SLOT 5: Cost of not knowing -->

# What This Actually Costs

- Without stored data, every program forgets everything when it closes.
- Apps like contacts, messages, and photos could not exist at all.
- Stored data that is not protected can be stolen or misused.

<div class="why">
<strong>In industry:</strong> most software jobs expect basic database
skill. Data breaches make daily news, and cost companies millions.
</div>

---

<!-- SLOT 6: Driving question -->

<!-- _class: section -->

# This Week's Question

<div class="driving-q">"What is a database, and how do we keep stored data safe?"</div>

---

<!-- SLOT 7: Learning outcomes -->

# By the End of This Week, You Can

1. Explain what a database is, in plain words.
2. Name the parts of a simple database table.
3. Explain why stored data needs protection.
4. Name two basic ways to keep data safe.

---

<!-- SLOT 8: Origin -->

# Where This Idea Came From

<div class="thread">You just felt the pain. Where did the answer come from?</div>

- **1960s:** companies kept records in separate files. Hard to search, easy to break.
- **1970:** Edgar Codd proposed storing data in tables. This became the relational model.
- **Since then:** almost every app saves its data in a database like this.

<div class="why">
Codd's idea let a program find and change data safely, without
breaking any other data.
</div>

---

<!-- SLOT 9: Core concept -->

# Database: Definition

<div class="thread">One idea, one clear definition.</div>

> A **database** is an organized collection of data, stored so a
> program can find, add, or change it quickly.

- A **table** stores data in rows and columns, like a list.
- A **record** is one row: one single entry.
- A **field** is one column: one piece of information.

---

<!-- NEW: Key Words Today, 차시 1 -->

# Key Words Today

- **Database** — an organized collection of data a program can search.
- **Table** — data stored in rows and columns, like a list.
- **Record** — one row in a table, one single entry.
- **Field** — one column in a table, one piece of information.
- **Query** — a question you ask a database, to find data.

<!-- notes: Read each word aloud. Ask students to repeat it once. Ask: "Which word did you already know?" -->

---

<!-- NEW: Try-It preview, closes 차시 1 -->

# Coming Up: Worksheet Part A

<div class="thread">Next, you will practice using these words.</div>

- In **[Worksheet Part A](materials/week11/worksheet.html)**, you build a small table by hand.
- Example: photo name, date, and place. What columns do you need?
- You will work with a partner. A guess is fine for now.

<!-- notes: Tell students to sit next to a partner for the next part. No prep needed. -->

---

<!-- _class: section -->

# End of 차시 1
<div class="driving-q">Short break. 차시 2: how a database actually stores and finds data.</div>

---

<!-- NEW: Key Words Today, 차시 2 -->

# Key Words Today

- **Row** — another word for a record, one entry in a table.
- **Column** — another word for a field, one piece of information.
- **Primary key** — a field that makes each row unique.
- **Search** — finding data that matches what you asked for.

<!-- notes: Read each word aloud. Say: "You will use these words with real tables today." -->

---

<!-- Act 3 / BUILD -->

# Databases vs. a Plain List

<div class="thread">Mia could just type a list in a notes app. Why not?</div>

- A plain list has no exact rules. Anyone can type it any way.
- Finding "only my Seoul photos" means reading the whole list by eye.
- A database enforces structure, so a program can search it instantly.

---

# A Table Looks Like a List

<div class="thread">One table, one topic. Rows and columns.</div>

| Photo | Date | Place | Caption |
|---|---|---|---|
| IMG001 | 2026-03-02 | Seoul | Class trip |
| IMG002 | 2026-03-02 | Seoul | Group photo |
| IMG003 | 2026-03-09 | Busan | Beach walk |
| IMG004 | 2026-03-09 | Busan | Sunset photo |

Each row is one record. Each column is one field.

---

# What Kind of Data Fits a Field

<div class="thread">Each field expects one particular kind of value.</div>

- **Text** — words, like a caption or a name.
- **Number** — a count or a price, ready for math.
- **Date** — one specific day, useful for sorting and filtering.

---

# Finding One Row: a Query

<div class="thread">Mia wants to see only her Seoul photos.</div>

- A **query** asks the database a question, using exact rules.
- Example: "Show me every row where Place is Seoul."
- The database checks each row, and returns only the matches.

---

# Adding and Changing Data

<div class="thread">A table is not frozen. It changes as Mia works.</div>

- **Insert** adds a brand new row, like one new photo.
- **Update** changes one value already in a row, like a caption.
- **Delete** removes a row completely, like a photo she no longer wants.

---

# Linking Two Tables

<div class="thread">One table is rarely the whole picture.</div>

- Mia adds a second table, Place, with a short description of each city.
- Her photo table links to it, using the matching place name.
- This way, she does not repeat the same description in every row.

---

# Where Data Actually Lives

<div class="thread">A database is not always on your own device.</div>

- **Local** — data stored only on your own phone or laptop.
- **Cloud** — data stored on a company's remote computer, reached online.
- Cloud storage needs a strong login, since many people share the machine.

---

# Counting By Group

<div class="thread">Sometimes Mia wants a summary, not just one row.</div>

<div class="groupviz">
<div class="bucket"><div class="label">Seoul</div><div class="rows">IMG001<br>IMG002<br>IMG005</div><div class="agg">Count: 3</div></div>
<div class="bucket"><div class="label">Busan</div><div class="rows">IMG003<br>IMG004</div><div class="agg">Count: 2</div></div>
<div class="bucket"><div class="label">Home</div><div class="rows">IMG006</div><div class="agg">Count: 1</div></div>
</div>

A database can group matching rows, and count each group.

---

# Every App Has One (or More)

<div class="thread">Databases hide behind almost every app you use.</div>

<div class="appgrid">
<div class="app"><div class="name">Contacts</div><div class="desc">One row per contact: name, phone, email.</div></div>
<div class="app"><div class="name">Messaging app</div><div class="desc">One row per message: sender, time, text.</div></div>
<div class="app"><div class="name">School portal</div><div class="desc">Stores your grades, classes, and attendance.</div></div>
<div class="app"><div class="name">Music app</div><div class="desc">Stores every song, artist, and your playlists.</div></div>
<div class="app"><div class="name">Online shop</div><div class="desc">Stores every product, price, and order.</div></div>
<div class="app"><div class="name">Photo app</div><div class="desc">Stores Mia's 200 photos, dates, and places.</div></div>
</div>

Every app you tap is reading or writing rows, somewhere.

---

<!-- NEW: Try-It hand-off, Worksheet Part A -->

# Try It: Worksheet Part A

<div class="thread">Now you practice. Work with a partner.</div>

- Open **[Worksheet Part A](materials/week11/worksheet.html)**.
- Build a small table for Mia's photo app, by hand.
- You have about 15 minutes. Ask your partner before you ask me.

<!-- notes: Hand out Worksheet Part A. Walk around and help pairs. After 15 minutes, ask 2-3 pairs to share one answer. -->

---

<!-- _class: section -->

# End of 차시 2
<div class="driving-q">Short break. 차시 3: keeping stored data safe.</div>

---

<!-- NEW: Key Words Today, 차시 3 -->

# Key Words Today

- **Password** — a secret word or phrase that proves who you are.
- **Login** — entering a username and password to get access.
- **Personal data** — information about one specific person.
- **Hacker** — someone who tries to reach data without permission.
- **Encryption** — scrambling data, so only the right person can read it.

<!-- notes: Read each word aloud. Say: "These words tie everything together today." -->

---

# Why Stored Data Needs Protection

<div class="thread">A database only helps if the right people can use it.</div>

- Mia's photo app stores her name, email, and location history.
- Anyone who reaches this data could misuse it, or sell it.
- A database must let Mia in, and keep everyone else out.

---

# The Password: A Simple Lock

<div class="thread">The most common protection is still the simplest.</div>

- A **login** checks a username and a password together.
- The password proves "this really is Mia," not someone else.
- A weak password, like "12345", is easy for others to guess.

---

# What Makes a Password Strong

<div class="thread">Not every password protects an account equally well.</div>

- **Long** — more characters are much harder for others to guess.
- **Mixed** — letters, numbers, and symbols together, not just one type.
- **Unique** — a different password for every single account you own.

---

# Two-Step Login: A Second Lock

<div class="thread">What if a hacker guesses the password anyway?</div>

- **Two-step login** asks for a second proof, after the password.
- Often, it sends a short code to your phone or email.
- Even a stolen password is useless without that second code.

---

# Beyond the Password

<div class="thread">Week 4 met the CPU. Real systems stack several defenses.</div>

<div class="pipeline">
<div class="stage"><div class="h">Password</div><div class="s">checks who is logging in</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Encryption</div><div class="s">scrambles data, so a stolen copy is useless</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Limited access</div><div class="s">only lets people see what they truly need</div></div>
</div>

No single lock is perfect. Together, these layers protect the data well.

---

# Backups: Protecting Against Loss

<div class="thread">Security is not only about keeping people out.</div>

- A **backup** is an extra copy of data, stored somewhere safe.
- If a laptop breaks, or a hacker deletes data, a backup saves it.
- Good security protects data from theft, and from simple accidents too.

---

# When Protection Fails: Data Breaches

<div class="thread">Sometimes, despite protection, stored data still gets out.</div>

- A **data breach** happens when protected data is stolen or leaked.
- One breach can expose millions of passwords and personal records at once.
- This is why companies use many layers of protection, not just one.

---

# One Weak Link, Many Accounts

<div class="barchart">
<div class="bar-row">
  <div class="bar-label">One weak password</div>
  <div class="bar-track"><div class="bar-fill short" style="width: 10%"></div></div>
  <div class="bar-value">protects one account</div>
</div>
<div class="bar-row">
  <div class="bar-label">One data breach</div>
  <div class="bar-track"><div class="bar-fill long" style="width: 100%"></div></div>
  <div class="bar-value">can expose millions of accounts</div>
</div>
</div>

The gap is huge. Good habits at your scale still matter a lot.

<!-- notes: Point at the two bars. Say: "See the size difference? That is why companies invest so much in protection." -->

---

# Who Works With Data

<div class="thread">Databases and security are full-time jobs, not just this week's topic.</div>

<div class="appgrid">
<div class="app"><div class="name">Database administrator</div><div class="desc">Builds and maintains an organization's databases.</div></div>
<div class="app"><div class="name">Data analyst</div><div class="desc">Writes queries to answer real business questions.</div></div>
<div class="app"><div class="name">Security analyst</div><div class="desc">Finds weaknesses, and stops hackers from getting in.</div></div>
<div class="app"><div class="name">Backend developer</div><div class="desc">Connects an app's features to its database.</div></div>
</div>

Each job protects, or makes sense of, data other people rely on.

---

<!-- SLOT N-2: Worked example -->

# Case Study: Mia's Protected Photo Table

<div class="thread">Back to Mia's laptop. Now she has data, and protection.</div>

<div class="chip-row">
<span class="chip">Table: photo, date, place, caption</span>
<span class="chip">Query: show only Seoul photos</span>
<span class="chip">Password: locks her account</span>
</div>

Together, these ideas let Mia store, find, and protect her 200 photos.

---

<!-- SLOT N-1: Common mistakes -->

# Common Mistakes

- **"A database is just a file, like a folder":** Wrong. It also lets you search and ask questions.
- **"A short, simple password is fine":** Wrong. Short passwords are the easiest to guess.
- **"Only companies need to worry about data safety":** Wrong. Anyone with an account is a target.
- **"One backup copy is enough forever":** Wrong. Backups can fail too; keep more than one.

---

# Checking a Password, Step by Step

<div class="thread">Use this quick check on any password you see.</div>

<div class="pipeline">
<div class="stage"><div class="h">Length</div><div class="s">at least 10 characters long?</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Mix</div><div class="s">letters, numbers, and symbols together?</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Unique</div><div class="s">different from your other passwords?</div></div>
</div>

Three checks. If any answer is "no," treat the password as weak.

---

<!-- NEW: Try-It hand-off, Worksheet Part B -->

# Try It: Worksheet Part B

<div class="thread">More practice. New scenarios.</div>

- Open **[Worksheet Part B](materials/week11/worksheet.html)**.
- Write one safe query, and judge one password's strength.
- You have about 15 minutes. Then we discuss answers together.

<!-- notes: Hand out Worksheet Part B. After 15 minutes, go through the answer key as a class. Ask for volunteers first. -->

---

<!-- SLOT N: Check yourself -->

# Check Yourself

1. What is a database, in your own words?
2. Name two parts of a simple table.
3. Which finds only rows you want: a query, or a password?

---

# Answers

1. Sample: an organized collection of data a program can search.
2. Any two: table, row (record), column (field).
3. A query — it asks a question, and returns only matching rows.

---

<!-- NEW: Self-check quiz hand-off -->

# Self-Check Quiz

<div class="thread">One more check, on your own.</div>

- Take the **[Week 11 Quiz](materials/week11/quiz.html)** (5-8 short questions).
- This quiz is not graded. It just checks your understanding.
- About 10 minutes. Check your own answers at the end.

<!-- notes: Hand out the quiz. Give students 10 minutes. Then read the answer key aloud, or let students self-check. -->

---

<!-- SLOT N+1: Limits (Act 4 / CLOSE), becomes Week 12 slot 4 -->

# What Databases And Passwords Cannot Do Yet

<div class="limits">
Data can now be stored, and protected with a password. But we have
only seen one narrow use of a computer at a time. What else can a
computer actually do for us? We do not know yet.
</div>

---

<!-- SLOT N+2: Bridge -->

# Next Week

Week 11 leaves **the wider uses of a computer** unsolved. **Week 12,
Computer Applications**, addresses it: a broad survey of what
computers actually do.

---

<!-- SLOT N+3: Summary -->

# Summary

- A database is an organized collection of data: tables, rows, and columns.
- A query asks a database a question, and returns matching rows.
- Passwords, encryption, and limited access help keep stored data safe.
- **Reading:** Tanenbaum & Austin, the chapter on databases and data security.
- **Handout:** [materials/week11/handout.md](materials/week11/handout.html), glossary and the full worked example.
- **Prepare:** Think of one app that asks for your password. Bring it to Week 12.

---

<!-- SLOT N+4: Thank You -->
<!-- _class: end -->

# Thank You
