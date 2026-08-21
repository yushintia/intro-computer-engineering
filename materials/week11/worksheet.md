# Week 11 Worksheet: Tables, Queries, and Passwords

Introduction to Computer Engineering (400507-001) · Week 11
Work with a partner. There can be more than one correct answer.

---

## Part A (차시 2, in-class, ~15 minutes)

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

## Part B (차시 3, in-class, ~15 minutes)

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
---

## Instructor Answer Key — do not hand out this section

Accept any reasonable, well-explained answer. The goal is reasoning
about tables, queries, and password strength, not one fixed wording.

### Part A

1. **Fields (sample):** Name, Phone. **Row:** Mia, 010-1234-5678.
2. **Fields (sample):** Title, Artist. **Row:** "Home", IU.
3. **Fields (sample):** Photo, Date, Place. **Row:** IMG004, 2026-03-09, Busan.
4. **Fields (sample):** Class, Grade. **Row:** Computer Engineering, A.
5. **Sample:** "Show me every row where Place is Busan."
6. **Sample:** "Group all rows by Place, and count each group."
   A good **primary key** in any table is a field that never repeats,
   such as a phone number, a song ID, or a photo file name.

### Part B

1. **Weak.** Short, only numbers, and a very common password.
2. **Strong.** Long, mixes letters, numbers, and symbols; not an
   obvious dictionary word alone.
3. **Weak.** One of the most common passwords in the world.
4. **Strong.** Random-looking, long, mixes character types.
5. **Yes.** Grades are personal data; leaking them could harm a student.
6. **No.** Public holidays are already public information for everyone.
7. **Yes.** A home address is personal data; misuse could be unsafe.
8. **Query (sample):** "Show me every row where Date is 2026-03-02."
