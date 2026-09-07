# Week 12 Handout: Computer Applications

Introduction to Computer Engineering (400507-001) · Week 12
This handout goes with the Week 12 slides. Keep it for the whole semester.

---

## 1. Glossary: Key Words

Simple, plain definitions. Read these before or after class.

| Word | Plain definition |
|---|---|
| **General-purpose computer** | One machine that runs many different jobs. |
| **Application domain** | A real-world field that uses computers, like healthcare. |
| **Specialized software** | A program built for one particular field. |
| **Fixed-purpose device** | A machine built to do only one job, forever. |
| **Simulation** | A computer model of something in the real world. |
| **E-commerce** | Buying and selling things over the internet. |
| **Transaction** | One single business action, like a payment. |
| **Medical imaging** | Using a computer to create pictures inside the body. |
| **Embedded computer** | A small computer built into another device. |
| **Mobile computing** | Using a computer wherever you go, not just at a desk. |
| **Cross-platform** | Software that runs on many kinds of devices. |
| **Ubiquitous computing** | Small computers built into ordinary objects, working quietly in the background. |
| **Home network** | A network that lets every device in a house talk to the same router. |
| **Augmented reality (AR)** | Adds digital images on top of the real world you can still see. |
| **Virtual reality (VR)** | Replaces what you see completely, with a fully digital world. |
| **Mixed reality (MR)** | Places digital objects inside the real world, so they react to real objects too. |
| **Digital twin** | A constantly updated digital copy of a real object or place. |
| **Wearable device** | A small computer built to be worn, like a smart watch or smart ring. |
| **Service robot** | A physical machine that senses its surroundings and acts, to help with a real-world task. |
| **Metaverse** | A shared virtual space where many people's digital versions of themselves can meet and interact. |
| **Multimedia** | Information that combines more than one form: text, image, audio, and video, together. |
| **Compression** | Shrinking a file's size, so it takes less storage and less time to send. |
| **JPEG** | A common way to compress a still image, like a photo. |
| **MPEG** | A common way to compress a moving video, frame after frame. |

---

## 2. Mia's Laptop: The Full Story

This is the full version of the story from class. The slide version was
shortened. Read this at home if you want more detail.

Mia's photos are safe now. They live in a database table, guarded by
a password (Week 11). But Mia only used her laptop for one narrow
job: renaming and storing 200 photos.

One evening, her family talks about their own workdays. Her sister
edits videos for an online channel. Her uncle works at a hospital,
reading scan images on a computer. A friend spends the weekend inside
a huge game world. Same kind of machine each time. Very different
jobs.

Mia's laptop is not stuck doing one job either. It is a
**general-purpose computer**: one machine that runs many different
programs, for many different jobs. Loading new software is enough to
give it a brand new job. This is different from a **fixed-purpose
device**, like a calculator or a microwave's timer, which only ever
does the one job it was built for.

Once Mia looks closely, she finds her own laptop already covers four
different fields, without her noticing:

1. **Office** — the essay she wrote for class, saved safely with the
   storage ideas from Week 5.
2. **Creative** — a photo she cropped and edited, before posting it
   online.
3. **Entertainment** — a game she played, or a show she streamed over
   the network (Week 9).
4. **Mobile** — she carried her laptop between home, class, and a
   café, using it wherever she went.

Two more fields exist, even though Mia's laptop has not used them
yet:

5. **Scientific** — computers run simulations of weather, and help
   doctors read medical scans, instead of guessing.
6. **Business** — computers run online stores and banks, keeping
   every product and every balance in a protected database (Week 11).

In every one of these six fields, the same six layers from this
semester are still there underneath: logic gates (Week 3), the CPU
(Week 4), memory and storage (Week 5), the operating system (Week 7),
programs (Week 10), and now databases and security (Week 11). Only
the top layer, the application software itself, changes to fit the
job.

---

## 3. Optional Reading: More Detail

This section holds extra detail that was trimmed from the slides. It
is optional, but useful if you want to go deeper.

**A short history of general-purpose computing.** In the 1940s, early
computers were built for one job only, like calculating artillery
paths. In 1945, John von Neumann described a machine that stores its
own program, not only its data. Because a program is just stored data
too, one machine can load a new program and get a brand new job. In
1975, personal computers reached ordinary homes for the first time.
In 2008, app stores let anyone download new software onto their own
device. Today, one phone can hold billions of possible apps, all
built on the same stored-program idea from 1945.

**Who works in each field.** Real careers map onto each application
domain: a business analyst or project manager in office work, a video
editor or sound engineer in creative work, a data scientist or
biomedical engineer in scientific work, a database administrator or
e-commerce developer in business, a game developer or streaming
engineer in entertainment, and a mobile app developer building for
phones. Each career exists because that field needs computer skills,
every single day.

**Why simulate instead of test for real?** Some real-world tests are
too costly, or too dangerous, to run directly. Crashing a real car
tests one safety design, and destroys the car in the process. A
computer simulation can crash a virtual car many times, safely, and
cheaply. Weather models and disease models predict danger before it
actually happens. Simulations save money, time, and sometimes lives.

