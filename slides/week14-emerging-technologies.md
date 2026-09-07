---
marp: true
theme: shintia
paginate: true
footer: 'Department of Intelligent Computing'
---

<!-- SLOT 1: Title -->
<!-- _class: title -->

# Week 14: Emerging Technologies

<span class="subtitle">Introduction to Computer Engineering (400507-001)</span>

<div class="meta">
Yushintia Pramitarini, Ph.D · Dept. of Intelligent Computing · Thu [1-3] · Seongpa Hall 701
</div>

<!-- notes: Ask everyone: "Name one smart device you own, besides your phone." Collect two or three answers. -->

---

<!-- SLOT 2: Where we are -->

# Where We Are

<div class="roadmap">
<div class="wk"><div class="n">Wk 1</div><div class="t">Introduction</div></div>
<div class="wk"><div class="n">Wk 2</div><div class="t">Computer History</div></div>
<div class="wk"><div class="n">Wk 3</div><div class="t">Boolean Logic</div></div>
<div class="wk"><div class="n">Wk 4</div><div class="t">CPU &amp; Instructions</div></div>
<div class="wk"><div class="n">Wk 5</div><div class="t">Memory &amp; Storage</div></div>
<div class="wk"><div class="n">Wk 6</div><div class="t">Application Software · Quiz 1</div></div>
<div class="wk"><div class="n">Wk 7</div><div class="t">Operating Systems</div></div>
<div class="wk review"><div class="n">Wk 8</div><div class="t">Midterm Exam</div></div>
<div class="wk"><div class="n">Wk 9</div><div class="t">Computer &amp; Internet</div></div>
<div class="wk"><div class="n">Wk 10</div><div class="t">Programming Language</div></div>
<div class="wk"><div class="n">Wk 11</div><div class="t">Databases &amp; Security</div></div>
<div class="wk"><div class="n">Wk 12</div><div class="t">Computer Applications</div></div>
<div class="wk"><div class="n">Wk 13</div><div class="t">AI · Quiz 2</div></div>
<div class="wk now"><div class="n">Wk 14</div><div class="t">Emerging Technologies</div></div>
<div class="wk review"><div class="n">Wk 15</div><div class="t">Final Exam</div></div>
</div>

<!-- notes: Point at Week 14. Say: "Today we look past AI, at what comes next. Then we prepare for the final exam." -->

---

<!-- SLOT 3: Recap + open wound -->

# Last Week, This Week

- **Last week delivered:** computers that learn patterns from examples, called AI.
- **Last week left broken:** AI is powerful today, but only one stop on a much longer road.

---

<!-- SLOT 4: The pain (Act 1 / MOTIVATE), ZERO jargon -->

# One Phone, Many Places

<div class="pain">

Jin takes a photo on his phone, in the morning.

By lunchtime, the same photo is already on his laptop. He never
used a cable.

His smart watch also knows how many steps he took. This happens
even when his phone is in another room.

His friend asks: "How does your phone even do that?" Jin says:
"I don't know. It just works."

</div>

<!-- notes: Ask: "Has something like this happened to you? A device that seems to know things by itself?" Let two or three students answer. Do not explain the cause yet. -->

---

<!-- SLOT 5: Cost of not knowing -->

# What This Actually Costs

- Not understanding these systems makes them hard to trust, or fix, when they fail.
- These ideas already sit inside phones, watches, cars, and home speakers.
- Many tech jobs now expect basic knowledge of cloud systems and connected devices.
- Without this picture, the final exam's last topics stay confusing, not connected.

<div class="why">
<strong>In industry:</strong> product teams need people who understand hardware,
software, and networks together. This week's ideas connect all three.
</div>

---

<!-- SLOT 6: Driving question -->

<!-- _class: section -->

# This Week's Question

<div class="driving-q">"What are today's biggest new computing ideas, and how do they connect?"</div>

---

<!-- SLOT 7: Learning outcomes -->

# By the End of This Week, You Can

