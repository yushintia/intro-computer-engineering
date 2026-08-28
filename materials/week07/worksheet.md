# Week 7 Worksheet: What Is the OS Doing?

Introduction to Computer Engineering (400507-001) · Week 7
Work with a partner. There can be more than one correct answer.

For every scenario, choose one or more OS jobs:

**CPU time (scheduling) · Memory · Device (driver)**

If you are not sure, guess. Then explain your guess in one short
sentence.

---

## Part A (차시 2, in-class, ~15 minutes)

For each scenario, circle the OS job(s) most likely involved, and
write one short sentence why.

1. **Your laptop switches smoothly between your browser and your music app, even with both open.**
   OS job(s): CPU time / Memory / Device
   Why: ______________________________________________

2. **One app crashes, but every other open app keeps working fine.**
   OS job(s): CPU time / Memory / Device
   Why: ______________________________________________

3. **Your video call sounds clear, even while a big file downloads in the background.**
   OS job(s): CPU time / Memory / Device
   Why: ______________________________________________

4. **You plug in a new printer, and it needs new software before it will print.**
   OS job(s): CPU time / Memory / Device
   Why: ______________________________________________

5. **Opening fifteen browser tabs makes every other app feel slower.**
   OS job(s): CPU time / Memory / Device
   Why: ______________________________________________

6. **A photo-editing app is not allowed to read your web browser's saved passwords.**
   OS job(s): CPU time / Memory / Device
   Why: ______________________________________________

**Discuss with your partner:** Pick one scenario above. Name a second,
different OS job that could also explain it.

______________________________________________

---

## Part B (차시 3, in-class, ~15 minutes)

Same task, new scenarios. Work with a partner again (same or new).

1. **A game freezes the whole laptop, and every other app freezes too.**
   OS job(s): CPU time / Memory / Device
   Why: ______________________________________________

2. **Your laptop keeps running many small background apps, and you never notice them.**
   OS job(s): CPU time / Memory / Device
   Why: ______________________________________________

3. **A wireless mouse stops working until you reinstall its software.**
   OS job(s): CPU time / Memory / Device
   Why: ______________________________________________

4. **Two word processor windows are open. Closing one does not affect the words in the other.**
   OS job(s): CPU time / Memory / Device
   Why: ______________________________________________

5. **A video call gets choppy the moment a large file starts downloading.**
   OS job(s): CPU time / Memory / Device
   Why: ______________________________________________

6. **An app that has been idle for an hour is still using almost no CPU time.**
   OS job(s): CPU time / Memory / Device
   Why: ______________________________________________

**Discuss with your partner:** Which scenario in Part B was hardest to
decide? Why?

______________________________________________

---
---

## Professor Answer Key — do not hand out this section

Accept any reasonable, well-explained answer. Multiple OS jobs are
often defensible; the goal is reasoning, not a single "correct" pick.

### Part A

1. **CPU time.** The scheduler gives each app short time slices, so
   both feel active at once.
2. **Memory.** Each process has its own private memory space, so one
   crash does not spread to others.
3. **CPU time** (priority for the call's audio requests) or **Device**
   (the disk driver serving the download). Both are defensible.
4. **Device.** A new printer needs a device driver before the OS can
   talk to it.
5. **CPU time** (more processes competing for turns) or **Memory**
   (each tab uses its own memory space). Both are defensible.
6. **Memory.** Private memory spaces stop one app from reading
   another app's data, which protects saved passwords too.

### Part B

1. **CPU time** (most likely, a whole-machine problem, not one
   process's private memory) — accept **Device** if a shared driver
   is blamed instead.
2. **CPU time.** Idle or lightly-used apps get very short, infrequent
   time slices, so they barely affect anything.
3. **Device.** The mouse needs its driver working correctly to
   communicate with the OS.
4. **Memory.** Each window (process) keeps its own separate memory
   space; one closing does not touch the other's data.
5. **Device** (both compete for the same disk/network driver) or
   **CPU time** (the download's requests crowd out the call's).
   Both are defensible.
6. **CPU time.** The scheduler gives idle processes very little time,
   since they are not asking to do anything.
