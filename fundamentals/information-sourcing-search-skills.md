# TryHackMe – Information Sourcing & Search Skills

**Date:** Feb 22, 2025  
**Room Link:** (add TryHackMe room link here)

---

## 🏆 Learning Objectives
- Evaluate information sources for credibility.
- Use search engines efficiently with advanced operators.
- Explore specialized search engines for cybersecurity.
- Read and utilize technical documentation.
- Leverage social media for professional growth.
- Stay updated using cybersecurity news outlets.

---

## 🖥️ Steps I Took
1. Learned how to evaluate information based on:
   - Source credibility.
   - Evidence and reasoning.
   - Objectivity vs. bias.
   - Corroboration across multiple sources.
2. Practiced advanced search engine operators:
   - `"exact phrase"`
   - `site:`
   - `-` (exclude results)
   - `filetype:`
3. Explored specialized search engines:
   - **Shodan** → internet-connected devices.
   - **Censys** → internet hosts, websites, certificates.
   - **VirusTotal** → file/URL scanning.
   - **Have I Been Pwned (HIBP)** → breached email accounts.
   - **CVE/NVD** → official vulnerability identifiers.
   - **Exploit Database / GitHub** → exploit and PoC code.
4. Checked examples of official documentation:
   - Linux man pages (`man ip`).
   - Microsoft Technical Documentation.
   - Product docs (Snort, Apache, PHP, Node.js).
5. Understood the role of social media and news outlets in cybersecurity:
   - Avoid oversharing personal info.
   - Follow companies, experts, and security groups.
   - Track trends, advisories, and new threats.

---

## 🔑 Key Concepts & Tools
- **Search Engine Skills:** refining queries with operators.
- **Specialized Engines:**
  - Shodan, Censys, VirusTotal, HIBP, CVE, Exploit-DB.
- **Documentation Sources:** man pages, Microsoft Docs, vendor docs.
- **Social Media:** LinkedIn, Twitter, forums → follow trusted experts.
- **News Outlets:** for up-to-date cyber threat reports.

---

## ⚠️ Challenges
- Distinguishing credible sources from opinion pieces or biased articles.
- Remembering which specialized tool to use for each type of query.
- Managing information overload while staying focused.

---

## 📌 Takeaways
- Evaluating sources is crucial to avoid misinformation.
- Advanced search operators save time and provide precise results.
- Specialized search engines (Shodan, Censys, VirusTotal, HIBP, CVE, Exploit-DB) are essential in both red and blue team work.
- Official documentation is always the most reliable source.
- Social media and news outlets help professionals stay current but require careful filtering.

---

## 📖 Appendix: Quick Reference Cheat Sheet

### 🔍 Search Engine Operators (Google Examples)

| Operator         | Use Case                                         | Example                                    |
|------------------|-------------------------------------------------|--------------------------------------------|
| `"exact phrase"` | Search for an exact phrase                      | `"passive reconnaissance"`                 |
| `site:`          | Limit results to a specific site/domain         | `site:tryhackme.com success stories`       |
| `-`              | Exclude terms from results                      | `pyramids -tourism`                        |
| `filetype:`      | Search for specific file types                  | `filetype:ppt cyber security`              |

---

### 🛠️ Specialized Cybersecurity Search Tools

| Tool              | Purpose                                                      | Example Use Case                              |
|-------------------|-------------------------------------------------------------|-----------------------------------------------|
| **Shodan**        | Search Internet-connected devices & services                 | Find servers running Apache 2.4.1             |
| **Censys**        | Search Internet hosts, domains, and certificates             | Audit open ports & rogue assets               |
| **VirusTotal**    | Multi-engine antivirus scanning for files/URLs               | Check suspicious file hashes                   |
| **Have I Been Pwned** | Check if emails appear in data breaches                  | Test if your email was leaked in a breach      |
| **CVE / NVD**     | Standardized vulnerability dictionary                        | Look up details of CVE-2024-29988              |
| **Exploit Database** | Exploit code and PoCs for vulnerabilities                 | Search for verified Heartbleed exploit code    |
| **GitHub**        | Open-source tools, PoCs, and exploit code                    | Search repos for CVE-related scripts           |

---

### 📚 Official Documentation Sources

- **Linux:** `man <command>` (e.g., `man ip`)  
- **Windows:** Microsoft Docs ([docs.microsoft.com](https://docs.microsoft.com))  
- **Products:** Snort, Apache HTTP Server, PHP, Node.js (official vendor docs)

---

### 🌐 Social Media & News

- **Social Media:** LinkedIn, Twitter (X), security forums.  
- **Best Use:** Follow trusted researchers, companies, and groups.  
- **Security News:** KrebsOnSecurity, The Hacker News, BleepingComputer, DarkReading.

---

📌 **Tip:** Always cross-check information from multiple credible sources before relying on it in security work.
