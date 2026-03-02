---
layout: post
title: "A Long Night With Shells"
---

Over the past several months, I’ve been intentionally building a foundation in cybersecurity with the long-term goal of becoming an ethical hacker and security professional. This site documents that journey, as I thought it would be helpful to show not just what I’m learning, but how I’m thinking through problems and developing practical skill. This post documents my time on TryHackMe "Shells Overview". Welcome in!

---

## Shells

The next step on the roadmap in my cybersecurity journey is dealing with shells. I've been working my way through the rooms on TryHackMe. I'm keeping details high-level to avoid spoilers for the millions of people that will for sure read this, and also to stay within platform guidelines.

I'm currently in the Offensive Security Tooling section (Cyber Security 101 > Offensive Security Tooling) which has been challenging, to say the least. It seems like for most of these rooms, there is one underlining concept that makes the whole room click. And so, you'll probably struggle until you understand that concept.

Shells are a way to get remote command processes on another machine.

Different methods of obtaining shells have been worked through previously in TryHackMe (like Metasploit payloads) and other non-metasploit attacks are known (nc -e). However, Metasploit payloads are commonly detected in many modern environments; many netcat builds don't include -e, and defenders are monitoring for common patterns. This pushed me to understand (literal) ins and outs of I/O mechanics. Enter FIFO pipe files.

The purpose of this room was to show different methods of engineering a reverse shell in various languages. Making it through this room was extremely difficult until I understood the significance of the pipe file, and how it interacts with whatever method you choose for the reverse shell and how the different methods interact with stdin, stdout, stderr. This was the key, and although the pipe file was not used in every situation, once I understood the purpose of the file, it made everything around it a lot simpler.

---

## What Clicked for Me

- What a shell is (interactive vs non-interactive)
- Reverse vs Bind
- Understanding stdin/stdout/stderr
- How a FIFO can help I/O between processes

---

## In the Rearview

- Obtained my Network+ Certification (January of 2026)
- Building a functional home lab, including Kali, Windows 11VM, and Windows Server

---

## What’s Next

- Continue learning the basics from TryHackMe. SQLMap: The Basics is next!
- Continue working in my home lab

This blog exists to make my growth visible to future employers, myself, and those interested in following along with my journey.

If you’re reviewing this as a hiring manager, thanks for popping in. What you’ll see here is not just study notes, but applied reasoning and documented progress.
