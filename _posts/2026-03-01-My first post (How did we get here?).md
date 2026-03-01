---
layout: post
title: "From Curiosity to Capability: Beginning My Cybersecurity Journey"
---

Over the past several months, I’ve been intentionally building a foundation in cybersecurity with the long-term goal of becoming an ethical hacker and security professional. This site documents that journey, as I thought it would be helpful to show not just what I’m learning, but how I’m thinking through problems and developing practical skill. This first post is everything that I've worked through so far. There's actually a lot to catch up on, so welcome in!

## Why Cybersecurity?

My interest started with my brother-in-law, who has been instrumental in starting me down this path. I always thought that I needed to go back to college and get my degree (and that is still a future goal of mine), but it turns out that I can learn everything I need by just committing to the process. So, I started with curiosity.

That curiosity turned into studying for the Network+. I started by consuming surface-level content, like facts of the OSI Model, the basics of subnetting, etc.  I quickly realized that just knowing the facts was not the way to go. Sure, the facts were helpful, but I needed to UNDERSTAND the concepts that I was learning so many facts about.

Security is built on understanding systems. So, I pivoted from the quick study of facts and bold terms to pursuing a deeper understanding of what I was learning. I tried to learn things to a level where I felt like I could teach them, given a textbook and a listening ear.

---

## Building a Networking Foundation

I began studying core networking concepts aligned with the Network+ objectives:

- The OSI Model
- TCP/IP fundamentals  
- DNS resolution (forward vs reverse lookups)  
- Subdomains vs virtual hosts  
- The TCP three-way handshake  
- Routing, ARP, and network categories  
- Firewall behavior and segmentation  

Rather than memorizing definitions, I’ve been working to understand what actually happens on the wire.

For example:

When using `nc 10.10.10.5 443`, I noticed connection delays.  
This led me to investigate reverse DNS lookups and the `-n` flag in Netcat.

Understanding why `nc -n` avoids DNS resolution helped me connect networking theory to real attacker and defender behavior.

That pattern — observe → question → investigate → test — is how I’m approaching everything.

---

## Home Lab Development

To move beyond theory, I built a local lab environment.

This included:

- Configuring Windows 11 networking profiles
- Troubleshooting domain authentication issues
- Working through DNS misconfigurations
- Diagnosing "host unreachable" vs "timeout" scenarios
- Making static IP configurations persistent
- Investigating why specific subnets were unreachable

Several times, configurations broke unexpectedly. Instead of restarting from scratch, I traced the issue through:

- IP addressing
- DNS configuration
- Routing tables
- Adapter settings

This process taught me more than any tutorial could. Turns out, when the Windows Server VM is not running, the Windows 11 VM cannot connect to the server. Instead of automatically jumping to the most complex solution, sometimes, the answer is as simple as: "Is the Server VM on?" This taught me to start at the baseline questions.

---

## Tool Exploration

I’ve begun working with foundational offensive tools:

- **Netcat** — connection testing, understanding flags (`-n`, `-l`, etc.)
- **Gobuster** — DNS vs VHost enumeration
- Basic service interaction and manual probing

One key realization:

DNS enumeration and virtual host enumeration are not the same.

DNS reveals publicly registered subdomains.

VHost enumeration reveals what the web server recognizes internally, even if DNS does not expose it.

Understanding that distinction was a major conceptual breakthrough for me.

---

## Lessons So Far

1. Networking fundamentals are non-negotiable.
2. DNS behavior reveals more than most beginners realize.
3. Troubleshooting broken labs builds real skill.
4. Understanding *why* a tool behaves a certain way matters more than memorizing flags.

Most importantly:

Security competence grows through iteration and reflection, not shortcuts.

## In the rearview

- Obtained my Network+ Certification
- Learning the basics from TryHackMe
- Building a functional home lab (Making sure that the server VM is on)

---

## What’s Next

- Continue learning/studying towards obtaining Security+
- Expand Active Directory lab complexity
- Deeper packet inspection with Wireshark
- Log analysis practice
- Documenting each technical breakthrough here

This blog exists to make my growth visible to future employers, myself, and those interested in following along with my journey.

If you’re reviewing this as a hiring manager, thanks for popping in. What you’ll see here is not just study notes, but applied reasoning and documented progress.
