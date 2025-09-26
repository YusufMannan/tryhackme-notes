# TryHackMe – Windows Fundamentals (Part 2)

**Date:** Sept 2025  
**Room Link:** https://tryhackme.com/room/windowsfundamentals2

---

## 🏆 Learning Objectives
- Explore tools available via **System Configuration (MSConfig)**.  
- Learn about system utilities such as **Task Scheduler, Event Viewer, Shared Folders, Perfmon, Disk Management, Services, WMI**.  
- Use **System Information (msinfo32)** to gather hardware/software details.  
- Monitor processes and resources with **Resource Monitor (resmon)**.  
- Interact with **Command Prompt** and key commands.  
- Understand the role and risks of the **Windows Registry**.  

---

## 🖥️ Key Topics

### ⚙️ System Configuration (MSConfig)
- Purpose: **Advanced troubleshooting** and diagnosing startup issues.  
- Tabs:  
  - **General** → Choose Normal, Diagnostic, or Selective startup.  
  - **Boot** → Define OS boot options.  
  - **Services** → Lists all services (running/stopped).  
  - **Startup** → Redirects to Task Manager for managing startup apps.  
  - **Tools** → Quick access to system utilities.  

---

### 🔒 User Account Control (UAC)
- Adjusted via a **slider** in MSConfig → Tools.  
- Ranges from *Always notify* (maximum security) to *Never notify* (not recommended).  
- Protects against malware by prompting before elevated operations.  

---

### 🛠️ Computer Management (compmgmt)
Three primary sections:  
- **System Tools**  
  - **Task Scheduler** → Automates apps/scripts at login, logout, or custom schedules.  
  - **Event Viewer** → Audit trail of system/application activity. Logs include Error, Warning, Information, Audit Success, Audit Failure.  
  - **Shared Folders** → View shares (e.g., C$, ADMIN$), sessions, and open files.  
  - **Local Users and Groups** → Manage accounts, groups, and permissions.  
  - **Performance Monitor (perfmon)** → Track system performance in real-time or via logs.  
  - **Device Manager** → Manage and configure hardware devices.  
- **Storage**  
  - **Disk Management** → Partition drives, assign letters, extend/shrink volumes.  
- **Services and Applications**  
  - Manage service properties.  
  - **WMI Control** → Configures Windows Management Instrumentation (deprecated WMIC tool replaced by PowerShell).  

---

### 🖥️ System Information (msinfo32)
- Displays details on **hardware, components, and software environment**.  
- **System Summary** → General specs (CPU, RAM, OS version).  
- **Hardware Resources** → IRQs, memory, DMA (advanced).  
- **Components** → Info about installed devices (e.g., Display, Input).  
- **Software Environment** → Installed software, environment variables, network connections.  
- **Environment Variables**: Examples include `%windir%` for Windows directory.  

---

### 📊 Resource Monitor (resmon)
- Provides detailed usage statistics by **process**.  
- Sections:  
  - **CPU** – process-level CPU utilization.  
  - **Memory** – physical and virtual memory allocation.  
  - **Disk** – I/O per process.  
  - **Network** – per-process network activity.  
- Includes filtering, file handle insights, and real-time graphical views.  

---

### 💻 Command Prompt (cmd)
- Early interface for Windows OS, still widely used.  
- Useful commands:  
  - `hostname` → Show computer name.  
  - `whoami` → Show logged-in user.  
  - `ipconfig` → Display network configuration.  
  - `cls` → Clear screen.  
  - `netstat` → View TCP/IP network connections and statistics.  
  - `net` → Manage network resources (`net user`, `net localgroup`, `net share`).  
- Help options:  
  - `<command> /?` (e.g., `ipconfig /?`).  
  - `net help <subcommand>` (e.g., `net help user`).  

---

### 🗂️ Windows Registry (regedit)
- Central database storing:  
  - User profiles.  
  - Installed applications.  
  - System/hardware configuration.  
  - Ports and drivers.  
- Accessible via **Registry Editor (regedit)**.  
- **Warning**: Editing can break system functionality if misused.  
- Reference: [Microsoft Registry Documentation](https://learn.microsoft.com/en-us/windows/win32/sysinfo/registry).  

---

## 📌 Takeaways
- MSConfig is a **launchpad for critical Windows tools**.  
- Many utilities (Task Scheduler, Event Viewer, Disk Management, Perfmon, Resmon, regedit, etc.) can be launched **directly** without MSConfig.  
- Understanding these tools is key for **troubleshooting, monitoring, and managing Windows systems**.  
- The room provided practical commands and shortcuts, reinforcing hands-on familiarity.  

---
