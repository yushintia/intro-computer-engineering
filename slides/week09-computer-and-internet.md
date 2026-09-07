---
marp: true
theme: shintia
paginate: true
footer: 'Department of Intelligent Computing'
---

<!-- SLOT 1: Title -->
<!-- _class: title -->

# Week 9: Computer & Internet

<span class="subtitle">Introduction to Computer Engineering (400507-001)</span>

<div class="meta">
Yushintia Pramitarini, Ph.D · Dept. of Intelligent Computing · Thu [1-3] · Seongpa Hall 701
</div>

<!--
notes: Ask everyone to check their phone's wifi icon. Ask: "What does
that icon actually mean?" Let two students guess. Do not explain yet.
-->

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
<div class="wk now"><div class="n">Wk 9</div><div class="t">Computer &amp; Internet</div></div>
<div class="wk"><div class="n">Wk 10</div><div class="t">Programming Language</div></div>
<div class="wk"><div class="n">Wk 11</div><div class="t">Databases &amp; Security</div></div>
<div class="wk"><div class="n">Wk 12</div><div class="t">Computer Applications</div></div>
<div class="wk"><div class="n">Wk 13</div><div class="t">AI · Quiz 2</div></div>
<div class="wk"><div class="n">Wk 14</div><div class="t">Emerging Technologies</div></div>
<div class="wk review"><div class="n">Wk 15</div><div class="t">Final Exam</div></div>
</div>

<!-- notes: Point at Week 9. Say: "Today one lonely machine finally gets to talk to another." -->

---

<!-- SLOT 3: Recap + open wound -->

# Last Week, This Week

- **Last week delivered:** one operating system that shares one machine fairly, among many apps.
- **Last week left broken:** that machine still cannot talk to any other machine, at all.

---

<!-- SLOT 4: The pain (Act 1 / MOTIVATE), ZERO jargon -->

# Two Laptops, One Meter Apart

<div class="pain">

Two students sit side by side in class. Each one has a laptop open.

One student has a photo on her screen. The other student wants a copy, right now.

She cannot just send it over. There is no wire between the two laptops.

She tries tapping her screen. Nothing happens. She tries saying the file's name out loud. Nothing happens.

In the end, she emails it to herself, then walks over. Two powerful machines, one meter apart, cannot say a single word to each other.

</div>

<!-- notes: Ask: "Why can't the laptops just talk directly?" Let two or three students guess. Do not explain yet. -->

---

<!-- SLOT 5: Cost of not knowing -->

# What This Actually Costs

- Without this, sharing files, browsing, or class assignments online makes no sense.
- "How does the internet work" is a classic tech interview question.
- Every "no connection" message on your phone is failing at this exact job.

<div class="why">
<strong>In industry:</strong> Network engineers keep this connection working. Their job exists because this problem is real, every single day.
</div>

---

# Where Networks Hide

<div class="appgrid">
<div class="app"><div class="name">Video call</div><div class="desc">Sends your voice and video to a friend, live.</div></div>
<div class="app"><div class="name">Online class</div><div class="desc">Loads slides and videos from a server far away.</div></div>
<div class="app"><div class="name">Group chat</div><div class="desc">Sends short messages between many phones, instantly.</div></div>
<div class="app"><div class="name">Cloud save</div><div class="desc">Sends your file to storage you cannot touch.</div></div>
</div>

Every one of these needs the exact same thing: a working network.

---

<!-- SLOT 6: Driving question -->

<!-- _class: section -->

# This Week's Question

<div class="driving-q">"How do two separate machines find each other and exchange information?"</div>

---

<!-- SLOT 7: Learning outcomes -->

# By the End of This Week, You Can

<div class="cardlist">
<div class="card"><div class="h">What a Network Is</div><div class="d">Explain what a network is, in plain words.</div></div>
<div class="card"><div class="h">Addresses</div><div class="d">Describe how an address helps one machine find another.</div></div>
<div class="card"><div class="h">Tracing a Webpage</div><div class="d">Trace what happens, step by step, when a webpage loads.</div></div>
<div class="card"><div class="h">Local Network vs. Internet</div><div class="d">Name the difference between a local network and the internet.</div></div>
</div>

---

<!-- SLOT 8: Origin -->

# Where This Idea Came From