<div class="cardlist">
<div class="card"><div class="h">Core Ideas</div><div class="d">Explain IoT, cloud computing, big data, and mobile computing in plain words.</div></div>
<div class="card"><div class="h">Everyday Examples</div><div class="d">Give one everyday example of each idea.</div></div>
<div class="card"><div class="h">Connecting to Layers</div><div class="d">Connect each new idea back to the six layers from Week 1.</div></div>
<div class="card"><div class="h">Benefits &amp; Tradeoffs</div><div class="d">Name one benefit and one tradeoff of each idea.</div></div>
<div class="card"><div class="h">Semester Summary</div><div class="d">Summarize this semester's topics, to prepare for the final exam.</div></div>
</div>

---

<!-- SLOT 8: Origin -->

# Where These Ideas Came From

<div class="thread">You just felt the pain. Where did these ideas come from?</div>

<div class="timeline">
<div class="pt"><div class="dot"></div><div class="y">2006</div><div class="d">Companies start renting computer power over the internet</div></div>
<div class="pt"><div class="dot"></div><div class="y">2007</div><div class="d">The first smartphone combines a phone and a computer</div></div>
<div class="pt"><div class="dot"></div><div class="y">2010s</div><div class="d">Small chips get cheap enough for everyday objects</div></div>
<div class="pt"><div class="dot"></div><div class="y">Today</div><div class="d">Devices everywhere collect and share more data than ever</div></div>
</div>

<div class="why">
Each idea needed the one before it. Small chips need networks.
Networks need somewhere to send data.
</div>

---

<!-- SLOT 9: Core concept -->

# Emerging Technology: Definition

<div class="thread">One term, one clear definition.</div>

> An **emerging technology** is a new computing idea. It is
> still changing how people use computers, today.

- This week covers four ideas: connected devices, shared power, big data, and mobile computers.
- Each one still uses the six layers from Week 1.

---

# Four Big Ideas

<div class="thread">This week's four ideas, in one place.</div>

<div class="appgrid">
<div class="app"><div class="name">IoT</div><div class="desc">Everyday objects connect to the internet.</div></div>
<div class="app"><div class="name">Cloud computing</div><div class="desc">Your data lives on a distant server.</div></div>
<div class="app"><div class="name">Big data</div><div class="desc">More data than one computer can hold.</div></div>
<div class="app"><div class="name">Mobile computing</div><div class="desc">A full computer, small enough to carry.</div></div>
</div>

We look at each idea, one at a time, over three short sessions.

---

<!-- NEW: Key Words Today, Part 1 -->

# Key Words Today

- **IoT (Internet of Things)** — everyday objects that connect to the internet.
- **Sensor** — a small part that senses light, motion, or heat.
- **Smart device** — an object with a chip and internet built in.
- **Wireless** — sending data with no cable, through radio signals.
- **Connected** — linked to the internet or to another device.
- **Automation** — a device acting by itself, with no person doing each step.

<!-- notes: Read each word aloud. Ask students to repeat it once. Ask: "Which word did you already know?" -->

---

<!-- NEW: Try-It preview, closes Part 1 -->

# Coming Up: Worksheet Part A

<div class="thread">Next, you will practice using these words.</div>

- In **[Worksheet Part A](materials/week14/worksheet.html)**, you match everyday objects to the right idea.
- Example: "A smart thermostat changes temperature by itself." Which idea is that?
- You will work with a partner. A guess is fine for now.

<!-- notes: Tell students to sit next to a partner for the next part. No prep needed. -->

---

<!-- NEW: Key Words Today, Part 2 -->

# Key Words Today

- **Cloud computing** — using computer power and storage over the internet.
- **Server** — a powerful computer that stores data for many users.
- **Data center** — a large building full of servers.
- **Big data** — huge amounts of data, too large for one computer.
- **Sync** — keeping the same data updated on more than one device.
- **Latency** — the short delay between asking for data and getting it.

<!-- notes: Read each word aloud. Say: "You will use several of these words in the next slides." -->

---

<!-- Act 3 / BUILD -->

# Everyday Objects That Talk

<div class="thread">IoT means small chips are now inside everyday things.</div>

