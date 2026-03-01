---
layout: post
title: "From Curiosity to Capability: Beginning My Cybersecurity Journey"
---

Over the past several months, I’ve been intentionally building a foundation in cybersecurity with the long-term goal of becoming an ethical hacker and security professional. This site documents that journey — not just what I’m learning, but how I’m thinking through problems and developing practical skill.

This first post summarizes everything I’ve worked through so far.

## Why Cybersecurity?

My interest started with a simple question: how do attackers actually think?

That curiosity quickly turned into structured study. Instead of consuming surface-level content, I began focusing on fundamentals — networking, system behavior, and how tools function under the hood.

Security is built on understanding systems deeply. So that’s where I started.

---

## Building a Networking Foundation

I began studying core networking concepts aligned with the Network+ objectives:

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

This process taught me more than any tutorial could.

---

## Tool Exploration

I’ve begun working with foundational offensive tools:

- **Netcat** — connection testing, understanding flags (`-n`, `-l`, etc.)
- **Gobuster** — DNS vs VHost enumeration
- Basic service interaction and manual probing

One key realization:

DNS enumeration and virtual host enumeration are not the same.

DNS reveals publicly registered subdomains.

VHost enumeration reveals what the web server recognizes internally — even if DNS does not expose it.

Understanding that distinction was a major conceptual breakthrough for me.

---

## Thinking Like an Analyst

As I learn tools, I’m also asking:

- How would a SOC detect this?
- What logs would show this behavior?
- What would unusual DNS traffic look like?
- How would reverse shells appear in network monitoring?

I’m not just learning how to execute commands — I’m learning how to interpret activity.

Long term, I’m especially interested in the intersection of offensive security and defensive monitoring.

---

## Lessons So Far

1. Networking fundamentals are non-negotiable.
2. DNS behavior reveals more than most beginners realize.
3. Troubleshooting broken labs builds real skill.
4. Understanding *why* a tool behaves a certain way matters more than memorizing flags.

Most importantly:

Security competence grows through iteration and reflection, not shortcuts.

---

## What’s Next

- Continue Network+ mastery
- Expand Active Directory lab complexity
- Deeper packet inspection with Wireshark
- Log analysis practice
- Documenting each technical breakthrough here

This blog exists to make my growth visible — to myself and to future employers.

If you’re reviewing this as a hiring manager, what you’ll see here is not just study notes, but applied reasoning and documented progress.

This is just the beginning.