<div class="thread">You just felt the pain. Where did the answer come from?</div>

- **1969:** US researchers built ARPANET. Far-apart computers shared scarce, expensive computing time.
- **1989:** Tim Berners-Lee built the World Wide Web, so scientists could share documents easily.

<div class="why">
Both ideas solved the same pain: one machine, unable to reach any other.
</div>

---

<!-- SLOT 9: Core concept -->

# Network: Definition

<div class="thread">One idea, one clear definition.</div>

> A **network** is devices connected together, so they can send and receive information.

- The **internet** is a network of networks, connected worldwide.
- Every device needs an **address**, so other devices can find it.

---

# Why Every Device Needs Its Own Address

<div class="thread">One idea, before we name more words.</div>

- Two houses cannot share one street address. Mail would get confused.
- Two devices cannot share one IP address, for the same reason.
- Your router gives each device on your wifi its own address.

<div class="why">
Without a unique address, a network cannot tell devices apart at all.
</div>

---

<!-- NEW: Key Words Today, session 1 -->

# Key Words Today

- **Network** — devices connected together, so they can send and receive data.
- **Internet** — one huge network, made of many smaller networks worldwide.
- **IP address** — a number that names one device, like a street address.
- **Wifi** — a way to join a network without a wire.
- **Router** — a device that sends data toward the correct address.

<!-- notes: Read each word aloud. Ask students to repeat it once. Ask: "Which word did you already know?" -->

---

<!-- NEW: Try-It preview, closes session 1 -->

# Coming Up: Worksheet Part A

<div class="thread">Next, you will practice using these words.</div>

- In **[Worksheet Part A](materials/week09/worksheet.html)**, you match everyday actions to network words.
- Example: "Turning on wifi" — which word from today matches that?
- You will work with a partner. A guess is fine for now.

<!-- notes: Tell students to sit next to a partner for the next part. No prep needed. -->

---

<!-- NEW: Key Words Today, session 2 -->

# Key Words Today

- **Packet** — one small piece of a message, sent on its own.
- **Server** — a computer that stores and sends information when asked.
- **Client** — the device that asks a server for information, like your laptop.
- **Browser** — the app that asks a server for a webpage.
- **URL** — the address you type to name one exact webpage.

<!-- notes: Read each word aloud. Say: "You will use all five words in the next slides." -->

---

<!-- Act 3 / BUILD -->

# What Does an Address Actually Look Like?

<div class="thread">A word is not enough. Let's see a real one.</div>

An IP address looks like four numbers, separated by dots: `192.168.1.5`.

- Each number can be from 0 to 255, no higher.
- Your router hands one out to every device that joins.
- No two devices on the same network share the same address.

---

# An Address for Every Machine

<div class="thread">Back to the two laptops. What were they missing?</div>

Every house has a street address. Mail cannot arrive without one.

Every device on a network needs the same thing: an **IP address**.

- Your laptop gets one address when it joins a network.
- A website's server has its own address too, somewhere far away.
- No address means no way for data to find its way there.

---

# Breaking a Message into Pieces

<div class="thread">A whole photo does not travel in one piece.</div>

A network breaks every message into small **packets** first.

- Each packet travels on its own, sometimes by a different path.
- Packets can arrive out of order. That is normal, not an error.
- The receiving device puts every packet back in the right order.

This is why a big file can look "slow," then finish all at once.

---

# Before Packets: The Line Problem

<div class="thread">Why not just send the whole photo down one open line?</div>

Early long-distance phone calls worked by reserving one whole line for one conversation, start to finish, even during silent pauses.

- Computers wanted to share a handful of expensive, long-distance lines among many people at once, not just one.
- Reserving a whole line per computer, for the whole call, would waste most of that line's capacity.
- Engineers instead chopped messages into small **packets**, so many different messages could share the same lines, taking turns.

<div class="why">
This is the same idea behind slot 8's ARPANET story, now at the level of "why packets," not just "who built it."
</div>

---

# Packet Switching in Numbers

<div class="thread">"Small pieces" sounds vague. Here are real numbers.</div>

Say a photo file is about 2,000,000 bytes (2 MB), and each packet can carry about 1,500 bytes.

