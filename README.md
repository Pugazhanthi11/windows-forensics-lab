# windows-forensics-lab
Hands-on Windows Digital Forensics investigations covering Registry, Browser Artifacts, Prefetch, Recycle Bin, and forensic timeline analysis. Each investigation includes evidence collection, observations, analysis, and conclusions based on practical lab exercises.

# Digital Forensics Artifacts Lab

## About This Repository

This repository documents my hands-on learning journey in Digital Forensics. Instead of studying only theoretical concepts, I decided to perform practical investigations on my own Windows 11 system and document every observation, finding, and conclusion throughout the learning process.

The primary goal of this repository is to understand how Windows stores digital evidence and how investigators use different system artifacts to reconstruct user activity.

Every investigation included in this repository was performed in a controlled learning environment. The findings are based on artifacts collected directly from my own system, allowing me to understand how forensic evidence is generated during normal computer usage.

---

# Learning Objectives

The objectives of this project are:

- Learn the fundamentals of Windows Digital Forensics.
- Understand how Windows stores forensic artifacts.
- Perform hands-on investigations instead of relying only on theory.
- Develop practical evidence collection and documentation skills.
- Build a structured forensic investigation portfolio.
- Improve analytical thinking while examining digital evidence.

---

# Investigation Topics

## Day 04 – Windows Registry Forensics

Investigated important Registry artifacts including:

- RunMRU
- RecentDocs
- UserAssist
- TypedPaths
- WordWheelQuery

This investigation demonstrated how Windows records user activity within the Registry and how these artifacts can support forensic investigations.

---

## Day 05 – Windows Prefetch Forensics

Explored Windows Prefetch artifacts to understand application execution evidence.

Applications identified during the investigation included:

- Command Prompt
- Visual Studio Code
- Google Chrome

The investigation also demonstrated how Prefetch artifacts can be correlated with Registry evidence collected previously.

---

## Day 06 – Browser History & Download Forensics

Examined Google Chrome browser artifacts including:

- Browser History
- Download History

This investigation focused on understanding how browser activity contributes to digital evidence and how browsing timelines can be reconstructed.

---

## Day 07 – Advanced Browser Forensics

Extended the browser investigation by examining:

- Chrome Bookmarks
- Stored Site Data
- Cookies

The collected evidence helped demonstrate long-term browsing behavior and frequently used online services.

---

## Day 08 – Recycle Bin Forensics

Performed a controlled experiment using a sample text document.

The investigation included:

- File creation
- File deletion
- Recycle Bin analysis
- Timeline reconstruction

This practical exercise demonstrated that deleting a file does not immediately remove it from the system.

---

## Day 09 – Windows Shortcut (LNK) Forensics

Introduced Windows Shortcut artifacts and their importance during digital forensic investigations.

Topics explored included:

- LNK files
- Metadata stored inside shortcuts
- Common storage locations
- Forensic significance

---

# Skills Practiced

Throughout this project, I practiced:

- Windows Registry Analysis
- Event Correlation
- Prefetch Analysis
- Browser Artifact Investigation
- Deleted File Analysis
- Timeline Reconstruction
- Evidence Documentation
- User Activity Analysis

---

# Tools Used

The following Windows utilities were used during the investigations:

- Registry Editor
- Windows Event Viewer
- File Explorer
- Google Chrome
- Command Prompt
- Windows Recycle Bin

The purpose of using built-in Windows tools was to first understand how evidence is stored before moving to advanced forensic software.

---

# Investigation Methodology

Each investigation followed a structured approach:

1. Identify the forensic artifact.
2. Understand its purpose.
3. Locate the artifact.
4. Collect available evidence.
5. Record observations.
6. Analyze the evidence.
7. Correlate findings with previous investigations.
8. Document conclusions.

This approach helped me maintain consistency throughout the learning process.

---

# What I Learned

Working on these investigations helped me understand that digital forensics is not simply about recovering deleted files. It is about understanding how operating systems record user activity and how different artifacts can be combined to reconstruct events.

One of the biggest lessons from this journey has been that a single artifact rarely tells the complete story. Meaningful conclusions are formed by correlating evidence collected from multiple independent sources.

---

# Future Learning Roadmap

This repository will continue to grow as I explore more Digital Forensics topics, including:

- Browser Cache Analysis
- Jump Lists
- NTFS File System
- Master File Table (MFT)
- Windows Timeline
- USB Artifact Analysis
- Memory Forensics
- Network Forensics
- Linux Forensics
- Incident Response
- Malware Analysis

---

# Repository Structure

```
Digital-Forensics-Artifacts-Lab/

├── Day-04-Registry-Forensics
├── Day-05-Prefetch-Forensics
├── Day-06-Browser-History-Forensics
├── Day-07-Advanced-Browser-Forensics
├── Day-08-Recycle-Bin-Forensics
└── Day-09-LNK-Shortcut-Forensics
```

---

# Project Status

**Status:** Active Learning Project

This repository will be updated regularly as I continue exploring new forensic artifacts, tools, and investigation techniques.

---

## Connect With Me

If you're also learning Digital Forensics or Cybersecurity, feel free to explore this repository, share suggestions, or discuss investigation techniques. I'm always interested in learning from the cybersecurity community and improving my practical skills.

---

### Disclaimer

This repository was created for educational purposes. All investigations were performed on my own Windows 11 system in a controlled environment. No unauthorized systems or third-party devices were examined during this learning project.

---

⭐ Thank you for visiting this repository. Feedback, suggestions, and learning discussions are always welcome.