<div class="appgrid">
<div class="app"><div class="name">Smart watch</div><div class="desc">Senses your steps and heart rate.</div></div>
<div class="app"><div class="name">Smart speaker</div><div class="desc">Listens for your voice, then acts.</div></div>
<div class="app"><div class="name">Smart thermostat</div><div class="desc">Senses room heat, then adjusts it.</div></div>
<div class="app"><div class="name">Fitness tracker</div><div class="desc">Counts steps, even without your phone.</div></div>
</div>

Each object still has hardware, software, and a network connection.

---

# A Watch Has Six Layers Too

<div class="thread">Even a tiny smart watch follows the same pattern.</div>

<div class="stack">
<div class="layer view"><span class="h">Watch app</span> <span class="s">the tiny screen and buttons you touch</span></div>
<div class="layer logical"><span class="h">Tiny OS &amp; chip</span> <span class="s">a small CPU, running simple instructions</span></div>
<div class="layer physical"><span class="h">Sensor &amp; radio</span> <span class="s">reads your pulse, sends data wirelessly</span></div>
</div>

Small does not mean simple. It still needs all six layers.

---

# Where Your Photo Actually Goes

<div class="thread">Jin's phone and laptop share data through the cloud.</div>

<div class="pipeline">
<div class="stage"><div class="h">1. Phone</div><div class="s">takes the photo, saves it</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">2. Network</div><div class="s">sends it over wifi or mobile data</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">3. Data center</div><div class="s">a server stores a copy, far away</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">4. Laptop</div><div class="s">asks the server, then downloads it</div></div>
</div>

No cable was ever needed. The "cloud" is just someone else's server.

---

<!-- NEW: Try-It hand-off, Worksheet Part A -->

# Try It: Worksheet Part A

<div class="thread">Now you practice. Work with a partner.</div>

- Open **[Worksheet Part A](materials/week14/worksheet.html)**.
- Match each object or scenario to IoT, cloud, or neither.
- You have about 15 minutes. Ask your partner before you ask me.

<!-- notes: Hand out Worksheet Part A. Walk around and help pairs. After 15 minutes, ask 2-3 pairs to share one answer. -->

---

<!-- NEW: Key Words Today, Part 3 -->

# Key Words Today

- **Mobile computing** — computing done on a device you can carry.
- **App store** — a place to download apps for your phone.
- **Battery life** — how long a device runs before it needs power.
- **Bandwidth** — how much data a network can send at once.
- **Portable** — small and light enough to carry anywhere.

<!-- notes: Read each word aloud. Say: "These words tie everything together today." -->

---

# From Kilobytes to Petabytes

<div class="thread">Week 5 met kilobytes and gigabytes. Big data goes further.</div>

<div class="pipeline">
<div class="stage"><div class="h">KB</div><div class="s">one short text message</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">GB</div><div class="s">one photo album, or a movie</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">TB</div><div class="s">one person's whole photo history</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">PB</div><div class="s">one company, storing everyone's data</div></div>
</div>

Big data usually means the last two sizes on this list, or bigger.

---

# More Data Than Ever Before

<div class="thread">One person's photos are tiny, next to a company's data.</div>

<div class="barchart">
<div class="bar-row">
  <div class="bar-label">One person's phone</div>
  <div class="bar-track"><div class="bar-fill short" style="width: 6%"></div></div>
  <div class="bar-value">a few hundred photos</div>
</div>
<div class="bar-row">
  <div class="bar-label">One big company, per day</div>
  <div class="bar-track"><div class="bar-fill long" style="width: 100%"></div></div>
  <div class="bar-value">billions of photos and messages</div>
</div>
</div>

Big data means data too large for one computer to hold alone.

---

# Your Phone Is Also a Computer

<div class="thread">Mobile computing is computing you carry in your pocket.</div>

- A phone from today is faster than a full computer from years ago.
- You get new software from an **app store**, not a disc or a shop.
- **Battery life** limits how long it runs. **Bandwidth** limits how fast it talks.

A phone is a full computer, built to fit in one hand.

---

# A Computer You Carry, Everywhere

<div class="thread">Week 1 found six layers. Your phone still has them all.</div>

