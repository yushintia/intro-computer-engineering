# Week 9 Handout: Computer & Internet

Introduction to Computer Engineering (400507-001) · Week 9
This handout goes with the Week 9 slides. Keep it for the whole semester.

---

## 1. Glossary: Key Words

Simple, plain definitions. Read these before or after class.

| Word | Plain definition |
|---|---|
| **Network** | Devices connected together, so they can send and receive data. |
| **Internet** | One huge network, made of many smaller networks worldwide. |
| **IP address** | A number that names one device, like a street address. Example: `192.168.1.5`. |
| **Wifi** | A way to join a network without a wire. |
| **Router** | A device that sends data toward the correct address. |
| **Packet** | One small piece of a message, sent on its own. |
| **Server** | A computer that stores and sends information when asked. |
| **Client** | The device that asks a server for information, like your laptop. |
| **Browser** | The app that asks a server for a webpage. |
| **URL** | The address you type to name one exact webpage. |
| **Website** | A set of connected webpages, stored on one server. |
| **Download** | Receiving data, sent from a server to your device. |
| **Upload** | Sending data, from your device to a server. |
| **Offline** | Not connected to any network, at all. |

---

## 2. Sending That Photo, Properly, Step by Step

This is the full version of the case study from class. The slide
version was shortened. Read this at home if you want more detail.

Two students sit side by side in class. One has a photo on her
screen. The other wants a copy, right now. There is no wire between
the two laptops, so nothing happens by itself. Here is what should
happen, using this week's words.

**Step 1: Join network.**
Both laptops connect to the same wifi. Without a shared network,
there is no path between them at all.

**Step 2: Get address.**
Each laptop gets its own **IP address** from the router. No two
devices on the same network can share one address, the same way no
two houses can share one street address.

**Step 3: Send request.**
One laptop asks the other for the photo. This laptop is the
**client**: the one asking a question.

**Step 4: Act as server.**
The laptop holding the photo is the **server** for this exchange. A
server does not have to be a huge machine. Even a laptop can serve a
file to another device.

**Step 5: Break into packets.**
The photo does not travel in one piece. It breaks into many small
**packets** first. Each packet can travel its own path, and packets
can arrive out of order. That is normal, not an error.

**Step 6: Reassemble.**
The client puts every packet back together, in the right order, and
shows the full photo.

No printer, no cable, no walking across the room. Just two
addresses, and one shared network between them.

**Bonus: loading a whole webpage works the same way, with more
requests.** A webpage needs many things at once: text, images, and
buttons. Your browser sends many small requests, not just one, to
build the page:

1. **Type** — you type a **URL** into your browser.
2. **Route** — the router finds the server's address.
3. **Answer** — the server sends the page back, in packets.
4. **Show** — your browser rebuilds the page and shows it.

---

## 3. Optional Reading: More Detail

This section holds extra detail that was trimmed from the slides. It
is optional, but useful if you want to go deeper.

**Where networking came from.** In 1969, US researchers built
ARPANET, so far-apart computers could share scarce, expensive
computing time. In 1989, Tim Berners-Lee built the World Wide Web, so
scientists could share documents easily. Both ideas solved the same
pain you felt in class: one machine, unable to reach any other.

**Why "walk me through what happens when you type a URL" is a famous
interview question.** It tests whether a candidate understands a
whole system, not just one narrow skill. This week's four-step
webpage-loading pipeline (Type, Route, Answer, Show) is a short
answer to that exact question.

**Who works on networks.** Real engineering jobs map onto this
week's ideas:

- **Network engineer** — builds and keeps networks running, everywhere.
- **Web developer** — builds the servers that answer browser requests.
- **Systems administrator** — manages servers and keeps them online.
- **Cloud engineer** — runs servers on someone else's machines, remotely.
- **Security analyst** — protects data as it travels across networks.
- **Network technician** — installs routers, cables, and wifi in real buildings.

**Common mistakes, and why they are tempting.**

- *"Wifi is the internet."* Wrong. Wifi is only one wireless way to
  join a network. Some networks use cables instead, with no wifi at
  all.
- *"More signal bars means faster."* Wrong. Bars show signal
  strength, not speed.
- *"The whole page arrives at once."* Wrong. It arrives as many
  small packets, which is why a big file can look "slow," then
  finish all at once.
- *"My IP address never changes."* Wrong. Many devices get a new
  address each time they join a network.
- *"A server is always a huge machine."* Wrong. Even a laptop can
  act as a server, as in the photo case study above.

---

## 4. Practice Problems (with Answers)

Try each problem yourself before checking the answer.

**Problem 1.** Name the word for "one small piece of a message, sent
on its own."

> **Answer:** Packet.

**Problem 2.** Two laptops are on the same wifi. Laptop A asks
Laptop B for a file. Which laptop is the client, and which is the
server?

> **Answer:** Laptop A is the client (it asks). Laptop B is the
> server (it answers and sends the file).

**Problem 3.** True or false: "Two devices on the same network can
share one IP address." Explain your answer in one sentence.

> **Answer:** False. Every device needs its own address, or the
> network cannot tell devices apart.

**Problem 4.** Put these four webpage-loading steps in order: the
server sends packets back, you type a URL, the browser shows the
page, the router finds the server's address.

> **Answer:** You type a URL → the router finds the server's
> address → the server sends packets back → the browser shows the
> page.

**Problem 5.** A friend says: "My wifi shows full signal bars, so my
internet must be fast." Is this correct? Explain in one sentence.

> **Answer:** No. Signal bars show signal strength, not speed; a
> strong signal can still be a slow or broken connection.

**Problem 6.** Name one everyday app, and name which part of it is
the client and which part is the server.

> **Answer (sample):** A weather app. The phone app is the client
> (asks for the forecast); the weather company's computer is the
> server (holds and sends the forecast).
