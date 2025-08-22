# TryHackMe – Offensive Security Intro 

**Date:** Aug 20, 2025  
**Room Link:** [(https://tryhackme.com/room/introtooffensivesecurity)  

---

## 🏆 Learning Objectives
- Understand the concept of **Offensive Security** (thinking like a hacker).
- Learn how ethical hackers use tools to find vulnerabilities.
- Perform a basic directory brute force attack with **Gobuster**.
- Discover hidden pages on a website and exploit them in a safe lab environment.
- Explore potential careers in offensive security.

---

## 🖥️ Steps I Took

### 🔐 What is Offensive Security?
- Involves breaking into computer systems, exploiting bugs, and finding loopholes.
- Goal: learn hacker tactics → strengthen defenses.
- Operates legally and ethically, with permission.

---

### 🧭 Beginning the Journey
1. Opened the **terminal** (command-line interface).
2. Learned that penetration testing uses tools like **Gobuster** to enumerate hidden pages on websites.

---

### ⚡ Using Gobuster
Command used:
```bash
gobuster -u http://fakebank.thm -w wordlist.txt dir
-u specifies the target URL.

-w specifies the wordlist of page names.
```
Gobuster tests each word as a possible directory/page.



⚠️ Ethical note: In real life, ethical hackers only exploit with permission and report vulnerabilities so they can be fixed.

## 🛠️ Key Concepts Learned
- Brute-forcing directories reveals sensitive/unprotected admin pages.
- Gobuster automates hidden content discovery.
- Attackers exploit misconfigurations or negligence.
- Ethical hackers help secure systems by reporting these flaws.

## 🚀 Career Paths in Offensive Security
- Penetration Tester → Finds exploitable vulnerabilities in systems.
- Red Teamer → Simulates real-world attackers to test defenses.
- Security Engineer → Designs and maintains security systems to prevent attacks.

## ⚠️ Challenges
- Understanding Gobuster syntax at first.
- Differentiating between status codes (e.g., 200 vs. 301 vs. 403).
- Remembering that offensive actions must always stay within legal/ethical boundaries.

## 📌 Takeaways
- Offensive security is about thinking like an attacker to defend better.
- Gobuster is a core tool for content discovery during web penetration testing.
- Even basic hidden pages (like /bank-transfer) can expose critical vulnerabilities.
- Hands-on practice builds confidence and job-readiness.
- Cybersecurity careers range from testing (Pentester), to simulating adversaries (Red Team), to building defenses (Security Engineer).