<div class="stack">
<div class="layer view"><span class="h">Apps</span> <span class="s">the app you tap, now on a small screen</span></div>
<div class="layer logical"><span class="h">OS &amp; CPU</span> <span class="s">the OS and chip, smaller but the same idea</span></div>
<div class="layer physical"><span class="h">Battery &amp; radio</span> <span class="s">power and wireless parts, instead of a plug and cable</span></div>
</div>

Mobile computing did not replace the six layers. It just shrank them.

---

<!-- NEW: Act 3 enrichment - 4IR framing, IoT extension, big data 3Vs, 3D printing, autonomous vehicles, drones, blockchain, crypto, NFTs, closing wrap -->

# The Fourth Industrial Revolution: When Physical, Digital, and Biological Meet

<div class="thread">One big label for everything this week studies.</div>

> The **Fourth Industrial Revolution (4IR)** describes today's wave of change, where physical machines, digital computing, and living systems increasingly work together.

- A sensor (physical) sends data to software (digital) that helps a doctor treat a patient (biological).
- Earlier waves added steam power, then electricity, then computers. This wave blends all three areas at once.
- IoT, big data, 3D printing, and the other ideas today are all pieces of this same wave.

---

# Case Study: Jin's Devices, Talking to Each Other

<div class="thread">Back to Jin's watch and phone, now with a third device.</div>

<div class="pipeline">
<div class="stage"><div class="h">1. Watch</div><div class="s">senses Jin finished a run</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">2. Phone</div><div class="s">receives that update over a wireless connection</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">3. Smart speaker</div><div class="s">announces "Nice run, Jin," using the same home network</div></div>
</div>

None of these three devices needed a cable, or a person carrying data between them by hand.

---

# Big Data's Three Signs: Volume, Variety, Velocity

<div class="thread">A clearer definition of "big," before another worked example.</div>

> **Big data** is usually described by three signs together: huge **volume**, many **varieties** of data, and fast **velocity**.

- **Volume:** far more data than one computer can hold alone.
- **Variety:** photos, text, video, and sensor readings, all mixed together.
- **Velocity:** new data keeps arriving, every second, not all at once.

---

# Case Study: How a Streaming App Recommends Your Next Show

<div class="thread">One plain example of big data actually working.</div>

- **Volume:** millions of users' viewing histories, stored together.
- **Variety:** what you watched, when you paused, and what you searched for.
- **Velocity:** the app updates its guess the moment you finish an episode.

Big data is not just "a lot of files." It is data too large, too varied, and too fast for one computer alone.

---

# 3D Printing: Building Up, Instead of Cutting Away

<div class="thread">A new kind of manufacturing, unlike anything studied so far.</div>

> **3D printing** (additive manufacturing) builds an object by adding material, layer by layer, instead of cutting it from a larger block.

- Traditional manufacturing often cuts, drills, or molds material away from a bigger piece.
- A 3D printer instead adds only the material the final object actually needs.
- A computer file describing the object's shape controls exactly where each layer goes.

---

# Tracing One 3D-Printed Object, Layer by Layer

<div class="thread">A worked example, from digital file to physical object.</div>

<div class="pipeline">
<div class="stage"><div class="h">1. 3D model</div><div class="s">a digital file describes the object's shape</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">2. Slicing software</div><div class="s">splits the shape into thin, flat layers</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">3. Printer</div><div class="s">lays down material, one layer at a time</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">4. Object</div><div class="s">the finished, physical result</div></div>
</div>

---

# 3D Printing in Practice: Two Real Uses

<div class="thread">Where this idea already leaves the lab.</div>

- **Rapid prototyping:** an engineer prints a rough part overnight, instead of waiting weeks for a factory order.
- **Custom medical models:** a hospital prints a patient-specific model, sized from that patient's own scan.

Both uses share one advantage: one single, custom copy, without building a whole factory line for it.

---

# Autonomous Vehicles: A Car That Senses and Decides

<div class="thread">A car that drives itself, conceptually, not the engineering behind it.</div>

> An **autonomous vehicle** uses sensors and software to sense the road and make its own driving decisions, without a person steering.

