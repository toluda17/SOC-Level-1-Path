# SOC Level 1 – Section 3: Endpoint Security Monitoring

Completed: June 2025  
Platform: [TryHackMe SOC Level 1 Path](https://tryhackme.com/path/outline/soc-level1)

---

## Overview

This section focused on tools and techniques used to monitor endpoints for signs of compromise, unauthorized changes, or malicious activity. Endpoint security monitoring is critical for SOC analysts because it bridges the gap between alerts and real evidence of attacker actions on individual systems.

Through practical labs, I learned how various tools collect and analyze endpoint data, how to interpret event logs, and how to pivot between different tools to gain a comprehensive view of endpoint activity.

---
## Tools and Resources Used

- **Windows Event Viewer** – Navigating and filtering native Windows event logs
- **Sysinternals Suite** – Tools like Process Explorer, Autoruns, and TCPView for examining live system activity
- **Sysmon (System Monitor)** – Configuring and interpreting logs for process creation, network connections, and more
- **osquery** – Querying endpoint state using SQL-like syntax
- **Wazuh** – Centralized log collection, monitoring, and alerting
- **TryHackMe Labs**, covering:
  - Event log analysis
  - Suspicious process tracking
  - Sysmon log creation and interpretation
  - Threat detection using osquery and Wazuh dashboards
- Microsoft official documentation and community Sysmon config resources

---
## Key Concepts and Takeaways

- **Windows Event Viewer** provides valuable logs such as process creations, logon events, and security policy changes, essential for both proactive hunting and reactive investigations.
- The **Sysinternals Suite** offers powerful utilities for real-time system investigation, letting analysts quickly identify suspicious processes, startup items, and network activity.
- **Sysmon** extends Windows logging capabilities, capturing granular details like command-line arguments, file creation, and network connections. Proper configuration is critical to balance detail with noise.
- **osquery** allows security teams to query endpoints as if they were databases, pulling live information on processes, users, network connections, and file integrity.
- **Wazuh** serves as both a SIEM and host-based intrusion detection system, correlating logs, generating alerts, and centralizing data for analysis across multiple endpoints.
- Understanding baseline normal activity is critical before identifying anomalies on endpoints.

---
## Lessons Learned and Real-World Reflections

Before this section, I mostly thought about security in terms of network traffic and external threats. This module showed me how much evidence lives inside the endpoints themselves, and how attackers often rely on blending into normal processes to avoid detection.

Sysinternals tools opened my eyes to how quickly an analyst can spot anomalies on a live system, like unknown startup programs or suspicious network connections. Sysmon felt like a huge force multiplier; it captures details that native logs miss, but also requires careful tuning to avoid overwhelming analysts with noise.

osquery was fascinating because it bridges IT operations and security. It made me realize how flexible endpoint visibility can be when it’s driven by targeted queries instead of just waiting for logs.

Wazuh tied everything together for me. It’s one thing to collect logs, but another to centralize them, correlate across multiple machines, and generate actionable alerts. It’s easy to see how Wazuh would be essential for scaling security monitoring in real environments.

This section gave me a new respect for endpoint visibility and taught me that effective SOC work isn’t just about reacting to alerts—it’s about proactively knowing what normal looks like and spotting deviations early.

---