- 2,000,000 ÷ 1,500 ≈ **1,333 packets**, for one single photo.
- Each packet carries a small piece of the photo, plus the destination address.
- Some packets may take a slightly different path, and still arrive within a fraction of a second of each other.

The receiving device only needs to wait for all 1,333 pieces, then reassemble them in order.

---

# Client and Server: Who Asks, Who Answers

<div class="thread">Now put an address and packets to work.</div>

<div class="pipeline">
<div class="stage"><div class="h">Client</div><div class="s">your laptop, asks a question</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Server</div><div class="s">a far-away computer, holds the answer</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Client</div><div class="s">receives packets, shows the answer</div></div>
</div>

Your browser is a client. A website lives on a server, somewhere else.

---

# Network Cheat Sheet

<div class="thread">Five words, one line each, before you practice.</div>

<div class="chip-row">
<span class="chip">IP address: names one device</span>
<span class="chip">Packet: one small piece of data</span>
<span class="chip">Router: directs data to the right address</span>
<span class="chip">Client: asks a question</span>
<span class="chip">Server: holds the answer</span>
</div>

---

# Practice Together: Trace One Request

<div class="thread">Let's do one example, out loud, as a class.</div>

You open a weather app. It needs today's forecast.

1. Your phone (**client**) sends a small request, with its own address.
2. The weather company's **server** receives it, and looks up the forecast.
3. The server sends the answer back, broken into **packets**.
4. Your phone puts the packets together, and shows the forecast.

<!-- notes: Ask the class to name which word matches each numbered step. -->

---

# How Big Is Your Network? LAN and WAN

<div class="thread">Not every network is the same size.</div>

<div class="two-col">
<div>

**LAN (Local Area Network)**
- Devices connected within one limited physical space.
- Example: one classroom's wifi, roughly 30 meters across.
- Usually owned and controlled by one person or group.

</div>
<div>

**WAN (Wide Area Network)**
- Devices connected across a wide geographic area.
- Example: the internet, spanning every country on Earth.
- Made of many smaller LANs, linked together.

</div>
</div>

---

# Meet the Hardware: The Modem

<div class="thread">Something has to connect your home to the outside world.</div>

> A **modem** is a device that converts data between your home network and the signal format your internet provider's line actually carries.

- It sits between your home network and the wider internet, like a front door.
- Without it, your home network has no way to reach anything outside itself.
- One modem usually serves one home, or one small office.

---

# Meet the Hardware: The NIC

<div class="thread">Every device needs its own way to physically join a network.</div>

> A **NIC (Network Interface Card)** is the hardware inside a device that lets it send and receive data on a network, wired or wireless.

- Your laptop's wifi chip is a NIC. So is a desktop's wired network port.
- No NIC means no way for that specific device to join any network at all.
- Most NICs today are tiny built-in chips, not a separate visible card.

---

# Meet the Hardware: The Hub

<div class="thread">One of the simplest ways to connect several wired devices.</div>

> A **hub** is a device that connects several wired devices, and repeats every incoming message out to all of them at once.

- A hub does not check addresses at all. Every device gets every message, needed or not.
- This wastes capacity as more devices join, so most networks now use smarter devices instead.
- A hub is still a useful first idea: one shared line, many devices.

---

# Meet the Hardware: The Router

<div class="thread">Something has to decide where each packet actually goes.</div>

> A **router** is a device that directs data between networks, choosing the correct path so each packet reaches the right address.

- A router hands out IP addresses to devices joining a home network.
- It decides whether a packet stays on the local network, or heads out to the internet.
- A router and a modem are not the same device, even though home setups often combine both into one box.

---

# Networking Hardware, Working Together

<div class="thread">Four devices, four different jobs, one shared path.</div>

<div class="pipeline">
<div class="stage"><div class="h">NIC</div><div class="s">joins your laptop to the network</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Hub</div><div class="s">shares the wired connection locally</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Router</div><div class="s">directs data toward the right address</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Modem</div><div class="s">converts data for the ISP's line</div></div>
</div>

Each device does one job. Together, they carry a packet from your laptop out to the internet.

---

# Networking Hardware Cheat Sheet

<div class="thread">Four devices, one line each, before we keep going.</div>

