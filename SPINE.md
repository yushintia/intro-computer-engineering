# The Spine: Standard Structure for Every Lecture Week

Introduction to Computer Engineering (400507-001), 2026-2. This document
is the standard. Every week's deck (`slides/weekNN-*.md`) must follow it.
If a deck and this document disagree, fix the deck.

## Principle

**Motivation always precedes definition.** A student should never meet a
term before meeting the concrete problem that forced someone to invent it.
Every week opens with a broken scenario in plain language, not a formal
statement. This is a first-year, required course: assume no prior computer
science background at all, only everyday device experience.

**Weeks chain.** The "Limits" slide that closes week N is, almost verbatim,
the "Pain" slide that opens week N+1. The semester should read as one
argument, not fourteen independent talks.

## The 17 slots

Acts 0, 1, 2, 4 are **mandatory and fixed**: same slot numbers, same order,
every full-spine week. Act 3 (Build) expands or contracts to fit the topic.

### Act 0: LOCATE

| # | Slide | Rule |
|---|---|---|
| 1 | Title | Week #, topic, course code, instructor, date |
| 2 | Where we are | Shared roadmap graphic (`_shared/roadmap.md`), current week highlighted |
| 3 | Recap + open wound | One sentence on what last week delivered, one sentence on what it left broken |

### Act 1: MOTIVATE

| # | Slide | Rule |
|---|---|---|
| 4 | The pain | Concrete broken scenario in the running case study. **Zero jargon.** If a technical term appears here, the slide is wrong |
| 5 | Cost of not knowing | What breaks downstream (confusion, wasted time, bad decisions) *and* where this bites in industry (interviews, real product failures, job requirements) |
| 6 | Driving question | One sentence the week must answer. Repeat it verbatim on any section-divider slide inside Act 3 |
| 7 | Learning outcomes | 3-4 verbs, each traceable to a syllabus objective |

**Hard rule:** no formal definition before slot 8. If you need one earlier,
the pain slide (4) is too abstract, so fix it instead of breaking the rule.

### Act 2: GROUND

| # | Slide | Rule |
|---|---|---|
| 8 | Origin | Who, when, what forced it. Ideas are answers to historical pain, not arbitrary convention |
| 9 | Core concept | First formal definition of the week |

### Act 3: BUILD (flexible)

| # | Slide | Rule |
|---|---|---|
| 10..N-3 | Mechanics | Stepwise, as many slides as the topic needs |
| N-2 | Worked example | Same running case study, continued from prior weeks; see `slides/_shared/case-study.md` |
| N-1 | Common mistakes | Anti-patterns and why each is tempting |
| N | Check yourself | 2-3 questions; put the answers on the slide immediately after, not the same slide |

### Act 4: CLOSE

| # | Slide | Rule |
|---|---|---|
| N+1 | Limits | What this week's technique cannot do. **This text becomes next week's slot 4** |
| N+2 | Bridge | "Week N leaves X unsolved -> Week N+1 addresses it." Explicit, one sentence |
| N+3 | Summary | Takeaways + reading assignment + what to prepare |
| N+4 | Thank You | Template end slide |

## The semester chain

| Wk | Topic | Limit (leads to next pain) |
|---|---|---|
| 1 | Introduction | We know how this course runs, how we're graded, and what's expected of us, but we still don't know what's actually inside the device that just froze, or where any of this technology came from -> **W2** |
| 2 | Computer History | We know how computers evolved, but not yet how they represent anything as simply as on and off -> **W3** |
| 3 | Boolean Logic | Gates can decide true or false, but not yet follow a sequence of steps, a program -> **W4** |
| 4 | CPU & Instructions | The CPU executes instructions perfectly, but has nowhere permanent to keep anything once the power goes off -> **W5** |
| 5 | Memory & Storage | Data can now be kept and retrieved, but nothing yet turns it into something a person can actually use -> **W6** |
| 6 | Application Software · Quiz 1 | Apps exist, but nothing coordinates which app runs when, or shares the machine fairly -> **W7** |
| 7 | Operating Systems | One machine now runs well by itself, but is still completely alone, unable to talk to any other machine -> **W9** |
| 8 | Midterm | review only, no chain link |
| 9 | Computer & Internet | Machines can now talk to each other, but someone still has to write the instructions they exchange -> **W10** |
| 10 | Programming Language | We can now write those instructions, but a program with no data to manage is not very useful yet -> **W11** |
| 11 | Databases & Security | Data can be stored and protected, but we have only seen one narrow use of a computer at a time -> **W12** |
| 12 | Computer Applications | We have surveyed many uses, but one fast-moving one deserves its own week -> **W13** |
| 13 | AI · Quiz 2 | AI is powerful today, but today's AI is only one stop on a much longer road -> **W14** |
| 14 | Emerging Technologies | The semester surveyed the whole field; only the exam remains -> **W15** |
| 15 | Final Exam | review only, no chain link |

Weeks 8 and 15 use the **short review variant**: Act 0 (slots 1-3) + Act 3
slot "Check yourself" (expanded into full review questions) + Act 4 (slots
N+1..N+4, "Limits" replaced by "What to focus on next"). No Pain or Ground
acts: there is no new concept to motivate. Weeks 6 and 13 carry an embedded
quiz but keep the full spine: new content is still taught that day.

Week 1 uses the **orientation variant**: Act 0 (slots 1-2, no recap since
there is no prior week) + a short, non-technical tease of the running
pain scenario + the course-level driving question + the full course
contract (description, objectives, prerequisites, textbook, schedule,
grading, policies, contact) in place of Act 2/3 + Act 4 (slots N+1..N+4).
It carries **near-zero technical content** - the six-layer hardware/
software map and the "tracing one tap" walkthrough live in later weeks
instead. Week 1 is **handout-only**: `materials/week01/handout.md` is a
Course Handbook mirroring the contract (grading, policies, schedule,
textbook, contact). There is no Week 1 worksheet or quiz - the first
in-class worksheet/quiz activities start in Week 2.

## Enforcement

- Copy `slides/_template/week-XX.md` for every new week. It carries all 17
  slots as HTML comments; fill them in, don't renumber them.
- `slides/_shared/roadmap.md`: single source for the Act 0 roadmap graphic.
- `slides/_shared/case-study.md`: the running example as it stands after
  each week; update it when a week changes it materially.
- Course logistics (grading, textbook, policies) live in an appendix block
  in Week 1 only, outside the spine numbering. Administrative content must
  never sit between the roadmap and the pain slide.
