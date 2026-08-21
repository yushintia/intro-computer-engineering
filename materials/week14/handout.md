# Week 14 Handout: Emerging Technologies

Introduction to Computer Engineering (400507-001) · Week 14
This handout goes with the Week 14 slides. Keep it for the whole semester.

---

## 1. Glossary: Key Words

Simple, plain definitions. Read these before or after class.

| Word | Plain definition |
|---|---|
| **Emerging technology** | A new computing idea that is still changing how people use computers. |
| **IoT (Internet of Things)** | Everyday objects that connect to the internet. Example: a smart watch. |
| **Sensor** | A small part that senses light, motion, or heat, and turns it into data. |
| **Smart device** | An object with a small chip and internet connection built in. |
| **Wireless** | Sending data with no cable, through radio signals. |
| **Connected** | Linked to the internet, or to another device. |
| **Automation** | A device acting by itself, with no person doing each step. |
| **Cloud computing** | Using computer power and storage that live over the internet, not on your device. |
| **Server** | A powerful computer that stores data and answers requests for many users. |
| **Data center** | A large building full of servers, usually far from any one user. |
| **Big data** | Amounts of data so large that one computer alone cannot hold or study it. |
| **Sync** | Keeping the same data updated and matching, on more than one device. |
| **Latency** | The short delay between asking a server for data and getting it back. |
| **Mobile computing** | Computing done on a device small and light enough to carry. |
| **App store** | A place to download apps for your phone or tablet. |
| **Battery life** | How long a device can run before it needs power again. |
| **Bandwidth** | How much data a network connection can send at once. |
| **Portable** | Small and light enough to carry and use anywhere. |

---

## 2. One Phone, Many Places, Step by Step

This is the full version of the story from class. The slide version was
shortened. Read this at home if you want more detail.

Jin takes a photo on his phone, in the morning. By lunchtime, the
same photo is already on his laptop. He never plugged in a cable, and
he never copied a single file by hand.

His smart watch also knows how many steps he took, even when his
phone was left behind in another room. His friend asks him: "How
does your phone even do that?" Jin honestly does not know. "It just
works," he says.

Here is what is actually happening, using this week's words:

1. Jin's phone is a piece of **mobile computing**: a small but full
   computer, with its own CPU, memory, and wireless radio.
2. When Jin's phone takes a photo, it quietly **syncs** a copy to the
   **cloud**: a **server**, sitting in a **data center**, far away.
3. Jin's laptop later checks that same cloud account, over its own
   network connection, and downloads the same photo.
4. His smart watch is a tiny **IoT** device. A **sensor** on its
   underside senses his pulse and movement, without any effort from
   Jin.

Nothing here is magic. Every step still uses ordinary hardware,
software, and networks, the same six layers this course studied all
semester. The pieces are just smaller, more numerous, and more
connected than before.

---

## 3. Old Layers, New Places: How Each Idea Fits

A fair question is: are IoT, the cloud, big data, and mobile
computing really *new* layers, on top of the six from Week 1? The
short answer is no. Each idea reuses the same six layers; it just
places them somewhere new, or shrinks them.

**IoT** puts all six layers inside a very small object. A smart watch
still has hardware (a tiny chip, a sensor, a battery), software (a
tiny operating system and a small app), and a network connection
(usually wireless). It is a full, tiny computer system, not a magic
box.

**Cloud computing** moves some of those layers far away from you. The
memory and storage layers, and sometimes even some of the
processing, now live on a server in a data center, instead of on your
own device. Your phone or laptop becomes mostly a window into that
distant machine.

**Big data** is less a new layer, and more a new *scale*. The same
storage layer from Week 5 is still storage; there is simply far more
of it, spread across many servers working together, because no
single computer's storage is large enough to hold it all alone.

**Mobile computing** keeps every layer, but shrinks them to fit in
one hand: a small CPU, a small amount of memory, a small screen, and
a small battery, instead of a desktop computer's larger versions of
the same parts.

None of these four ideas needed a brand-new, seventh layer. Each one
found a new way to arrange, move, or shrink the six layers this
course has studied since Week 1.

---

## 4. Optional Reading: More Detail

This section holds extra detail that was trimmed from the slides. It
is optional, but useful if you want to go deeper.

**Where these ideas came from.** Cloud computing became widely
available around 2006, when companies began renting out spare
computer power over the internet, instead of every company buying and
running its own servers. In 2007, the first modern smartphone
combined a phone, a small computer, and internet access into one
pocket-sized device, starting the mobile computing era. Through the
2010s, computer chips became small and cheap enough to place inside
everyday objects, from watches to thermostats, starting the IoT era.
As more of these connected devices came online, the amount of data
they produced grew far beyond what one computer could store or
study, giving rise to big data.

**Real tradeoffs, not just benefits.** Every idea in this week also
carries a real cost, alongside its convenience. Storing your data on
someone else's server is convenient, but it also means trusting that
company to protect it. A smart device that senses your habits can be
genuinely useful, but it can also quietly collect data about you that
you never explicitly agreed to share. Big data helps companies build
better products, but it also raises fair questions about who owns,
and who can see, all of that combined data. None of this makes these
technologies bad; it just means using them well requires understanding
both sides.

**Why this matters in industry.** Almost every modern tech product
now touches at least one of this week's four ideas: a fitness app
uses IoT sensors and syncs to the cloud; a photo app relies on cloud
storage and big data to work well for millions of users; nearly every
new consumer product is, in some way, a piece of mobile computing.
Understanding these ideas, even at a basic level, is now assumed
knowledge for many technical interviews and real engineering roles.

**Who works in this field.** Real engineering and business jobs map
onto this week's ideas:

- **IoT engineer** — designs the small chip and sensors inside a smart device.
- **Cloud engineer** — builds and runs the servers that store data for millions of users.
- **Data scientist** — studies big data for useful, real patterns.
- **Mobile app developer** — builds the apps that run on phones and tablets.
- **Network engineer** — keeps every connected device talking reliably. Week 9's field.
- **Security analyst** — protects data sitting on someone else's server. Week 11's field.

---

## 5. Practice Problems (with Answers)

Try each problem yourself before checking the answer.

**Problem 1.** In your own words, explain what "the cloud" really is,
in one or two sentences.

> **Answer:** The cloud is not a real cloud in the sky; it is just
> computer power and storage that live on someone else's server, far
> away, reached over the internet.

**Problem 2.** Name two IoT devices you, or someone you know, already
use, besides a smartphone.

> **Answer (sample):** A smart watch, a smart speaker, a smart
> thermostat, or a fitness tracker.

**Problem 3.** A company collects millions of users' photos every
day. Why can this be called "big data," instead of just "a lot of
files"?

> **Answer:** It is called big data because the total amount is too
> large for any single computer to store or study alone; it needs
> many computers, working together.

**Problem 4.** True or false: "A smartphone is a weaker, simplified
version of a real computer." Explain your answer in one sentence.

> **Answer:** False. A modern smartphone is a full computer, with all
> six layers, simply built to fit in one hand.

**Problem 5.** Put these four size units in order, from smallest to
largest: **gigabyte, kilobyte, terabyte, petabyte**.

> **Answer:** Kilobyte → gigabyte → terabyte → petabyte.

**Problem 6.** A friend says, "Smart devices only bring benefits, no
downsides." Explain, in one or two sentences, why this is not fully
accurate.

> **Answer (sample):** Smart devices are convenient, but many quietly
> collect data about their users, which raises real privacy
> questions alongside their benefits.
