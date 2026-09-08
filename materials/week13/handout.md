# Week 13 Handout: AI

Introduction to Computer Engineering (400507-001) · Week 13
This handout goes with the Week 13 slides. Keep it for the whole semester.

---

## 1. Glossary: Key Words

Simple, plain definitions. Read these before or after class.

| Word | Plain definition |
|---|---|
| **Artificial intelligence (AI)** | Software that learns patterns from examples, instead of following only fixed rules. |
| **Machine learning** | The main way AI learns today. Show it many examples, and it finds the pattern itself. |
| **Data** | Information a computer can store and learn from. Example: thousands of labeled photos. |
| **Pattern** | Something that repeats often enough that it can be recognized. |
| **Rule-based software** | Old-style software. A person writes every rule by hand, in advance. |
| **Training** | Showing a computer many labeled examples, so it can learn a pattern. |
| **Label** | The correct answer attached to one example. Example: "cat" or "dog." |
| **Model** | What an AI builds after training. Its own learned pattern, stored inside the software. |
| **Prediction** | A model's best guess about something new, after training is done. |
| **Accuracy** | How often a model's guess turns out to be correct. |
| **Bias** | When a model's training examples are not fair or complete, so its guesses are less fair too. |
| **Error** | A case when a model's best guess is wrong. |
| **Deepfake** | A fake photo or video, made by AI, that looks real. |
| **Privacy** | Keeping your personal data safe from misuse. |
| **Neural network** | A machine-learning model built from layers of small, simple units, each passing its result to the next layer. |
| **Automation** | A machine repeating a fixed set of steps, with no person doing each one. Not always AI. |
| **Image recognition** | An AI domain: identifying what is in a photo or video frame. |
| **Recommendation system** | An AI domain: guessing what a person will want next. |
| **Voice & language processing** | An AI domain: turning speech or text into an understood request. |
| **Fraud & anomaly detection** | An AI domain: flagging activity that looks unlike the normal pattern. |
| **Generative AI** | A model trained to produce new content, such as text or images, instead of only labeling existing content. |

---

## 2. The Folder That Knew Your Dog's Name, Step by Step

This is the full version of the story from class. The slide version was
shortened. Read this at home if you want more detail.

A student opens her phone's photo app. It has already sorted her
photos into folders, one folder per person's face. One folder is
named after her little sister. But a photo of the family dog sits in
that same folder too.

She never told the app to do this. She never even asked it to sort
her photos at all. She has no idea how the app made this choice,
right or wrong.

Here is what likely happened, using this week's words:

1. **Training** happened long before, on thousands of labeled family photos.
2. The app's **model** learned patterns: fur, shapes, and colors near the family's faces.
3. Her dog's photo matched some of those patterns, by pure coincidence.
4. The model's **prediction** was still wrong: a dog is not her sister.

This is a normal AI **error**, not a broken app. She can fix it
herself: tell the app "no," and it can learn from her correction.
Over time, small corrections like this make the model's guesses
better.

---

## 3. Rules vs. Learning: Two Ways to Build Software

Old, rule-based software follows rules a programmer writes by hand.
Example: "if it has pointy ears and whiskers, call it a cat." Real
photos break simple rules like this all the time. A cat can hide its
ears, or sit in shadow, or face away from the camera.

AI software works differently. Instead of a hand-written rule, a
programmer shows the software 10,000 labeled cat photos, and lets it
learn on its own what a cat usually looks like. This is why AI can
handle messy, real-world photos better than a simple fixed rule can.

Training itself takes many examples, and often a long time, on
powerful computers. Once training is done, the finished model is
ready. It no longer needs the answer key. It can now make a
**prediction** about a brand-new example it has never seen before.

---

## 4. Optional Reading: More Detail

This section holds extra detail that was trimmed from the slides. It
is optional, but useful if you want to go deeper.

**Where the idea came from.** In 1950, Alan Turing asked a simple
question: "Can a machine think?" In 1956, a small workshop at
Dartmouth College first used the words "artificial intelligence." For
decades after that, computers were too slow, and there was too little
data, to make the idea very useful. Starting in the 2010s, far more
data and much faster chips finally made today's AI possible. AI is an
old idea. It only recently became powerful enough to use every day.

**Why bias happens.** If a model's training photos show mostly one
type of face, lighting, or background, the model learns that type
best, and struggles with anything less common in its training data.
This is called **bias**. It is not the model being unkind on purpose.
It is a direct result of what it was, and was not, shown during
training. This is why AI ethics reviewers are part of many modern
tech teams: someone has to check whether training data is fair before
a model reaches real users.