<div class="chip-row">
<span class="chip">NIC: lets one device join a network</span>
<span class="chip">Hub: repeats data to every wired device</span>
<span class="chip">Router: directs data to the right address</span>
<span class="chip">Modem: converts data for the provider's line</span>
</div>

---

# Extending the Case Study: A Home Network

<div class="thread">Put all four devices to work in one everyday place.</div>

A student's apartment has a fiber line coming in from the internet provider.

<div class="pipeline">
<div class="stage"><div class="h">Modem</div><div class="s">converts the incoming fiber signal</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Router</div><div class="s">creates the home wifi (a LAN), assigns addresses</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Laptop's NIC</div><div class="s">joins that LAN, gets its own IP address</div></div>
</div>

From here, one more step — through the router, out past the modem — reaches the wider internet: a WAN.

---

<!-- NEW: Try-It hand-off, Worksheet Part A -->

# Try It: Worksheet Part A

<div class="thread">Now you practice. Work with a partner.</div>

- Open **[Worksheet Part A](materials/week09/worksheet.html)**.
- Match each everyday action to the correct network word.
- You have about 15 minutes. Ask your partner before you ask me.

<!-- notes: Hand out Worksheet Part A. Walk around and help pairs. After 15 minutes, ask 2-3 pairs to share one answer. -->

---

# Getting Online: The DSL Family

<div class="thread">Before fiber, most homes connected another way.</div>

> **DSL (Digital Subscriber Line)** is a family of connections that send digital data over the same copper phone wires already installed in most buildings.

- A special modem lets data travel much faster than old dial-up, without blocking phone calls.
- **Broadband** is the general term for any fast, "always-on" connection, DSL included.
- DSL speed depends partly on how far a building sits from the provider's equipment.

---

# Getting Online: Fiber and Gigabit Internet

<div class="thread">A newer way to carry the same kind of data.</div>

> **Fiber-optic internet** sends data as pulses of light through a thin glass or plastic cable, instead of electrical signals over copper wire.

- Light signals can carry more data, and travel farther, with less loss than copper.
- "**Gigabit internet**" is a conceptual term for a connection fast enough to move roughly a billion bits every second.
- Faster access does not change *what* a network does, only *how quickly* it can do it.

---

# Comparing Access Speeds

<div class="thread">Same idea — a working network — at very different speeds.</div>

<div class="barchart">
<div class="bar-row">
  <div class="bar-label">Old dial-up</div>
  <div class="bar-track"><div class="bar-fill short" style="width: 4%"></div></div>
  <div class="bar-value">shares the phone line</div>
</div>
<div class="bar-row">
  <div class="bar-label">DSL broadband</div>
  <div class="bar-track"><div class="bar-fill short" style="width: 35%"></div></div>
  <div class="bar-value">always-on, faster</div>
</div>
<div class="bar-row">
  <div class="bar-label">Fiber / gigabit</div>
  <div class="bar-track"><div class="bar-fill long" style="width: 100%"></div></div>
  <div class="bar-value">fastest, most stable</div>
</div>
</div>

<div class="bar-note">Illustrative comparison only, not measured or marketed figures.</div>

---

# Mobile Generations: 1G to 3G

<div class="thread">Your phone's network has gone through several whole generations.</div>

<div class="timeline">
<div class="pt"><div class="dot"></div><div class="y">1G</div><div class="d">Analog signals carried voice calls only. No data at all.</div></div>
<div class="pt"><div class="dot"></div><div class="y">2G</div><div class="d">Digital signals added text messages alongside voice calls.</div></div>
<div class="pt"><div class="dot"></div><div class="y">3G</div><div class="d">Added real mobile internet access, at last, though a slow one.</div></div>
</div>

Each generation's "defining leap" solved one specific limit of the one before it.

---

# Mobile Generations: 4G to 6G

<div class="thread">The most recent leaps, one still barely finished.</div>

<div class="timeline">
<div class="pt"><div class="dot"></div><div class="y">4G</div><div class="d">Fast enough mobile data for smooth video streaming and modern apps.</div></div>
<div class="pt"><div class="dot"></div><div class="y">5G</div><div class="d">Much lower delay, and room for many more connected devices at once.</div></div>
<div class="pt"><div class="dot"></div><div class="y">6G</div><div class="d">Still being researched worldwide; its exact defining leap is not yet settled.</div></div>
</div>