- Cameras, radar, and other sensors constantly scan the road around the car.
- Software combines those readings into one decision: speed up, slow down, or turn.
- The car repeats this sense-then-decide cycle many times every second.

---

# Sensor Fusion: Why One Sensor Is Not Enough

<div class="thread">The key challenge behind autonomous driving.</div>

> **Sensor fusion** combines readings from several different sensors, so their weaknesses do not all fail at once.

- A camera can be fooled by bright glare, or heavy fog.
- Radar still detects a nearby car's shape, even when the camera cannot see clearly.
- Combining both readings gives a safer answer than trusting either sensor alone.

---

# Drones: Flying Computers With Their Own Rules

<div class="thread">A smaller, flying cousin of the autonomous vehicle.</div>

> A **drone** is a small, uncrewed flying vehicle, controlled remotely or partly by its own software.

- Sensors keep the drone stable in the air, and help it avoid obstacles.
- Drones already deliver small packages, inspect power lines, and capture aerial video.
- Unlike a car, a drone shares open airspace with planes, helicopters, and other drones.

---

# Airspace Rules: Why a Drone Cannot Fly Just Anywhere

<div class="thread">The key challenge behind everyday drone use.</div>

- Airspace near an airport is tightly restricted, to keep drones away from landing planes.
- Many regions require a drone to stay within the operator's sight, and below a set height.
- These rules exist because one careless drone can risk a much larger, crewed aircraft.

---

# Blockchain: A Ledger No Single Person Controls

<div class="thread">A new way to keep a shared record, without hype.</div>

> A **blockchain** is a shared record of transactions, copied across many computers, where each new entry links back to the one before it.

- No single company or person holds the only copy of the record.
- Many computers each keep a matching copy, and compare notes before accepting a new entry.
- Changing one old entry would break its link to every entry after it, so old entries are very hard to quietly alter.

---

# Tracing One Blockchain Record

<div class="thread">A worked example, one recorded transfer at a time.</div>

<div class="pipeline">
<div class="stage"><div class="h">1. Transaction</div><div class="s">someone records "A sends one unit to B"</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">2. Verification</div><div class="s">many computers check that the record is valid</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">3. New block</div><div class="s">the accepted record joins the chain, linked to the last block</div></div>
</div>

Every later block links back to this one, which is what makes quietly editing it so difficult.

---

# Cryptocurrency: Digital Money Built on a Blockchain

<div class="thread">One well-known use of a blockchain, described plainly.</div>

> **Cryptocurrency** is digital money whose transactions are recorded on a blockchain, instead of by one central bank.

- Sending cryptocurrency records a new transaction, verified the same way as any other blockchain entry.
- Its value can rise or fall quickly, since no central bank manages its supply the way ordinary currency is managed.
- This slide is conceptual only. It is not advice about buying, holding, or trading anything.

---

# NFTs: A Unique Digital Record, Not a Copy

<div class="thread">A second, different use of the same underlying idea.</div>

> An **NFT (non-fungible token)** is a blockchain record proving one person owns one specific, unique digital item.

- "Non-fungible" means not interchangeable: each NFT points to one particular item, not an identical unit like a coin.
- Owning the NFT record does not stop other people from viewing, or even copying, the underlying image or file.
- Like cryptocurrency, this slide describes the concept only, neutrally, without investment advice.

---

# Cryptocurrency vs. NFTs: Two Different Ideas

<div class="thread">Same underlying technology, two different jobs.</div>

<div class="two-col">
<div>
<strong>Cryptocurrency</strong>
<ul><li>Interchangeable units, like digital coins</li><li>Built to be spent or exchanged</li></ul>
</div>
<div>
<strong>NFTs</strong>
<ul><li>One unique record per item</li><li>Built to prove ownership of one specific thing</li></ul>
</div>
</div>

Both sit on a blockchain. They answer two different questions: "how much do I have?" versus "who owns this one thing?"

---

# Where 4IR Ideas Already Touch Jin's Day

<div class="thread">Zooming back out, to the case study you already know.</div>

