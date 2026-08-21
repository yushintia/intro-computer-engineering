# Week 11 Handout: Databases & Security

Introduction to Computer Engineering (400507-001) · Week 11
This handout goes with the Week 11 slides. Keep it for the whole semester.

---

## 1. Glossary: Key Words

Simple, plain definitions. Read these before or after class.

| Word | Plain definition |
|---|---|
| **Database** | An organized collection of data. A program can find, add, or change it quickly. |
| **Table** | Data stored in rows and columns, like a list. One table, one topic. |
| **Record (row)** | One single entry in a table. Example: one photo, one contact. |
| **Field (column)** | One piece of information in a table. Example: a name, a date. |
| **Primary key** | A field that makes each row unique, so no two rows are confused. |
| **Query** | A question you ask a database, using exact rules, to find data. |
| **Search** | Finding data that matches what you asked for. |
| **Relational model** | Storing data as tables that can be linked together. Proposed in 1970. |
| **Password** | A secret word or phrase that proves who you are. |
| **Login** | Entering a username and password, to get access to an account. |
| **Personal data** | Information about one specific person. Example: a name, an address. |
| **Hacker** | Someone who tries to reach data without permission. |
| **Encryption** | Scrambling data, so only the right person can read it. |
| **Data breach** | An event where protected data is stolen or leaked. |
| **Backup** | An extra copy of data, kept safe in case the first copy is lost. |

---

## 2. Mia's Photo Database, Step by Step

This is the full version of the story from class. The slide version was
shortened. Read this at home if you want more detail.

Last week, Mia's program could rename all 200 of her trip photos, one
at a time, using sequence, loop, and decision. But once the program
stopped running, it forgot everything: the old names, the new names,
and which photos it had already renamed.

This week, Mia gives her program a real place to keep that
information: a **database**. She builds one **table** with four
**fields**: Photo, Date, Place, and Caption. Every photo becomes one
**record**, one row in that table.

Now Mia can ask her database questions, called **queries**. "Show me
every photo from Seoul" returns only the rows where Place is Seoul.
"Count my photos by place" groups the rows together, and gives her a
total for each group: 3 from Seoul, 2 from Busan, 1 from home.

But Mia's table also holds personal information: her name, her email,
and where each photo was taken. If anyone could open her account
without permission, they could see all of it, or even change it.

So Mia adds a **login**: a username and a password. The password
proves that whoever is signing in is really her. Her photo app also
uses **encryption**, so that even if someone steals a copy of her
data, it looks like scrambled nonsense without the right key. Finally,
the app limits access: only Mia, not random employees, can see her
private photos.

Storing data and protecting it are two different jobs, but Mia needs
both. A database with no protection is a public folder. Protection
with no database is just a locked door with nothing valuable behind
it.

---

## 3. Database Basics and Security Basics, Side by Side

| Database idea | What it does | Security idea | What it does |
|---|---|---|---|
| **Table** | Holds one kind of data, in rows and columns | **Login** | Checks who is trying to get in |
| **Record** | One single entry, like one photo | **Password** | Proves you are really you |
| **Field** | One piece of information, like a date | **Encryption** | Scrambles data so theft is useless |
| **Query** | Asks a question, returns matching rows | **Limited access** | Only shows people what they need |

These two lists work together. A database organizes data so it is
useful. Security keeps that same data safe from the wrong hands.

---

## 4. Optional Reading: More Detail

This section holds extra detail that was trimmed from the slides. It
is optional, but useful if you want to go deeper.

**Why the relational model mattered.** Before 1970, most programs
stored data in separate files, and each program had its own private
way of reading its own files. If two programs needed the same data,
sharing it safely was very hard, and mistakes broke data easily.
Edgar Codd, working at IBM, proposed storing all data as simple
tables, with clear rules for finding and linking rows. This became
the **relational model**, and it is still the basis for most databases
used today, including the ones behind banks, hospitals, and schools.

**Who works with databases and security.** Real engineering jobs map
onto the ideas in this week:

- **Database administrator** — designs and maintains an organization's databases.
- **Data analyst** — writes queries to answer business questions from stored data.
- **Security analyst** — protects data from hackers and misuse.
- **Backend developer** — connects an app's features to its database.

**Why this matters in industry.** Data breaches are common news
stories: a company loses control of personal data for millions of
users at once. Interviewers often ask candidates to design a simple
database table, or to explain why a certain password is weak. Both
skills from this week show up directly in real technical interviews.

---

## 5. Practice Problems (with Answers)

Try each problem yourself before checking the answer.

**Problem 1.** Name the three parts of a simple database table:
the table itself, plus two smaller parts inside it.

> **Answer:** The table itself, plus **records** (rows) and
> **fields** (columns).

**Problem 2.** A school wants to store each student's name, ID
number, and major. Design one table: list the field names you would
use as column headers.

> **Answer (sample):** Student ID, Name, Major. Any reasonable, clear
> field names are correct.

**Problem 3.** True or false: "A query can only find one single
row." Explain your answer in one sentence.

> **Answer:** False. A query can return many matching rows, or even
> zero rows, depending on the question asked.

**Problem 4.** A friend uses the password "password123" for every
account they own. Name two reasons this is risky.

> **Answer (sample):** It is easy for others to guess or find in a
> list of common passwords, and using it everywhere means one stolen
> password unlocks every account.

**Problem 5.** Explain, in your own words and in two sentences or
less, why encryption still helps even if a hacker steals a copy of
a database.

> **Answer (sample):** Encryption scrambles the data, so a stolen
> copy looks like nonsense without the right key to unscramble it.

**Problem 6.** Mia's photo app groups her photos by place, and
counts each group. Which database idea from this week does that:
a query, a password, or encryption?

> **Answer:** A query. Grouping and counting rows is a kind of
> question asked of the database.
