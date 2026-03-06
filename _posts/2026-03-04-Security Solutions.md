---
layout: post
title: "Security Solutions: Firewalls, IDS, and Vulnerability Scanners"
---

Over the past several months, I’ve been intentionally building a foundation in cybersecurity with the long-term goal of becoming an ethical hacker and security professional. This site documents that journey, as I thought it would be helpful to show not just what I’m learning, but how I’m thinking through problems and developing practical skill. This post documents my time on TryHackMe's "Firewall Fundamentals", "IDS Fundamentals", and "Vulnerability Scanner Overview" rooms. Welcome in!

---

## Security Solutions

The next step on the roadmap in my cybersecurity journey is learning about Security Solutions. I've been working my way through the rooms of this module on TryHackMe, and I'm keeping details high-level to avoid spoilers for the millions of people that will for sure read this, and also to stay within platform guidelines.

These Security Solutions (Firewalls, IDS, and Vulnerability Scanners) will be employed heavily in an SOC role, so it would be good to know all that I can about them!

Firewalls provide traffic filtering for an organizations network, filtering traffic based on rules, and give control over network traffic. intrusion Detection Systems flag traffic in your host or network based on rules, signatures, or anomalies from regular usage patterns and issue an alert; and provide security to hosts or networks.Vulnerability Scans can help to patch hardware or software that has bugs or vulnerabilities.

---

## Key Concepts Covered in Firewalls Fundamentals

- The types of firewalls: Stateless, Stateful, Next-Gen Firewalls, Proxy
- Actions: Allow/Deny/Log
- Rules: Inbound/Outbound/Forwarding (routing between interfaces)
- Heuristic: analysis based on behavior patterns, rather than a threat signature. Next-Gen Firewalls have this capability.
- We got hands-on with a Windows Firewall and a Linux firewall.


## Key Concepts Covered in IDS Fundamentals
- Types of IDS and their detection capabilities: Host intrusion Detection System (HIDS) and Network Intrusion Detection System (NIDS). These firewalls may be Anomaly based, Signature based, or a Hybrid of the two.
- We got hands-on with Snort, configuring rules and accessing the local.rules file.


## Key Concepts Covered in Vulnerability Scanner Overview

- We were given an explanation of the major categorizations of scans- Authenticated vs. Unauthenticated (with credentials vs without credentials), Internal vs. External (scans within a network vs. outside of a network).
- We were given a few examples of popular vulnerability scanners, like Nessus and Qualys.
- We were given the opportunity to get hands-on with OpenVAS.
- CVSS provides a standardized severity score.


---

## What clicked for me

- Authenticated scans answer “what’s vulnerable on the inside,” not just what’s exposed.
- IDS is about detection/alerting; firewalls are about blocking/allowing.
- “Noise” is real: rule tuning matters more than installing the tool.


---

## Defender Insights

- Firewalls reduce attack surface, but misconfigurations and overly-permissive rules are common failure points.

- IDS alerts require tuning (signatures + baselines) to avoid alert fatigue.

- These tools complement each other: firewall blocks, IDS detects, vulnerability scanning identifies what needs fixing.
---

## In the Rearview

- Obtained my Network+ Certification (January of 2026)
- Building a functional home lab, including Kali, Windows 11VM, and Windows Server

---

## What’s Next

- Continue learning the basics from TryHackMe.
- Continue working in my home lab
- Continue building towards the Security+

This blog exists to make my growth visible to future employers, myself, and those interested in following along with my journey.

If you’re reviewing this as a hiring manager, thanks for popping in. What you’ll see here is not just study notes, but applied reasoning and documented progress.
