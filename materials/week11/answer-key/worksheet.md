## Professor Answer Key — do not hand out this section

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

### Part C

**C1.** Sample:
```
SELECT Photo, Caption
FROM Photos
WHERE Place = 'Busan';
```

**C2.** Sample: "It shows the Name and Major of every student whose
Year is 2 (second-year students)."

**C3.**
1. Insert. A brand new row is added.
2. Update. One value already in a row is changed.
3. Delete. A row is removed completely.

**C4.**
1. **Data redundancy**: the same fact, stored in more than one place.
2. Sample: If Mia misses even one copy of "Busan," her records now
   quietly disagree with each other: some files say "Busan," others
   say "Busan City," for the same actual place.

**C5.**
1. Hierarchical.
2. Relational.
3. Network.

Discuss answer (sample): "Every table built today already assumes the
relational model: simple tables, linked by shared values."

### Part D

**D1.**
1. Availability. The data is not stolen or changed, but it is not
   reachable when needed.
2. Confidentiality. An unauthorized person reads data they should not
   see.
3. Integrity. The data is secretly changed, even though no one
   outside is involved.

**D2.**
1. Virus.
2. Worm.
3. Trojan.
4. Ransomware.

**D3.**
1. **Yes.** It creates false urgency and asks for a password, a
   classic phishing pattern.
2. **No.** It comes from an app Mia installed herself and only shows
   her own information; no unexpected request for credentials.

**D4.**
1. Authentication.
2. Firewall.
3. Two-step login (2FA).

**D5.** Sample: Collecting more personal data than a task actually
needs is a privacy problem on its own; even a perfectly secure
system can still misuse or over-collect data within the rules, which
is why responsible data use means only collecting what is needed.