<div class="why">
6G is deliberately described here as "still emerging." Treat any confident claim about it with caution.
</div>

---

<!-- NEW: Key Words Today, session 3 -->

# Key Words Today

- **Website** — a set of connected webpages, stored on one server.
- **Download** — receiving data, sent from a server to your device.
- **Upload** — sending data, from your device to a server.
- **Offline** — not connected to any network, at all.

<!-- notes: Read each word aloud. Say: "You will see these words in Worksheet Part B." -->

---

# From One Request to a Full Page

<div class="thread">One request is simple. A webpage needs many.</div>

A weather app needs one small answer: today's forecast.

A webpage needs many things at once: text, images, and buttons.

Your browser sends many small requests, not just one, to build the page.

---

# Finding a Name: What DNS Actually Does

<div class="thread">You type a name. The network still needs a number.</div>

> **DNS (Domain Name System)** works like a phonebook: it turns an easy-to-remember website name into the numeric IP address a computer actually needs.

- You type a website's name into your browser, not its IP address.
- Your device asks a DNS look-up: "what address matches this name?"
- Only after that answer comes back can your browser actually contact the right server.

---

# How a Webpage Loads, Step by Step

<div class="thread">Every word today, working together, in order.</div>

<div class="pipeline">
<div class="stage"><div class="h">1. Type</div><div class="s">you type a URL into your browser</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">2. Route</div><div class="s">the router finds the server's address</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">3. Answer</div><div class="s">the server sends the page back, in packets</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">4. Show</div><div class="s">your browser rebuilds the page and shows it</div></div>
</div>

<!-- notes: Ask: "Which of these four steps happens on our own laptop, and which happens far away?" -->

---

# What the Internet Actually Delivers

<div class="thread">One network, many different everyday jobs.</div>

<div class="appgrid">
<div class="app"><div class="name">Web browsing</div><div class="desc">Requests and displays pages of text, images, and links.</div></div>
<div class="app"><div class="name">Email</div><div class="desc">Sends and stores written messages between accounts.</div></div>
<div class="app"><div class="name">Streaming</div><div class="desc">Sends video or audio continuously, played as it arrives.</div></div>
</div>

Every one of these services still relies on addresses, packets, clients, and servers.

---

# The Web, Then and Now

<div class="thread">The web itself has changed, even though the network underneath has not.</div>

<div class="timeline">
<div class="pt"><div class="dot"></div><div class="y">Web 1.0</div><div class="d">Mostly read-only pages, published by a small number of people.</div></div>
<div class="pt"><div class="dot"></div><div class="y">Web 2.0</div><div class="d">Interactive and social; ordinary users post, comment, and share.</div></div>
<div class="pt"><div class="dot"></div><div class="y">Web 3.0</div><div class="d">A still-forming idea about a more open, less centrally-controlled web.</div></div>
</div>

<div class="why">
Web 3.0 is described here only as an evolving concept, not a finished or agreed-upon technology.
</div>

---

# Big Idea: Small Steps, Whole Internet

<div class="thread">Zoom out for a moment before the case study.</div>

- One request only fetches one small piece of information.
- Millions of requests, every second, build the whole internet you use.
- Every video, game, and website is built the same simple way.

<div class="why">
Every app on your phone traces back to a request like this.
</div>

---

<!-- SLOT N-2: Worked example -->

# Case Study: Sending That Photo, Properly (1/2)

<div class="thread">Back to the frozen moment. Now you have the words.</div>

Here is what should have happened, back in slot 4.

<div class="pipeline">
<div class="stage"><div class="h">Join network</div><div class="s">both laptops connect to the same wifi</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Get address</div><div class="s">each laptop gets its own IP address</div></div>
<div class="arrow">&rarr;</div>
<div class="stage"><div class="h">Send request</div><div class="s">one laptop asks the other for the photo</div></div>
</div>

---

# Case Study: Sending That Photo, Properly (2/2)

<div class="thread">The rest of the exchange, in order.</div>

- The sending laptop acts as the **server**; the other is the **client**.
- The photo breaks into small **packets**, and travels across the network.
- The client puts every packet back together, and shows the full photo.

No printer needed. Just two addresses, and one shared network between them.

---

# Who Works on Networks

