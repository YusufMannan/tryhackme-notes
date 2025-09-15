# TryHackMe – Windows Fundamentals

**Date:** Sep 2025  
**Room Link:** (https://tryhackme.com/room/windowsfundamentals)

---

## 🏆 Learning Objectives
- Gain a general overview of the Windows OS.  
- Learn the history of Windows versions.  
- Understand the Windows GUI: desktop, start menu, taskbar, notification area.  
- Explore the NTFS file system, permissions, and alternate data streams (ADS).  
- Understand the Windows folder, environment variables, and System32.  
- Manage user accounts, profiles, and groups.  
- Learn about User Account Control (UAC).  
- Explore Settings vs. Control Panel.  
- Use Task Manager to monitor processes and performance.  

---

## 🖥️ Steps I Took

### 🌐 Introduction & VM Setup
- Windows OS is a complex system with many files, utilities, and settings.  
- VM provided via TryHackMe for hands-on exploration.  
- Credentials: `administrator / letmein123!`.  
- Access via browser or Remote Desktop (RDP).  

---

### 📜 Windows History
- Windows has existed since 1985; dominant in home and enterprise.  
- **Windows XP**: long life cycle, widely adopted.  
- **Windows Vista**: unpopular, quickly phased out.  
- **Windows 7**: stable, heavily adopted, but also given end-of-life dates.  
- **Windows 8.x**: short-lived.  
- **Windows 10 & 11**: modern versions, Windows 11 is current (Home & Pro editions).  
- Server edition: **Windows Server 2025** is the latest.  
- VM used: **Windows Server 2019 Standard**.  

---

### 🖼️ Windows Desktop (GUI)
- **Login screen** requires username/password.  
- **Desktop**: quick access to files/folders/programs; customizable via right-click menu, Display settings, and Personalize.  
- **Start Menu**:  
  - Left side → account settings, documents, pictures, shutdown/restart.  
  - Middle → recently added + installed apps (alphabetical).  
  - Right side → tiles for apps/utilities, customizable.  
- **Taskbar**: shows running programs; hover for preview thumbnails; can pin items for persistence.  
- **Notification Area**: bottom right with time, volume, network, etc.; customizable in Taskbar settings.  

---

### 📂 File System (NTFS)
- Modern Windows uses **NTFS**.  
- Previous systems: FAT16/FAT32 and HPFS (still used in USB/memory cards).  
- **NTFS Features**:  
  - Files >4GB.  
  - Permissions per file/folder.  
  - Compression & Encryption (EFS).  
  - Journaling for recovery.  
- **Permissions**: Full Control, Modify, Read/Execute, List Contents, Read, Write.  
- **Alternate Data Streams (ADS)**: hidden streams attached to files, used by malware but also for metadata (e.g., download origin).  

---

### 🗂️ Windows Folder & System32
- Traditionally `C:\Windows`, but can reside elsewhere.  
- **%windir%** environment variable points to the correct folder.  
- **System32**: contains critical OS files and tools; deleting contents can break Windows.  

---

### 👤 User Accounts & Profiles
- **Administrator**: full system changes (add/delete users, modify settings).  
- **Standard User**: restricted, can only change own files.  
- User profiles stored in `C:\Users\Username`.  
- Profile created at first login (User Profile Service runs).  
- Default profile folders: Desktop, Documents, Downloads, Music, Pictures.  
- **Local Users & Groups (lusrmgr.msc)**:  
  - Manage users and groups.  
  - Groups define permissions; users can belong to multiple groups.  

---

### 🛡️ User Account Control (UAC)
- Introduced in Windows Vista to mitigate risks of always running as admin.  
- By default, admins run with standard privileges until elevated.  
- UAC prompt triggers when elevated action is requested.  
- Standard user accounts see a **shield icon** on programs requiring elevation.  
- Prevents malware from easily gaining system control.  

---

### ⚙️ Settings vs. Control Panel
- **Control Panel**: traditional location for system changes (printers, uninstalling programs).  
- **Settings Menu**: introduced in Windows 8, now primary in Windows 10/11.  
- Often interlinked (e.g., Network settings → opens Control Panel for adapter options).  
- Best approach: search in Start Menu for desired setting.  

---

### 📊 Task Manager
- Monitors running applications, processes, CPU, and RAM usage.  
- Access via right-click on Taskbar.  
- Opens in **Simple View** by default; expanded with **More Details**.  
- Critical for troubleshooting performance issues and investigating processes.  

---

## ⚠️ Challenges
- Understanding differences between NTFS permissions vs. user/group roles.  
- Balancing security vs. usability with UAC.  
- Navigating Settings vs. Control Panel (overlap can be confusing).  
- Recognizing which processes are safe or malicious in Task Manager.  

---

## 📌 Takeaways
- Windows has evolved significantly from XP to 11, with a strong focus on security and usability.  
- NTFS provides advanced features like permissions, compression, encryption, and ADS.  
- The **System32 folder** is critical — tampering with it can break Windows.  
- Proper user account management (using Standard Users when possible) strengthens system security.  
- UAC prevents automatic privilege abuse by malware.  
- Both **Settings** and **Control Panel** are important, but Settings is now primary.  
- Task Manager is an essential tool for monitoring performance and troubleshooting.  

---

## 🚀 Next Steps
- Explore advanced Windows tools:  
  - Windows Defender & Firewall.  
  - Microsoft Management Console (MMC).  
  - Core Windows processes.  
- Practice using user management, permissions, and Task Manager in depth.  
- Continue with other TryHackMe rooms: **Core Windows Processes**, **Bash Scripting**, **Regular Expressions**, etc.  

---
