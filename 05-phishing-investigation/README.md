# SOC Level 1 – Section 5: Phishing Investigation

Completed: July 2025  
Platform: [TryHackMe SOC Level 1 Path](https://tryhackme.com/path/outline/soc-level1)

---

## Overview

This section focused on one of the most common initial attack vectors faced by SOC analysts: phishing. Through hands-on labs, I learned how to analyze suspicious emails, investigate attachments, extract indicators of compromise (IOCs), and spot subtle signs that distinguish phishing attempts from legitimate messages.

This module connected technical skills with critical thinking, highlighting how a seemingly ordinary email can be the starting point for significant security incidents.

---
## Tools and Resources Used

- Email clients and webmail interfaces for examining message headers
- **Message source view** in email clients to analyze:
  - Headers
  - MIME boundaries
  - Hidden metadata
- Online tools and sandboxes:
  - [VirusTotal](https://www.virustotal.com/)
  - [Any.Run](https://any.run/)
  - [Hybrid Analysis](https://www.hybrid-analysis.com/)
  - [URLScan.io](https://urlscan.io/)
- Manual inspection techniques for:
  - Suspicious links and redirects
  - Macros in attachments
  - Encoded payloads
- TryHackMe labs covering:
  - Email header analysis
  - Phishing scenario investigations
  - Malicious attachment review

---
## Key Concepts and Takeaways

- Phishing emails are often well-crafted and appear legitimate at first glance, making header analysis and attention to detail essential.
- **Message source code** reveals hidden information:
  - Return paths
  - Reply-to discrepancies
  - Received headers tracing email origins
- Indicators like mismatched sender names, suspicious domains, and poorly formed links are reliable red flags.
- Online sandboxes help safely analyze malicious attachments and URLs without risking local systems.
- Phishing investigations require both technical skill and intuition, combining evidence from headers, content, and external tools.
- Documentation is crucial: SOC analysts must clearly record findings and provide actionable intelligence for mitigation.

---
## Lessons Learned and Real-World Reflections

Working through these labs was relatively easy in comparison to the others. I saw how attackers disguise malicious emails to look genuine and how subtle clues in headers and metadata can expose the truth. It’s easy to assume phishing is obvious, but these labs showed me how convincing some emails can be.

Reading emails in source code format felt strange at first, but it quickly became clear why it’s so important. Small details like a misspelled domain, unusual return paths, or suspicious IP addresses can completely change the outcome of an investigation.

Using tools like VirusTotal and Hybrid Analysis gave me confidence that I can safely analyze suspicious attachments and links without risking my own system. It also taught me how to collect hashes, file behavior reports, and other IOCs to feed back into detection rules.

This section made me realize that phishing isn’t just an IT problem—it’s one of the biggest threats SOC analysts deal with. Knowing how to break down an email and find hidden clues is a core skill I’m excited to keep building.

---
