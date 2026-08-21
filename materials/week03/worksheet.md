# Week 3 Worksheet: AND, OR, or NOT?

Introduction to Computer Engineering (400507-001) · Week 3
Work with a partner. There can be more than one correct answer.

For every scenario, decide which gate (or gates) it needs:

**AND · OR · NOT**

If you are not sure, guess. Then explain your guess in one short
sentence.

---

## Part A (차시 2, in-class, ~15 minutes)

For each scenario, circle the gate(s) that best model it, and fill in
the small truth table.

1. **Turn on the fan = "Room is hot" AND "Fan switch is set to auto."**
   Gate(s): AND / OR / NOT
   | Room hot? | Switch on auto? | Fan on? |
   |---|---|---|
   | No | No | _____ |
   | No | Yes | _____ |
   | Yes | No | _____ |
   | Yes | Yes | _____ |

2. **Door alarm sounds = "Door open" OR "Window open."**
   Gate(s): AND / OR / NOT
   | Door open? | Window open? | Alarm sounds? |
   |---|---|---|
   | No | No | _____ |
   | No | Yes | _____ |
   | Yes | No | _____ |
   | Yes | Yes | _____ |

3. **Screen stays on = NOT "No one is looking at it."**
   Gate(s): AND / OR / NOT
   | No one looking? | Screen stays on? |
   |---|---|
   | Yes | _____ |
   | No | _____ |

4. **Free seat light turns on = "Seat empty" AND "Seatbelt sign is off."**
   Gate(s): AND / OR / NOT
   Why: ______________________________________________

5. **Game controller vibrates = "Hit landed" OR "Low health warning."**
   Gate(s): AND / OR / NOT
   Why: ______________________________________________

**Discuss with your partner:** Pick one scenario above. Name a
different everyday situation that uses the same gate.

______________________________________________

---

## Part B (차시 3, in-class, ~15 minutes)

Same task, harder scenarios. Some need more than one gate. Work with
a partner again (same or new).

1. **Elevator door opens = "Floor reached" AND NOT "Doors already open."**
   Gate(s): AND / OR / NOT
   Why: ______________________________________________

2. **Washing machine starts = "Door closed" AND ("Start button pressed"
   OR "Timer reached zero").**
   Gate(s): AND / OR / NOT
   Why: ______________________________________________

3. **Traffic light turns green = NOT "Pedestrian button pressed"
   AND "Timer done."**
   Gate(s): AND / OR / NOT
   Why: ______________________________________________

4. **Low-fuel warning shows = "Fuel below 10%" AND NOT "Just refueled."**
   Fuel is at 8%, and the car was refueled two minutes ago. Does the
   warning show? Explain in one sentence.
   ______________________________________________

5. **Build your own:** Write one true/false decision from your own
   life (like the umbrella example). Use at least one AND, OR, or NOT.
   ______________________________________________
   ______________________________________________

**Discuss with your partner:** Which scenario in Part B needed more
than one gate? Draw a small chain, like in class, if you have time.

______________________________________________

---
---

## Instructor Answer Key — do not hand out this section

Accept any reasonable, well-explained answer. The goal is correct gate
reasoning, not a single memorized phrasing.

### Part A

1. **AND.** Row order: No/No → No, No/Yes → No, Yes/No → No,
   Yes/Yes → **Yes**. Both conditions must hold.
2. **OR.** Row order: No/No → No, No/Yes → **Yes**, Yes/No → **Yes**,
   Yes/Yes → **Yes**. Either condition is enough.
3. **NOT.** Row order: Yes (someone looking) → No; No (no one
   looking) → **Yes**. The gate flips the input.
4. **AND.** Both "seat empty" and "seatbelt sign off" must be true at
   the same time for the light to turn on.
5. **OR.** Either a landed hit or a low-health warning alone is
   enough to trigger vibration.

### Part B

1. **AND with a NOT inside it.** The elevator needs the floor reached
   AND the doors not already open (NOT flips "doors already open").
2. **AND with an OR inside it.** The door must be closed (AND), and
   either the button was pressed or the timer reached zero (OR).
3. **AND with a NOT inside it.** The light needs no pedestrian request
   (NOT) AND the timer being done.
4. **Yes, the warning shows only if the AND gate's inputs are both
   true.** Fuel below 10% is true (8%). But NOT "just refueled" is
   false, since the car was just refueled. One false input means the
   AND gate outputs false. **So the warning does NOT show.** This is
   a common trap: fuel is low, but the recent refuel input matters.
5. **Open-ended.** Accept any answer that correctly names at least one
   gate and matches its own stated logic. Ask students to explain
   their gate choice out loud if time allows.