<div class="appgrid">
<div class="app"><div class="name">IoT</div><div class="desc">Jin's watch and speaker, sensing and connecting.</div></div>
<div class="app"><div class="name">Big data</div><div class="desc">His streaming app's recommendations, from millions of viewers.</div></div>
<div class="app"><div class="name">3D printing</div><div class="desc">A custom part, printed instead of factory-made.</div></div>
<div class="app"><div class="name">Autonomous vehicles</div><div class="desc">A self-driving shuttle Jin might ride to campus.</div></div>
</div>

---

# Who Builds 4IR Systems?

<div class="thread">New ideas, and the careers built around each one.</div>

<div class="appgrid">
<div class="app"><div class="name">Robotics engineer</div><div class="desc">Builds sensors and control software for machines.</div></div>
<div class="app"><div class="name">3D printing technician</div><div class="desc">Prepares and runs additive manufacturing jobs.</div></div>
<div class="app"><div class="name">Blockchain developer</div><div class="desc">Builds software that reads and writes shared ledgers.</div></div>
<div class="app"><div class="name">Data engineer</div><div class="desc">Builds the pipelines that move big data around.</div></div>
</div>

---

# Benefits and Tradeoffs of These Newer Ideas

<div class="thread">One more honest look, before the closing wrap.</div>

<div class="two-col">
<div>
<strong>Real benefits</strong>
<ul><li>Custom objects, printed on demand</li><li>Records that are hard to quietly alter</li><li>Fewer crashes, in principle, with careful sensor fusion</li></ul>
</div>
<div>
<strong>Real tradeoffs</strong>
<ul><li>3D printing is still slower than a mass factory line</li><li>Blockchain records use real computing power to maintain</li><li>Autonomous vehicles still need very careful testing</li></ul>
</div>
</div>

---

# The Field Keeps Moving: Back to This Course's Five Goals

<div class="thread">One last zoom-out, before Week 15's review.</div>

- Week 1 set five goals for this whole course: hardware and software structure, data and instructions, system software and networks, databases and multimedia, and AI, IoT, cloud, and mobile technology.
- This week's ideas, IoT, big data, 3D printing, autonomous systems, and blockchain, all extend that fifth goal, and still rest on the earlier four.
- New technology will keep appearing after this course ends. The six layers, and the habit of asking "what is actually inside this," will still apply to it.

---

<!-- SLOT N-2: Worked example -->

# Case Study: The Whole Picture, One Last Time

<div class="thread">Back to the very first case study, now complete.</div>

<div class="chip-row">
<span class="chip">IoT: your watch and speaker, both small computers</span>
<span class="chip">Cloud: your laptop's real backup, far away</span>
<span class="chip">Big data: millions of users, stored together</span>
<span class="chip">Mobile: the whole six-layer stack, in your pocket</span>
</div>

Every device this semester studied is part of one connected system now.
Hardware, software, networks, and data all work together, at once.

---

# New Tech, Old Lessons

<div class="thread">These new ideas still use skills you already learned.</div>

- **Week 3's logic gates** are still what every tiny sensor chip is built from.
- **Week 9's networks** carry every byte between your phone and the cloud.
- **Week 11's security ideas** protect your data while it sits on someone else's server.

New technology does not replace old lessons. It depends on them.

---

# Not All Upside

<div class="thread">These ideas bring real benefits, and real tradeoffs.</div>

- Your data on the cloud is convenient, but stored on someone else's computer.
- Smart devices are useful, but many quietly collect data about you.
- Big data helps companies improve products, but raises real privacy questions.
- A phone in your pocket is powerful, but only while it has signal and power.

Convenience and privacy do not always point the same direction.

---

# Four Ideas, Six Layers

<div class="thread">Every new idea still fits inside Week 1's picture.</div>

| Idea | Mainly which layer? |
|---|---|
| IoT | Hardware, plus a network connection |
| Cloud computing | Storage and networks, far away |
| Big data | Storage, at a much bigger scale |
| Mobile computing | All six layers, made small |

None of this week's ideas needed a seventh layer. They reused the six we already had.

---

# Who Builds These Systems?

<div class="thread">New ideas, but familiar kinds of jobs.</div>

