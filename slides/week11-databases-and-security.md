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
Yushintia Pramitarini, Ph.D · Dept. of Intelligent Computing · Thu [1-3] · Seongpa Hall 701
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

<div class="cardlist">
<div class="card"><div class="h">What a Database Is</div><div class="d">Explain what a database is, in plain words.</div></div>
<div class="card"><div class="h">Table Parts</div><div class="d">Name the parts of a simple database table.</div></div>
<div class="card"><div class="h">Data Protection</div><div class="d">Explain why stored data needs protection.</div></div>
<div class="card"><div class="h">Keeping Data Safe</div><div class="d">Name two basic ways to keep data safe.</div></div>
</div>

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

<!-- NEW: Key Words Today, session 1 -->

# Key Words Today

- **Database** — an organized collection of data a program can search.
- **Table** — data stored in rows and columns, like a list.
- **Record** — one row in a table, one single entry.
- **Field** — one column in a table, one piece of information.
- **Query** — a question you ask a database, to find data.

<!-- notes: Read each word aloud. Ask students to repeat it once. Ask: "Which word did you already know?" -->

---

<!-- NEW: Try-It preview, closes session 1 -->

# Coming Up: Worksheet Part A

<div class="thread">Next, you will practice using these words.</div>

- In **[Worksheet Part A](materials/week11/worksheet.html)**, you build a small table by hand.
- Example: photo name, date, and place. What columns do you need?
- You will work with a partner. A guess is fine for now.

<!-- notes: Tell students to sit next to a partner for the next part. No prep needed. -->

---

<!-- NEW: Key Words Today, session 2 -->

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

# Why Not Just Use Flat Files?

<div class="thread">A plain list has a deeper problem than just being messy.</div>

Imagine Mia keeps her photo list in three separate text files: one for Seoul trips, one for Busan trips, one for home photos. Each file repeats words like "Seoul" or "Busan," typed by hand, over and over.

- This repeated copying is called **data redundancy**: the same fact, stored in more than one place.
- If Mia later renames "Busan" to "Busan City," she must find and fix every single copy herself.
- Miss even one copy, and her records now quietly disagree with each other.

<div class="why">
A database stores each fact once, and lets many rows point to it — the redundancy problem, solved structurally.
</div>

---

# Before Relational: Data Models, Briefly

<div class="thread">Tables were not the first way anyone organized stored data.</div>

- **Hierarchical model** (1960s): data arranged like a family tree, each record with exactly one parent. Fast, but rigid.
- **Network model** (late 1960s): records could link to several other records, not just one parent. More flexible, but complex to search.
- **Relational model** (1970, Edgar Codd): data arranged in simple tables instead, linked by shared values. It became, and remains, the dominant model.

<div class="why">
Every table you will see for the rest of this week already assumes the relational model.
</div>

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

# Primary Key: Making Each Row Unique

<div class="thread">What stops two rows from being confused with each other?</div>

> A **primary key** is a field (or small set of fields) whose value is guaranteed to be different in every single row of a table.

- No two rows may ever share the same primary key value.
- A primary key lets a database find, update, or delete exactly one row, with no confusion.
- Mia's photo table can use **Photo** (like IMG001) as its primary key, since no two photos share that name.

---

# Worked Example: A Student Roster Table

<div class="thread">Same idea, a different everyday table.</div>

| StudentID | Name | Major | Year |
|---|---|---|---|
| S1001 | Jiho | Computer Engineering | 2 |
| S1002 | Yuna | Computer Engineering | 3 |
| S1003 | Minseo | Business | 1 |

- **StudentID** is the primary key: every student gets a different one, even if two students share the same name.
- **Name**, **Major**, and **Year** are ordinary fields, free to repeat across rows.
- Two students could both be named "Jiho" — the ID still tells them apart.

---

# Finding One Row: a Query

<div class="thread">Mia wants to see only her Seoul photos.</div>

- A **query** asks the database a question, using exact rules.
- Example: "Show me every row where Place is Seoul."
- The database checks each row, and returns only the matches.

---

# A Taste of SQL: Asking in Structured Words

<div class="thread">A query is not just an idea — it has its own exact wording.</div>

> **SQL** is a structured language used to ask a relational database a question, in a small set of exact, reusable words.

- **SELECT** names which fields you want to see.
- **FROM** names which table to look in.
- **WHERE** names the condition a row must match.

A SQL query reads almost like an English sentence, but every word follows exact rules — Week 10's "programming language" idea, now applied to asking questions instead of giving steps.

---

# A Taste of SQL: One Worked Query

<div class="thread">Turn "show me only my Seoul photos" into SQL.</div>

```
SELECT Photo, Caption
FROM Photos
WHERE Place = 'Seoul';
```

