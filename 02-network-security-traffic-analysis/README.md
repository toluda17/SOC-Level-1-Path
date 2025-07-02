# SOC Level 1 – Section 2: Network Security and Traffic Analysis

Completed: June 2025  
Platform: [TryHackMe SOC Level 1 Path](https://tryhackme.com/path/outline/soc-level1)

---

## Overview

This section focused on the fundamental tools, techniques, and concepts used in network security and traffic analysis. It introduced practical skills that SOC analysts rely on daily to detect malicious activity, investigate incidents, and identify anomalies within network traffic.

Through hands-on labs, I learned how to capture, analyze, and interpret packet data, as well as how to leverage various open-source tools to examine traffic for signs of compromise. This section strengthened my ability to look beyond basic alerts and understand what’s happening at the packet level in a network.

---
## Tools and Resources Used

- **Wireshark** – Deep packet inspection and protocol analysis
- **TShark** – Command-line version of Wireshark for automated analysis
- **Snort** – Network intrusion detection and rule-based alerting
- **Zeek (formerly Bro)** – Network security monitoring and logging at scale
- **NetworkMiner** – Passive network forensic analysis and artifact extraction
- TryHackMe labs covering:
  - Packet capture analysis
  - Signature-based detection
  - Traffic fingerprinting
  - Protocol dissection
- Example PCAP files for lab analysis
- Personal notes and protocol cheat sheets
  
---

## Key Concepts and Takeaways

- Network security monitoring involves capturing traffic and looking for indicators that might signal an attack, data exfiltration, or policy violations.
- **Wireshark** is a powerful tool for dissecting packets, inspecting protocols, and filtering specific conversations or anomalies.
- **TShark** allows similar analysis to Wireshark but is suited for scripting, automation, and large-scale PCAP processing.
- **Snort** uses rule-based detection to identify suspicious patterns in network traffic and can be deployed inline or in passive mode.
- **Zeek** provides high-level logs and extracts metadata from network traffic, enabling faster analysis without having to review every single packet.
- **NetworkMiner** can extract files, credentials, and other artifacts from network captures, assisting in forensic investigations.
- Understanding normal network behavior is crucial for identifying anomalies that could indicate malicious activity.

---
## Lessons Learned and Real-World Reflections

Before this section, I knew the names of these tools but had never truly used them in a practical way. Working through these labs showed me how powerful they are, and also how different their use cases can be.

Wireshark helped me see traffic down to the byte level, which made protocols like DNS, HTTP, and TLS feel far less abstract. TShark gave me a glimpse into how large-scale environments might automate analysis rather than manually opening large captures.

Learning Snort rules was eye-opening because it highlighted how precise detection logic needs to be to avoid false positives while still catching threats. Zeek changed how I think about network monitoring altogether; it feels like a bridge between raw packet data and higher-level security analysis, providing logs that SOC analysts can quickly pivot on.

I also realized that tools like NetworkMiner can reveal artifacts I didn’t expect, like images, documents, or credential data embedded in traffic—which connects directly to real-world forensic work.

Overall, this module gave me confidence that I can begin analyzing network captures, write basic detection logic, and think more critically about what network traffic reveals during investigations.