<div class="appgrid">
<div class="app"><div class="name">IoT engineer</div><div class="desc">Builds the chip inside a smart device.</div></div>
<div class="app"><div class="name">Cloud engineer</div><div class="desc">Runs the servers that store your data.</div></div>
<div class="app"><div class="name">Data scientist</div><div class="desc">Finds patterns inside huge amounts of data.</div></div>
<div class="app"><div class="name">Mobile app developer</div><div class="desc">Builds apps made for phones and tablets.</div></div>
<div class="app"><div class="name">Network engineer</div><div class="desc">Keeps every device talking, reliably. Week 9.</div></div>
<div class="app"><div class="name">Security analyst</div><div class="desc">Protects data in the cloud. Week 11.</div></div>
</div>

Every job here still needs hardware, software, and network skills, together.

---

<!-- SLOT N-1: Common mistakes -->

# Common Mistakes

<div class="cardlist">
<div class="card"><div class="h">"The cloud is a real cloud, in the sky"</div><div class="d">Wrong. It is just someone else's computer.</div></div>
<div class="card"><div class="h">"IoT devices have no real computer inside"</div><div class="d">Wrong. Even a tiny sensor has a chip.</div></div>
<div class="card"><div class="h">"Big data just means a lot of files"</div><div class="d">Wrong. It means data too large for one computer.</div></div>
<div class="card"><div class="h">"A phone is just a small, weak computer"</div><div class="d">Wrong. Modern phones are surprisingly powerful.</div></div>
</div>

---

<!-- NEW: Try-It hand-off, Worksheet Part B -->

# Try It: Worksheet Part B

<div class="thread">More practice. New scenarios.</div>

- Open **[Worksheet Part B](materials/week14/worksheet.html)**.
- Match each scenario to IoT, cloud, big data, or mobile computing.
- You have about 15 minutes. Then we discuss answers together.

<!-- notes: Hand out Worksheet Part B. After 15 minutes, go through the answer key as a class. Ask for volunteers first. -->

---

<!-- SLOT N: Check yourself -->

# Check Yourself

1. Name one everyday IoT device, besides a phone.
2. Why do we call it "the cloud," if it is really just a computer?
3. Jin's watch counts his steps, without his phone nearby. Which idea explains that?

---

# Answers

1. Sample: a smart watch, a smart speaker, or a smart thermostat.
2. It is a friendly name. The data is really stored on a distant server.
3. IoT — the watch is its own small connected computer.

---

<!-- NEW: Self-check quiz hand-off -->

# Self-Check Quiz

<div class="thread">One more check, on your own.</div>

- Take the **[Week 14 Quiz](materials/week14/quiz.html)** (5-8 short questions).
- This quiz is not graded. It just checks your understanding.
- About 10 minutes. Check your own answers at the end.
- Next week's final exam review covers all fourteen weeks together.

<!-- notes: Hand out the quiz. Give students 10 minutes. Then read the answer key aloud, or let students self-check. -->

---

<!-- SLOT N+1: Limits (Act 4 / CLOSE), becomes Week 15 slot 4 -->

# What This Semester Cannot Cover Yet

<div class="limits">
The semester surveyed the whole field: hardware, logic, memory, software,
operating systems, networks, programming, databases, AI, and today's
newest ideas. Only the exam remains.
</div>

---

<!-- SLOT N+2: Bridge -->

# Next Week

Week 14 leaves **pulling it all together** unsolved. **Week 15, the
Final Exam**, addresses it: a full review, weeks 1 through 14.

---

<!-- SLOT N+3: Summary -->

# Summary

- IoT, cloud computing, big data, and mobile computing are today's newest ideas.
- Every one of them still uses the same six layers from Week 1.
- Each idea also brings a real tradeoff, usually about privacy or dependence on a network.
- This semester walked from logic gates, up to AI, and now to what comes next.
- **Reading:** review your handouts from Weeks 1-13, plus this week's handout.
- **Handout:** [materials/week14/handout.md](materials/week14/handout.html), glossary and the full worked example.
- **Prepare:** bring one question about any week's topic, for the final exam review.

---

<!-- SLOT N+4: Thank You -->
<!-- _class: end -->

# Thank You
