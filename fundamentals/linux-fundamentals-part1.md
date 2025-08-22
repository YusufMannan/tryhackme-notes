# TryHackMe – Linux Fundamentals (Part 1)

**Date:** Aug 22, 2025  
**Room Link:** ((https://tryhackme.com/room/linuxfundamentalspart1))

---

## 🏆 Learning Objectives
- Understand Linux as an operating system and its global usage.
- Learn about Linux distributions (flavours).
- Practice essential terminal commands (`echo`, `whoami`, `ls`, `cd`, `cat`, `pwd`).
- Explore file searching with `find`.
- Learn pattern searching with `grep`.
- Use shell operators (`&`, `&&`, `>`, `>>`) for efficiency.

---

## 🖥️ Steps I Took

### 🌍 Where Linux is Used
- Powers websites, smart cars, PoS systems, and infrastructure.
- Common in enterprise servers, Android devices, and supercomputers.

### 🐧 Linux Distributions
- Linux is based on UNIX.
- Examples: **Ubuntu, Debian**.
- Lightweight → Ubuntu Server can run with only **512MB RAM**.
- Many distributions don’t include a GUI; interaction is through the **terminal**.

### 💻 Essential Commands
- `echo` → output text.
- `whoami` → current logged-in user.
- `ls` → list directory contents.
- `cd` → change directories.
- `cat` → display file contents.
- `pwd` → print current working directory.

Example workflow:
- Use `ls` to list files → see `Documents/todo.txt`.
- Run `cat Documents/todo.txt` → outputs file contents.
- Run `pwd` → gives full path (e.g., `/home/ubuntu/Documents`).

---

## 🔎 Searching with `find`
- Search for specific files across directories without manually browsing.
- `find -name passwords.txt` → finds file by name.  
- `find -name *.txt` → finds all `.txt` files with wildcard search.

---

## 📝 Searching with `grep`
- Used to search file contents for specific values.
- More efficient than reading line by line with `cat`.

Example:
```bash
grep "81.143.211.90" access.log
Returns all log entries containing the IP 81.143.211.90.
```
Useful for searching logs (e.g., web server activity).

---

## ⚙️ Shell Operators
Operator	Purpose	Example
- &	Run a command in the background	cp largefile.txt backup/ &
- &&	Run second command only if first succeeds	mkdir test && cd test
- >	Redirect output (overwrites file contents)	echo hey > welcome
- >>	Redirect output (appends to file without erasing)	echo hello >> welcome

---

## ⚠️ Challenges
- Adjusting to a terminal-only environment without GUI. 
- Remembering directory paths and commands at first.
- Learning the difference between overwriting vs. appending (> vs. >>).

---

## 📌 Takeaways
- Linux is powerful, lightweight, and widely used across industries.
- The terminal is the core of Linux interaction.
- Mastery of basic commands leads to efficiency and confidence.
- find and grep are essential tools for searching files and contents.
- Shell operators (&, &&, >, >>) increase productivity and control.
