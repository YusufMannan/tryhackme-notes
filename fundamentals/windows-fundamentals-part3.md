# Windows Fundamentals 3 Notes

## Windows Update
- **Purpose**: Provides security updates, patches, and feature enhancements for Windows and Microsoft products.  
- **Patch Tuesday**: Updates are released on the 2nd Tuesday of each month. Critical updates may be released anytime.  
- **Access**:  
  - Via *Settings → Update & Security → Windows Update*.  
  - Or use `control /name Microsoft.WindowsUpdate`.  
- **Behavior**: Updates can be postponed but not ignored permanently. A restart may be required.  
- **Recommendation**: Keep updates enabled to maintain security.

---

## Windows Security Overview
- **Access**: Found in *Settings*.  
- **Protection Areas**:  
  - Virus & Threat Protection  
  - Firewall & Network Protection  
  - App & Browser Control  
  - Device Security  
- **Status Icons**:  
  - Green = fully protected  
  - Yellow = needs review  
  - Red = immediate attention required  

---

## Virus & Threat Protection
### Current Threats
- **Scan Options**:  
  - Quick Scan → common folders.  
  - Full Scan → all files/programs.  
  - Custom Scan → chosen files/locations.  
- **Threat History**:  
  - Last Scan  
  - Quarantined Threats  
  - Allowed Threats (not recommended unless certain).  

### Settings
- **Manage Settings**:  
  - Real-time protection  
  - Cloud-delivered protection  
  - Automatic sample submission  
  - Controlled folder access  
  - Exclusions (use cautiously)  
  - Notifications  
- **Updates**: Definitions can be updated manually.  
- **Ransomware Protection**: Requires controlled folder access + real-time protection.  
- **Tip**: Right-click a file/folder → *Scan with Microsoft Defender*.  

---

## Firewall & Network Protection
- **Definition**: Controls traffic allowed through ports.  
- **Profiles**:  
  - Domain → authenticated to domain controller.  
  - Private → home/private networks.  
  - Public → public Wi-Fi (default).  
- **Options**: Enable/disable firewall, block all incoming connections.  
- **App Rules**: Allows or blocks apps through firewall per profile.  
- **Advanced Settings**: Available via `WF.msc` (for advanced users).  

### Microsoft Defender SmartScreen
- Protects against phishing, malware, and malicious downloads.  
- Checks apps, files, and websites.  

### Exploit Protection
- Built-in protection against exploit attacks.  
- Recommended to leave defaults.  

---

## Device Security
### Core Isolation
- **Memory Integrity**: Protects high-security processes from malicious code injection.  

### Security Processor (TPM)
- **Trusted Platform Module (TPM)**:  
  - Hardware crypto-processor.  
  - Provides tamper-resistant cryptographic operations.  
  - Ensures integrity during startup.  

---

## BitLocker
- **Definition**: Drive encryption tool to protect data from theft or exposure.  
- **Best with TPM**: Offers strongest protection when paired with TPM 1.2 or later.  
- **Purpose**: Ensures computer hasn’t been tampered with offline.  

---

## Volume Shadow Copy Service (VSS)
- **Function**: Creates snapshots/restore points of system data.  
- **Uses**:  
  - Create restore point  
  - Perform system restore  
  - Configure restore settings  
  - Delete restore points  
- **Security Note**: Malware often deletes shadow copies to block recovery.  
- **Storage**: Located in *System Volume Information* folder.  

---

## Key Takeaways
- **Windows Update**: Essential for system security.  
- **Windows Security**: Centralized management for protective tools.  
- **Defender Antivirus**: Scans, quarantines, and updates.  
- **Firewall & SmartScreen**: Guards against unauthorized access and malicious sites/files.  
- **Device Security**: Core isolation and TPM secure high-level processes.  
- **BitLocker**: Encrypts data at rest for theft protection.  
- **VSS**: Enables restore points but can be targeted by ransomware.  

---

## Further Reading
- Antimalware Scan Interface  
- Credential Guard  
- Windows Hello  
- CSO Online – Best new Windows 10 security features  
- **Living Off The Land**: Attackers abusing built-in Windows tools. Learn more [here](https://lolbas-project.github.io).
