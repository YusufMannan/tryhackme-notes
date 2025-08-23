# TryHackMe – Linux Fundamentals (Part 2)

**Date:** Aug 23, 2025  
**Room Link:** [https://tryhackme.com/room/linuxfundamentalspart2]

---

## 🏆 Learning Objectives
- Connect to and control remote Linux machines using **SSH**.
- Learn about **flags and arguments** to extend command functionality.
- Use **manual (man) pages** and `--help` for documentation.
- Practice advanced filesystem commands: create, move, copy, delete, identify files.
- Understand **file permissions** and how users/groups affect access.
- Switch between users using `su`.
- Explore important Linux root directories (`/etc`, `/var`, `/root`, `/tmp`).

---

## 🖥️ Steps I Took

### 🔑 Secure Shell (SSH)
- SSH = Secure Shell, an encrypted protocol for remote access.
- Syntax:  
  ```bash
  ssh username@MACHINE_IP
  ````

* Example:

  ```bash
  ssh tryhackme@10.10.10.10
  ```
* Default account: **username = tryhackme, password = tryhackme**.
* Key points:

  * Provides encrypted communication.
  * Executes commands remotely.
  * Password input shows no visible feedback (normal).

---

### ⚙️ Flags & Arguments

* Commands can be extended with flags (switches).
* Example: `ls` lists files → but does not show hidden files by default.

  * `ls -a` → shows hidden files.
* Commands often support `--help` for usage.
* Example:

  ```bash
  ls --help
  ```
* For full documentation, use **man pages**:

  ```bash
  man ls
  ```

---

### 📂 Filesystem Management Commands

| Command | Full Name      | Purpose                     |
| ------- | -------------- | --------------------------- |
| `touch` | touch          | Create a new empty file     |
| `mkdir` | make directory | Create a new folder         |
| `cp`    | copy           | Copy file/folder            |
| `mv`    | move           | Move/rename file/folder     |
| `rm`    | remove         | Delete files or folders     |
| `file`  | file           | Identify the type of a file |



### 🔒 File Permissions & Ownership

* Use `ls -l` or `ls -lh` to view permissions.
* Example output:

  ```
  -rw-r--r-- 1 user user 0 Feb 19 10:37 file1
  ```
* **Permissions** include:

  * Read (`r`)
  * Write (`w`)
  * Execute (`x`)

#### Users & Groups

* Files are owned by a user and may also be shared with a group.
* Permissions can be set individually for **user, group, others**.

---

### 👥 Switching Between Users

* Use `su` to switch accounts.
* Example:

  ```bash
  su user2
  ```
* Login shell:

  ```bash
  su -l user2
  ```
* Requires knowing the user’s password.
* `su -l` provides full login shell → sets environment variables, starts in the new user’s home.

---

### 📂 Important Root Directories

| Directory | Purpose                                                    |
| --------- | ---------------------------------------------------------- |
| `/etc`    | System config files (e.g., `passwd`, `shadow`, `sudoers`). |
| `/var`    | Variable data like logs, databases (`/var/log`).           |
| `/root`   | Home directory for the **root** user.                      |
| `/tmp`    | Temporary files, cleared on reboot. Writable by all users. |

---

## ⚠️ Challenges

* Remembering SSH syntax and handling invisible password input.
* Understanding man pages and large help outputs.
* Avoiding mistakes with destructive commands (`rm -R`).
* Recognizing the difference between user and group permissions.

---

## 📌 Takeaways

* SSH is essential for remote Linux administration.
* Flags and arguments expand command functionality.
* Man pages (`man`) are the go-to documentation for commands.
* Core file operations: create, copy, move, delete, identify.
* Permissions control what users and groups can do.
* `su` allows user switching (with correct password).
* `/etc`, `/var`, `/root`, `/tmp` are crucial system directories.
* Practice improves fluency with commands and concepts.