**Not every device is general-purpose.** A calculator, a microwave's
timer, and a traffic light are all fixed-purpose devices. Each one
runs exactly one program, forever, and cannot learn a new job. A
laptop, a phone, and a desktop computer are general-purpose: new
software is enough to give any of them a brand new job.

**Why this matters in industry.** Job listings almost always name one
exact field, such as "healthcare software" or "game development," not
just generic "computer skills." Knowing which application domain
interests you helps you choose a career path, and helps you speak the
right language in an interview.

**Computers everywhere, not just laptops.** Not every computer looks
like a laptop. **Ubiquitous computing** means small computers are
built into ordinary objects, working quietly in the background: a
car's dashboard, a modern refrigerator, an elevator's control panel.
You do not "turn on" most of these computers; they are already on,
all the time. Inside one house, a **home network** lets every device,
Mia's laptop, her phone, the family smart TV, and a game console, all
share one router connection, using the same networking ideas from
Week 9. One tap in an app, like Mia saying "good morning," can reach
her thermostat and her lights at once, over that same home network.

**Three ways to blend the real and the digital: AR, VR, and MR.**
**Augmented reality (AR)** adds digital images on top of the real
world you can still see, like a shopping app that draws a virtual
sofa in your real living room. **Virtual reality (VR)** replaces what
you see completely, with a fully digital world, like a flight-training
program that puts a student pilot inside a fully virtual cockpit;
unlike AR, nothing real stays visible while VR runs. **Mixed reality
(MR)** places digital objects inside the real world so that they react
to real objects too, like a virtual character that slides off your
real desk when you tilt it; MR must constantly sense the real room,
not just paint an image over it. In short: AR adds a layer, VR
replaces the world, and MR makes the digital layer aware of the real
one.

**Digital twins, wearables, and service robots.** A **digital twin**
is a constantly updated digital copy of a real object or place; sensors
on the real object keep sending fresh data to its digital copy, so a
factory can test a repair on the twin before touching the real
machine. A **wearable device**, like a fitness tracker, smart watch,
smart glasses, or smart ring, is a computer small enough to wear all
day, trading a bigger screen for something you never have to pull out
of a pocket. A **service robot** is a physical machine that senses its
surroundings and acts, to help with a real task, like a hospital
delivery robot or a warehouse robot; today's robot only needs to
sense, move, and act, while Week 13's AI is what makes many of them
smart.

**The metaverse.** The **metaverse** is a shared virtual space, built
from VR, AR, and networks together, where many people's digital
versions of themselves can meet and interact: a virtual meeting space
where classmates sit as digital characters, or a virtual store where
you browse products alongside other shoppers. Today, the metaverse is
still an early, developing idea; not every promised use has fully
arrived yet.

**Multimedia and why we compress it.** **Multimedia** means
information that combines more than one form, text, image, audio,
and video, together; a plain essay is only text, and a silent
slideshow is only images, but a video with sound combines several
forms at once. Multimedia files are usually far bigger than a plain
text file for the same length of content, which is exactly why they
are almost always **compressed** before you ever see them: shrinking a
file's size so it takes less storage and less time to send. **JPEG**
compresses a still image, and **MPEG** compresses a moving video,
frame after frame; both trade a small amount of quality for a much
smaller file. For example, an uncompressed photo might be about 24 MB,
while the same photo saved as a JPEG is only about 3-4 MB, a small
fraction of the original size.

---

## 4. Practice Problems (with Answers)

Try each problem yourself before checking the answer.

**Problem 1.** In your own words, what is a general-purpose computer?

> **Answer:** One machine that can run many different programs, for
> many different jobs, instead of only one fixed job.

**Problem 2.** Name three of the six application domains covered this
week.

> **Answer:** Any three of: office, creative, scientific, business,
> entertainment, mobile.

**Problem 3.** A microwave's timer only ever counts down minutes. Is
this a general-purpose computer, or a fixed-purpose device? Explain
in one sentence.

> **Answer:** A fixed-purpose device. It runs one program, forever,
> and cannot be given a new job.

**Problem 4.** A hospital uses a computer to turn scan signals into a
picture of the inside of your body. Which application domain is this?

> **Answer:** Scientific (medical imaging is part of the scientific
> and medical field).

**Problem 5.** True or false: "Every application domain needs a
completely different kind of computer." Explain your answer.

> **Answer:** False. Most domains run on the same general-purpose
> design; only the installed software, and sometimes the amount of
> CPU, memory, or storage, changes.

**Problem 6.** Name one task that needs a fast CPU, and one task that
needs a lot of storage.

> **Answer:** Sample: video editing or gaming needs a fast CPU; a
> large photo or video library, or a business database, needs a lot
> of storage.

**Problem 7.** A headset places a virtual character on your real
desk, and the character slides off if you tilt the desk. Is this AR,
VR, or MR? Explain in one sentence.

> **Answer:** Mixed reality (MR). The digital object actually
> reacts to the real object's position, instead of only sitting on
> top of the video, or replacing the real world entirely.

**Problem 8.** Why is a JPEG photo usually much smaller than an
uncompressed photo of the same picture?

> **Answer:** Compression, like JPEG, shrinks a file's size so it
> takes less storage and less time to send, trading a small amount
> of quality for a much smaller file.