- **SELECT Photo, Caption** — show only these two fields.
- **FROM Photos** — look inside the Photos table.
- **WHERE Place = 'Seoul'** — only rows where Place matches "Seoul."

This is not a full SQL course — just enough to see that a query is really a small, precise sentence.

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

<!-- NEW: Key Words Today, session 3 -->

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

# Why Security Matters: Confidentiality, Integrity, Availability

<div class="thread">"Keep data safe" actually means three separate promises.</div>

- **Confidentiality** — only the right people can read the data.
- **Integrity** — the data stays accurate, and is not secretly changed.
- **Availability** — the data is there and reachable when it is actually needed.

<div class="why">
Losing any one of these three is still a security failure, even if the other two hold up fine.
</div>

---

# Case Study: Is Mia's Photo App Secure?

<div class="thread">Apply all three promises to one everyday app.</div>

<div class="cardlist">
<div class="card"><div class="h">Confidentiality</div><div class="d">Only Mia's own login can view her private photo captions.</div></div>
<div class="card"><div class="h">Integrity</div><div class="d">No one else can quietly rename her photos without her knowing.</div></div>
<div class="card"><div class="h">Availability</div><div class="d">Mia can still open her photos, even if one server briefly goes down.</div></div>
</div>

Losing any one of these three still counts as a security problem for Mia's app.

---

# Authentication: Proving Who You Are

<div class="thread">Passwords and two-step logins are both one bigger idea.</div>

> **Authentication** is the general process of proving that someone really is who they claim to be, before letting them in.

- A password is one common form of authentication: something only Mia should know.
- Two-step login adds a second form: something only Mia should have, like her phone.
- Authentication answers one question only: "are you really Mia?" It does not decide what Mia is allowed to do next.

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

# Firewalls: A Gate Between Networks

<div class="thread">Not every layer of protection lives inside the database itself.</div>

> A **firewall** is a system that watches traffic passing between two networks, and blocks anything that does not match its allowed rules.

- Think of it as a gate between Mia's home network and the wider internet.
- It can stop an unknown outside computer from ever reaching Mia's devices in the first place.
- A firewall protects the network path; encryption and passwords protect the data and the login, further inside.

---

# Security Technologies Cheat Sheet

<div class="thread">Four techniques, one line each, before we look at threats.</div>

<div class="chip-row">
<span class="chip">Authentication: proves who you are</span>
<span class="chip">Encryption: scrambles data for outsiders</span>
<span class="chip">Firewall: blocks unwanted network traffic</span>
<span class="chip">Backup: protects against loss, not just theft</span>
</div>

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

# Types of Malware: Virus, Worm, Trojan, Ransomware

<div class="thread">Not every threat tries to log in through the front door.</div>

<div class="cardlist">
<div class="card"><div class="h">Virus</div><div class="d">Attaches to a real file, and spreads when that file is shared or opened.</div></div>
<div class="card"><div class="h">Worm</div><div class="d">Spreads on its own across a network, with no file or person needed.</div></div>
<div class="card"><div class="h">Trojan</div><div class="d">Disguises itself as useful software, then does something harmful.</div></div>
<div class="card"><div class="h">Ransomware</div><div class="d">Locks or scrambles a victim's data, then demands payment to restore it.</div></div>
</div>

---

# Recent Hacking Trends: Phishing and Social Engineering

<div class="thread">Many modern attacks target a person, not a machine.</div>

- **Phishing** — a fake message pretends to be a trusted sender, tricking someone into sharing a password or clicking a bad link.
- **Social engineering** — a broader term for tricking a person into breaking their own security, through pressure, urgency, or false trust.
- These attacks skip the encryption and the firewall entirely, by aiming at human judgment instead.

<div class="why">
Awareness is the main defense here: pause before trusting an urgent, unexpected request.
</div>

---

# Information Ethics: Privacy and Responsible Data Use

<div class="thread">Protecting data is not only a technical question.</div>

- **Privacy** — a person's reasonable expectation that their personal data is not collected or shared without good reason.
- Responsible data use means only collecting what is actually needed, and only using it for the purpose it was collected for.
- Even perfectly secure data can still be used unethically, if it is misused within the rules.

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

<div class="cardlist">
<div class="card"><div class="h">"A database is just a file, like a folder"</div><div class="d">Wrong. It also lets you search and ask questions.</div></div>
<div class="card"><div class="h">"A short, simple password is fine"</div><div class="d">Wrong. Short passwords are the easiest to guess.</div></div>
<div class="card"><div class="h">"Only companies need to worry about data safety"</div><div class="d">Wrong. Anyone with an account is a target.</div></div>
<div class="card"><div class="h">"One backup copy is enough forever"</div><div class="d">Wrong. Backups can fail too; keep more than one.</div></div>
</div>

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
