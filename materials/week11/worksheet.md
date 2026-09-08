# Week 11 Worksheet: Tables, Queries, and Passwords

Introduction to Computer Engineering (400507-001) · Week 11
Work with a partner. There can be more than one correct answer.

---

## Part A (Session 2, in-class, ~15 minutes)

Design a small database table for each app below. Write 3-4 field
names (column headers), and one sample row of data.

1. **A contacts app.** It stores each person's name and phone number.
   Fields: ______________________________________________
   Sample row: ______________________________________________

2. **A music app.** It stores each song's title and artist.
   Fields: ______________________________________________
   Sample row: ______________________________________________

3. **Mia's photo app.** It stores each photo's date and place.
   Fields: ______________________________________________
   Sample row: ______________________________________________

4. **A school portal.** It stores each class's name and grade.
   Fields: ______________________________________________
   Sample row: ______________________________________________

Now use the table you built in question 3 (Mia's photo app).

5. **Write a query in plain words** that finds only photos taken in
   Busan.
   Query: ______________________________________________

6. **Write a query in plain words** that counts how many photos were
   taken in each place.
   Query: ______________________________________________

**Discuss with your partner:** Pick one table above. Name one field
that could work as a **primary key**, making each row unique.

______________________________________________

---

## Part B (Session 3, in-class, ~15 minutes)

**Judge each password.** Circle Weak or Strong, and write one reason.

1. **"123456"**
   Weak / Strong — Why: ______________________________________________

2. **"MyDog'sName!s_Coco88"**
   Weak / Strong — Why: ______________________________________________

3. **"password"**
   Weak / Strong — Why: ______________________________________________

4. **"Su3#kL9!qzT2"**
   Weak / Strong — Why: ______________________________________________

**Decide: does this data need protection?** Circle Yes or No, and
write one reason.

5. **A student's exam grades, stored in the school portal.**
   Yes / No — Why: ______________________________________________

6. **The list of public holidays this year.**
   Yes / No — Why: ______________________________________________

7. **A user's home address, stored in a delivery app.**
   Yes / No — Why: ______________________________________________

8. **Write one safe query.** Mia's photo table has fields Photo, Date,
   Place, and Caption. Write, in plain words, a query that finds
   every photo taken on 2026-03-02.
   Query: ______________________________________________

**Discuss with your partner:** Which password in this worksheet was
hardest to judge? Why?

______________________________________________

---

## Part C: Actual SQL, and Where Tables Came From (~15 minutes)

Use Mia's photo table from class: fields **Photo, Date, Place,
Caption**.

### C1. Write a real SQL query

Write one SQL query, using **SELECT**, **FROM**, and **WHERE**, that
finds the Photo and Caption of every photo taken in **Busan**. Follow
the same style as the class example:

```
SELECT Photo, Caption
FROM Photos
WHERE Place = 'Seoul';
```

Your query:
```
______________________________________________
______________________________________________
______________________________________________
```

### C2. Read a query

A classmate wrote this query on a **Students** table (fields:
StudentID, Name, Major, Year):

```
SELECT Name, Major
FROM Students
WHERE Year = 2;
```

In one sentence, explain in plain words what this query returns.

______________________________________________

### C3. Insert, update, or delete?

For each action, write **Insert**, **Update**, or **Delete**.

1. Mia takes a new photo and adds it to her table as a brand new row.
   ______________________________________________
2. Mia fixes a typo in one photo's caption.
   ______________________________________________
3. Mia removes a blurry photo from her table completely.
   ______________________________________________

### C4. Why not just use flat files?

Mia keeps three separate text files: one for Seoul trips, one for
Busan trips, one for home photos. Each file repeats the word "Busan"
by hand, typed over and over.

1. What is the name for this problem: the same fact, stored in more
   than one place? ______________________________________________
2. If Mia renames "Busan" to "Busan City," what could go wrong if she
   only fixes some of the copies? ______________________________________________

### C5. Match the data model

Write **Hierarchical**, **Network**, or **Relational** next to its
description.

1. Data arranged like a family tree, each record with exactly one
   parent. ______________________________________________
2. Data arranged in simple tables, linked by shared values.
   ______________________________________________
3. Records could link to several other records, not just one parent.
   ______________________________________________

**Discuss with your partner:** Which data model does every table
you've built today already assume?

______________________________________________

---

## Part D: Keeping Data Safe (~15 minutes)

### D1. The CIA triad

Mia's school portal stores grades. For each event, write
**Confidentiality**, **Integrity**, or **Availability**: which
promise is broken?

1. A hacker cannot read any student's grades, but floods the school
   server so no one, not even teachers, can log in for a day.
   ______________________________________________
2. Someone without permission views another student's private grades.
   ______________________________________________
3. A classmate secretly changes their own failing grade to an A in
   the database.
   ______________________________________________

### D2. Match the malware

Write **Virus**, **Worm**, **Trojan**, or **Ransomware** next to its
description.

1. Attaches to a real file, and spreads when that file is shared or
   opened. ______________________________________________
2. Spreads on its own across a network, with no file or person
   needed. ______________________________________________
3. Disguises itself as useful software, then does something harmful.
   ______________________________________________
4. Locks or scrambles a victim's data, then demands payment to
   restore it. ______________________________________________

### D3. Is this phishing?

For each message, circle **Yes** or **No**, and write one reason.

1. "URGENT: Your account will be deleted in 1 hour. Click here and
   enter your password now to keep it."
   Yes / No. Why: ______________________________________________
2. A calendar reminder from an app you installed yourself, showing
   your own class schedule.
   Yes / No. Why: ______________________________________________

### D4. Quick match

Write the correct word for each blank: **Authentication · Two-step
login (2FA) · Firewall**

1. The general process of proving that someone really is who they
   claim to be, before letting them in, is called ______________.
2. A gate between two networks that blocks traffic not matching its
   allowed rules is called a ______________.
3. Asking for a password, then a second code sent to your phone, is
   called ______________.

### D5. Privacy check

Mia's photo app wants to collect her exact home address, even though
it only needs her city to show local weather. In one sentence,
explain why this is a privacy concern, even if the app's security
(passwords, encryption) is otherwise strong.

______________________________________________
