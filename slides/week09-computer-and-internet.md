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
Yushintia Pramitarini, Ph.D · Dept. of Intelligent Computing · Thu [1-3] · 성파 701
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

1. Explain what a network is, in plain words.
2. Describe how an address helps one machine find another.
3. Trace what happens, step by step, when a webpage loads.
4. Name the difference between a local network and the internet.

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

<!-- NEW: Key Words Today, 차시 1 -->

# Key Words Today

- **Network** — devices connected together, so they can send and receive data.
- **Internet** — one huge network, made of many smaller networks worldwide.
- **IP address** — a number that names one device, like a street address.
- **Wifi** — a way to join a network without a wire.
- **Router** — a device that sends data toward the correct address.

<!-- notes: Read each word aloud. Ask students to repeat it once. Ask: "Which word did you already know?" -->

---

<!-- NEW: Try-It preview, closes 차시 1 -->

# Coming Up: Worksheet Part A

<div class="thread">Next, you will practice using these words.</div>

- In **[Worksheet Part A](materials/week09/worksheet.html)**, you match everyday actions to network words.
- Example: "Turning on wifi" — which word from today matches that?
- You will work with a partner. A guess is fine for now.

<!-- notes: Tell students to sit next to a partner for the next part. No prep needed. -->

---

<!-- _class: section -->

# End of 차시 1
<div class="driving-q">Short break. 차시 2: how one machine actually finds another.</div>

---

<!-- NEW: Key Words Today, 차시 2 -->

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

<!-- NEW: Try-It hand-off, Worksheet Part A -->

# Try It: Worksheet Part A

<div class="thread">Now you practice. Work with a partner.</div>

- Open **[Worksheet Part A](materials/week09/worksheet.html)**.
- Match each everyday action to the correct network word.
- You have about 15 minutes. Ask your partner before you ask me.

<!-- notes: Hand out Worksheet Part A. Walk around and help pairs. After 15 minutes, ask 2-3 pairs to share one answer. -->

---

<!-- _class: section -->

# End of 차시 2
<div class="driving-q">Short break. 차시 3: watch a whole webpage load, step by step.</div>

---

<!-- NEW: Key Words Today, 차시 3 -->

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
