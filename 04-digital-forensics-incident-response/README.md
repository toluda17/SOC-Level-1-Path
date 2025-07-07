# SOC Level 1 – Section 4: Digital Forensics and Incident Response (DFIR)

Completed: July 2025  
Platform: [TryHackMe SOC Level 1 Path](https://tryhackme.com/path/outline/soc-level1)

---

## Overview

This section provided a hands-on introduction to Digital Forensics and Incident Response (DFIR), covering practical techniques and tools used to investigate security incidents on both Windows and Linux systems.

Through a series of labs, I learned how to collect forensic artifacts, analyze live systems and memory dumps, and manage investigations using structured workflows and collaboration tools. This module connected everything I’ve learned so far—from log analysis to attacker techniques—into the bigger picture of responding to real-world incidents.

---
## Tools and Resources Used

- **Autopsy** – Graphical digital forensics tool for analyzing disk images and file systems
- **KAPE (Kroll Artifact Parser and Extractor)** – Rapid collection and processing of forensic artifacts from Windows systems
- **Redline** – Host-based analysis of memory and system activity snapshots
- **Volatility** – Memory forensics framework for analyzing memory dumps and detecting malicious processes
- **Velociraptor** – Endpoint visibility, live response, and artifact collection at scale
- **TheHive Project** – Incident response and case management platform
- **TryHackMe Labs**, including:
  - Windows Forensics 1 & 2
  - Linux Forensics
  - Disk image analysis
  - Memory forensics
  - Basic malware analysis
  - DFIR case management exercises
- Community resources and official documentation for each tool

---
# Key Concepts and Takeaways

- **Windows Forensics** involves examining artifacts like event logs, registry hives, prefetch files, browser history, and link files to reconstruct user and attacker activity.
- **Linux Forensics** relies heavily on log files, file system metadata, shell history, and artifacts in /var and /etc directories.
- **Memory forensics** is essential for detecting fileless malware, hidden processes, and volatile data that may never be written to disk.
- Tools like **Volatility** and **Redline** make it possible to extract evidence from memory dumps, such as suspicious processes, open network connections, and injected code regions.
- **Autopsy** and similar tools simplify disk image analysis by parsing file systems, recovering deleted files, and identifying user activity.
- **KAPE** significantly speeds up artifact collection, allowing focused triage on key evidence paths instead of pulling entire disk images.
- **Velociraptor** demonstrates how enterprise-scale live response is performed, providing flexibility and speed for rapid incident scoping.
- **TheHive Project** shows how professional teams manage investigations, track tasks, and collaborate during complex incidents.
- Even basic malware analysis—looking at file hashes, PE headers, and strings—can reveal useful indicators for detection or further investigation.

---
## Lessons Learned and Real-World Reflections

Working through this labs was an eye-opener. I finally saw how the tools fit together and how much you can uncover on a system if you know where to look. It made forensics feel a lot less mysterious and way more practical
Windows Forensics was eye-opening. I learned how prefetch files, registry keys, and link files reveal the true timeline of user and attacker activity. Linux Forensics taught me how critical logs and file metadata are for reconstructing events.

Memory forensics stood out as one of the most powerful skills. Tools like Volatility and Redline made me realize how much evidence lives in memory—like injected malicious code, suspicious network connections, and processes that never touch disk.

I also discovered how valuable it is to have automated triage tools like KAPE for quickly gathering the right artifacts. Velociraptor took this further, showing how live response can scale across many endpoints.

Finally, learning about TheHive highlighted that forensics isn’t just technical—it’s also about process, documentation, and teamwork. Investigations require collaboration, reporting, and structured workflows.

This section reinforced the idea that incident response is more than reacting to alerts—it’s about digging into systems, understanding how attacks unfold, and finding truth in the data. I’m excited to keep exploring memory analysis, malware reverse engineering, and incident handling as I progress.

---