**Why this matters in industry.** "Explain how a recommendation or a
face-matching tool decides" is now a common interview and on-the-job
question, in many roles, not only AI-specific ones. Photo apps,
streaming apps, spam filters, and maps apps all quietly use AI
already. Understanding, even at a basic level, how these tools learn
and where they can fail is now a widely useful skill.

**Who works with AI.** Real engineering and business jobs map onto
this week's ideas:

- **AI / ML engineer** — builds and trains models.
- **Data scientist** — studies data for useful patterns.
- **Data labeler** — labels examples used for training.
- **AI ethics reviewer** — checks models for bias and fairness.
- **Product manager** — decides where AI should help users.
- **Security analyst** — guards the data used for training.

**Neural networks: learning in layers.** Machine learning is not one
single technique. Today, most modern AI tools are powered by **neural
networks**, a layered kind of machine learning built from layers of
small, simple units, each passing its result to the next layer. The
first layer looks at raw input, like a photo's individual pixels.
Each next layer combines the layer before it into a slightly bigger
pattern: edges, then shapes, then a whole face. The last layer turns
those combined patterns into one final guess. No single layer
"understands" a face; the pattern only appears once all the layers
work together. A simple rule-based example, like an if-then
thermostat ("if room temperature is below 18°C, turn on the heater"),
shows the older approach by contrast: the rule never changes unless a
person edits the code by hand, and no example was ever learned.

**The four AI application domains.** Beyond the photo-sorting example
from class, AI shows up in four named domains: **image recognition**
(a hospital's scan-reading tool highlights an area matching past,
confirmed cases, though a doctor still makes the final call),
**recommendation systems** (a streaming app finds viewers with a
similar pattern to yours, and suggests what they liked),
**voice & language** (a voice assistant converts spoken words into
text, then matches that text to the closest known request), and
**fraud & anomaly detection** (a bank flags a charge that does not
match your usual pattern, without ever "knowing" for certain it is
fraud).

**AI and automation are not the same thing.** **Automation** means a
machine repeats a fixed set of steps, with no person doing each one.
Not all automation is AI: a dishwasher automates cleaning using one
fixed cycle, with no learning at all. AI is one way to build smarter
automation, when the fixed steps are not known in advance.

**Generative AI.** **Generative AI** is a model trained to produce
new content, such as text or images, instead of only labeling
existing content. It is trained on huge amounts of existing text or
images, learns the patterns behind them, and then predicts a
plausible new result from a short prompt, one piece at a time. The
result is a new pattern-based guess, not a fact retrieved from a
database.

---

## 5. Practice Problems (with Answers)

Try each problem yourself before checking the answer.

**Problem 1.** In your own words, explain the difference between
rule-based software and AI software, in one or two sentences.

> **Answer:** Rule-based software follows rules a person wrote by
> hand. AI software learns its own patterns from many examples,
> instead of following a fixed rule.

**Problem 2.** Name two AI tools you already use on your own phone or
laptop, and say what each one predicts or recognizes.

> **Answer (sample):** A keyboard predicts the next word you will
> type. A streaming app recommends the next video or song to watch.

**Problem 3.** A face-unlock feature on a phone fails more often for
some users than others. What is the most likely cause?

> **Answer:** Bias in the training data. If the training photos did
> not include enough examples like that user's face, the model learns
> that type less well.

**Problem 4.** True or false: "An AI model's wrong guess means the
app is broken." Explain your answer in one sentence.

> **Answer:** False. A wrong guess is a normal error, a pattern match
> that did not fit this one case; it does not mean the software is
> broken.

**Problem 5.** Put these four steps in the correct order: prediction,
labeled examples, training, model.

> **Answer:** Labeled examples → training → model → prediction.

**Problem 6.** A friend says, "AI understands photos the same way a
person does." Explain, in one or two sentences, why this is not
accurate.

> **Answer (sample):** AI only matches patterns it learned from
> training examples. It does not understand meaning the way a person
> does; a totally new situation can still confuse it.

**Problem 7.** A dishwasher runs one fixed cleaning cycle every time.
Is this AI? Explain in one sentence.

> **Answer:** No, it is plain automation. It repeats one fixed set of
> steps, with no learning from examples involved.

**Problem 8.** Name one of the four AI application domains covered
this week, and give one example.

> **Answer (sample):** Fraud & anomaly detection: a bank flagging a
> purchase that does not match your usual spending pattern.
