# Week 1 Worksheet: Which Layer Is It?

Introduction to Computer Engineering (400507-001) · Week 1
Work with a partner. There can be more than one correct answer.

For every scenario, choose one or more layers:

**Hardware · Software · Operating System (OS) · Network**

If you are not sure, guess. Then explain your guess in one short
sentence.

---

## Part A (차시 2, in-class, ~15 minutes)

For each scenario, circle the layer(s) most likely responsible, and
write one short sentence why.

1. **Your phone gets very hot after 20 minutes of gaming.**
   Layer(s): Hardware / Software / OS / Network
   Why: ______________________________________________

2. **A single app closes by itself, but every other app still works.**
   Layer(s): Hardware / Software / OS / Network
   Why: ______________________________________________

3. **Your video call freezes, but your music app keeps playing fine.**
   Layer(s): Hardware / Software / OS / Network
   Why: ______________________________________________

4. **Your laptop is very slow when many apps are open at once.**
   Layer(s): Hardware / Software / OS / Network
   Why: ______________________________________________

5. **A message says "no internet connection" on every app.**
   Layer(s): Hardware / Software / OS / Network
   Why: ______________________________________________

6. **Your phone's battery drains twice as fast as last month.**
   Layer(s): Hardware / Software / OS / Network
   Why: ______________________________________________

**Discuss with your partner:** Pick one scenario above. Name a second,
different layer that could also explain it.

______________________________________________

---

## Part B (차시 3, in-class, ~15 minutes)

Same task, new scenarios. Work with a partner again (same or new).

1. **An app will not open at all, no matter how many times you tap it.**
   Layer(s): Hardware / Software / OS / Network
   Why: ______________________________________________

2. **Your wifi icon shows full signal, but no page will load.**
   Layer(s): Hardware / Software / OS / Network
   Why: ______________________________________________

3. **Your laptop screen stays black, but you can hear the fan running.**
   Layer(s): Hardware / Software / OS / Network
   Why: ______________________________________________

4. **After a software update, your phone restarts by itself every hour.**
   Layer(s): Hardware / Software / OS / Network
   Why: ______________________________________________

5. **Two apps both try to use the camera, and both freeze.**
   Layer(s): Hardware / Software / OS / Network
   Why: ______________________________________________

6. **A downloaded file is missing after you restart your computer.**
   Layer(s): Hardware / Software / OS / Network
   Why: ______________________________________________

**Discuss with your partner:** Which scenario in Part B was hardest to
decide? Why?

______________________________________________

---
---

## Instructor Answer Key — do not hand out this section

Accept any reasonable, well-explained answer. Multiple layers are
often defensible; the goal is reasoning, not a single "correct" pick.

### Part A

1. **Hardware.** The chip is producing heat under heavy use. (Software
   could contribute if a buggy app overuses the CPU — accept that too.)
2. **Software.** One app crashing alone, while others keep running,
   points to that app's own code, not the device as a whole.
3. **Network** (most likely) or **Software** (the call app itself). A
   working music app rules out most hardware causes.
4. **OS** (fails to share resources fairly) or **Hardware** (not
   enough memory/CPU for the load). Both are defensible.
5. **Network.** Every app failing at once, with the same message,
   points to the connection, not any single app.
6. **Software** (a misbehaving app draining power) or **Hardware**
   (aging battery). Both are defensible; ask students to justify.

### Part B

1. **Software** (the app itself is broken) or **OS** (not enough
   memory to launch it). Both are defensible.
2. **Network.** A full signal icon with no working connection is a
   classic network-layer symptom (e.g., no real internet access).
3. **Hardware.** The fan running but no screen output suggests a
   hardware/display fault, not software.
4. **Software.** A recent update is the direct trigger; this is a
   software-layer regression.
5. **OS.** Sharing one physical resource (the camera) between two apps
   fairly is exactly the OS's job, and it failed here.
6. **Storage** (part of hardware) or **Software** (a save/write bug).
   Both are defensible; ask students which they'd check first.