<div class="thread">Real jobs, built on exactly today's ideas.</div>

<div class="appgrid">
<div class="app"><div class="name">Network engineer</div><div class="desc">Builds and keeps networks running, everywhere.</div></div>
<div class="app"><div class="name">Web developer</div><div class="desc">Builds the servers that answer browser requests.</div></div>
<div class="app"><div class="name">Systems administrator</div><div class="desc">Manages servers and keeps them online.</div></div>
<div class="app"><div class="name">Cloud engineer</div><div class="desc">Runs servers on someone else's machines, remotely.</div></div>
<div class="app"><div class="name">Security analyst</div><div class="desc">Protects data as it travels across networks.</div></div>
<div class="app"><div class="name">Network technician</div><div class="desc">Installs routers, cables, and wifi in real buildings.</div></div>
</div>

---

<!-- SLOT N-1: Common mistakes -->

# Common Mistakes (1/2)

- **"Wifi is the internet":** wrong. Wifi is just one wireless way to join a network.
- **"More signal bars means faster":** wrong. Bars show signal strength, not speed.
- **"The whole page arrives at once":** wrong. It arrives as many small packets.

---

# Common Mistakes (2/2)

- **"My IP address never changes":** wrong. Many devices get a new address each time they join.
- **"No wifi means no network":** wrong. Some networks use cables, not wifi, at all.
- **"A server is always a huge machine":** wrong. Even a laptop can act as a server.

---

<!-- NEW: Try-It hand-off, Worksheet Part B -->

# Try It: Worksheet Part B

<div class="thread">More practice. New scenarios.</div>

- Open **[Worksheet Part B](materials/week09/worksheet.html)**.
- Put the webpage-loading steps in the correct order.
- You have about 15 minutes. Then we discuss answers together.

<!-- notes: Hand out Worksheet Part B. After 15 minutes, go through the answer key as a class. Ask for volunteers first. -->

---

<!-- SLOT N: Check yourself -->

# Check Yourself

1. What does an IP address let one device do?
2. Your browser is a client. What is a server?
3. Why does a big file often arrive in small pieces?

---

# Answers

1. It lets one device find, and be found by, another device.
2. A server is a far-away computer that stores and sends information.
3. A network breaks every message into small packets first.

---

<!-- NEW: Self-check quiz hand-off -->

# Self-Check Quiz

<div class="thread">One more check, on your own.</div>

- Take the **[Week 9 Quiz](materials/week09/quiz.html)** (5-8 short questions).
- This quiz is not graded. It just checks your understanding.
- About 10 minutes. Check your own answers at the end.

<!-- notes: Hand out the quiz. Give students 10 minutes. Then read the answer key aloud, or let students self-check. -->

---

# Quick Recap: Today in Four Words

<div class="thread">Before we close, one more look at the whole picture.</div>

<div class="chip-row">
<span class="chip">Network: devices connected together</span>
<span class="chip">IP address: names one device</span>
<span class="chip">Packet: one small piece of data</span>
<span class="chip">Client and server: who asks, who answers</span>
</div>

---

<!-- SLOT N+1: Limits (Act 4 / CLOSE), becomes Week 10 slot 4 -->

# What Talking Machines Cannot Do Yet

<div class="limits">
Machines can now talk to each other, packets and all. But someone
still has to write the instructions they exchange. A server does not
know what to send back on its own. Somebody must **write that
program**. We do not know how yet.
</div>

---

<!-- SLOT N+2: Bridge -->

# Next Week

Week 9 leaves **writing the instructions machines exchange** unsolved. **Week 10,
Programming Language**, addresses it: how people actually write those instructions.

---

<!-- SLOT N+3: Summary -->

# Summary

- A network connects devices; the internet is a network of networks.
- Every device needs an address, so other devices can find it.
- Messages travel as small packets, put back together on arrival.
- A client asks; a server answers. A browser loads a page in four steps.
- **Reading:** course reading packet, "How Networks Move Data" (posted online).
- **Handout:** [materials/week09/handout.md](materials/week09/handout.html), glossary and the full webpage-loading walkthrough.
- **Prepare:** Think of one app that needs the internet to work. Bring it to Week 10.

---

<!-- SLOT N+4: Thank You -->
<!-- _class: end -->

# Thank You
