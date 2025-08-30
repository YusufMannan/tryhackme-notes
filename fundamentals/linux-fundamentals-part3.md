# TryHackMe – Linux Fundamentals (Part 3)

**Date:** Aug 30, 2025  
**Room Link:** [https://tryhackme.com/room/linuxfundamentalspart3]

---

## 🏆 Learning Objectives
- Explore useful Linux utilities and applications for daily use.  
- Learn about **automation** for repetitive tasks.  
- Understand **package management** for installing and updating software.  
- Work with **service and application logging** to troubleshoot issues.  
- Advance Linux skills with practical system administration tools.  

---

## 🖥️ Steps I Took
- Noted that Part 3 builds on concepts from Part 1 and Part 2.  
- Learned this module will focus on **utilities, automation, package management, and logging**.  
- Learned that text editing in Linux can be done with **terminal editors** instead of just echo and redirection.  
- Introduced to two editors: **Nano** (beginner-friendly) and **VIM** (advanced).  
- Learned about transferring and downloading files in Linux using **wget**, **scp**, and **python3 -m http.server**.  
- Explored processes, how to view them, manage them, and control foreground/background execution.  
- Learned about automation with **cron jobs**.  
- Explored **apt repositories**, adding/removing them, and installing packages.  
- Reviewed logs in `/var/log` to monitor system and service activity.  
- Completed recap of all topics and next learning recommendations.  

---

## 🔑 Key Commands & Concepts

### 📝 Terminal Text Editors
- **Nano** → Simple and beginner-friendly. Supports search, copy/paste, jump to line, save, and exit.  
- **VIM** → Advanced editor. Benefits include customisation, syntax highlighting, and availability on almost all terminals.  

---

### 🌐 Downloading and Transferring Files
- **wget** → Download files from the web (HTTP/HTTPS).  
- **scp** → Securely copy files between local and remote systems (source → destination).  
- **python3 -m http.server** → Serve files in the current directory on port 8000 by default for download.  

---

### 🔍 Processes
- **ps** → View running processes.  
- **ps aux** → View all processes, including system ones.  
- **top** → Real-time process statistics.  
- **kill [PID]** → End a process.  
  - SIGTERM → Graceful stop.  
  - SIGKILL → Forceful stop.  
  - SIGSTOP → Pause a process.  
- **systemd** → Parent of most processes, manages services.  
- **systemctl [start|stop|enable|disable]** → Manage services at boot or runtime.  
- **Foregrounding & Backgrounding** →  
  - `&` to run in background.  
  - Ctrl + Z to pause process.  
  - fg to bring process back to foreground.  

---

### ⏰ Automation with Cron
- **crontab** manages scheduled tasks.  
- Each cron job has 6 fields:  
  MIN HOUR DOM MON DOW CMD  
- Example: backup every 12 hours:  
  0 */12 * * * cp -R /home/cmnatic/Documents /var/backups/  
- Use `crontab -e` to edit cron jobs.  
- Wildcards (`*`) can be used when specific values don’t matter.  

---

### 📦 Package Management
- Software is distributed via **apt repositories**.  
- Ubuntu has official repos, but third-party/community repos can be added.  
- Repositories are secured with **GPG keys** to verify authenticity.  

**Workflow example (Sublime Text):**  
1. Add developer’s GPG key.  
2. Create `.list` file in `/etc/apt/sources.list.d/` for repo.  
3. Update package list so apt recognizes it.  
4. Install software from the new repo.  
5. Remove repos with `add-apt-repository --remove` or by deleting the `.list` file.  
6. Remove packages with `apt remove [package]`.  

---

### 📂 Logs
- Logs stored in `/var/log`.  
- Examples:  
  - **Apache2**: access and error logs.  
  - **fail2ban**: brute force attempts.  
  - **UFW**: firewall logs.  
- Logs help monitor **system health, security, and user activity** (e.g., authentication).  
- Linux uses **log rotation** to manage log sizes automatically.  

---

## ⚠️ Challenges
- Remembering command syntax differences between foregrounding and backgrounding.  
- Understanding cron’s 6-field format (DOM vs. DOW).  
- Managing repositories securely with GPG keys.  
- Knowing where specific logs are stored for different services.  

---

## 📌 Takeaways
- Linux is powerful for daily system administration.  
- Editors (Nano/Vim) are essential for editing files quickly.  
- File transfers can be done through wget, scp, or http.server.  
- Processes are managed with ps, top, kill, and systemctl.  
- Automation with cron saves time and ensures consistency.  
- Package management with apt provides security and simplicity.  
- Logs in `/var/log` are crucial for monitoring and investigating issues.  

---
