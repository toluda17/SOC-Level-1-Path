# SOC Level 1 – Section 1: Cyber Defence Frameworks

Completed: June 2025 
---

## Overview

This section provided a deep dive into the strategic frameworks that underpin defensive cybersecurity operations. These models are essential for Security Operations Center (SOC) teams, threat analysts, and incident responders in understanding adversary behavior, structuring incident detection, and building repeatable response strategies. 

By exploring these frameworks, I gained foundational knowledge that will shape how I approach threats, map attacker behavior, and contribute to blue team workflows.

---
## Frameworks Covered

### Pyramid of Pain
I learnt the concept of the Pyramid of Pain, which illustrates how the difficulty for attackers to evade detection increases as we enhance our defense mechanisms. It categorizes indicators based on how easily attackers can modify them:

 - Hashes: Simple for attackers to change. Low impact.

 - IP Addresses: Attackers can rotate them quickly. Low to moderate impact.

 - Domain Names: Easily modified. Moderate impact.

 - URLs: Slightly harder to alter, but still changeable. Moderate to high impact.

 - File Names: More challenging to modify. High impact.

 - TTPs (Tactics, Techniques, and Procedures): Most difficult to change. Very high impact.

The key takeaway is that the higher up the pyramid you go, the more difficult it becomes for attackers to adapt. By focusing on TTPs, we significantly increase the difficulty for attackers to bypass our defenses.

### Cyber Kill Chain
- This is a 7-stage model that outlines the stages of a cyberattack: Reconnaissance → Weaponization → Delivery → Exploitation → Installation → Command & Control → Actions on Objectives.
- It offers a linear view of how targeted attacks unfold, helping defenders understand where they can intervene.
- It's particularly useful for designing early detection strategies and mapping threats across different intrusion phases.

### Unified Kill Chain
- This merges the Cyber Kill Chain with MITRE ATT&CK (a framework for Adversarial Tactics, Techniques and Common Knowledge) to reflect modern, multi-stage attacker operations.
- It covers pre-exploit, exploitation, and post-compromise activity in a continuous cycle.
- It offers a more comprehensive lifecycle for understanding advanced persistent threats (APTs), including social engineering and internal movement.

### Diamond Model of Intrusion Analysis
- This is based on four interconnected vertices: Adversary, Infrastructure, Victim, and Capability.
- It promotes structured analysis by enabling analysts to pivot between these elements to discover patterns, infrastructure reuse, or similar victims.
- It encourages hypothesis generation for threat hunting and long-term adversary tracking.

---

## Tools and Resources Used

- [MITRE ATT&CK Navigator](https://attack.mitre.org/)
- [Unified Kill Chain Website](https://www.unifiedkillchain.com/)
- [NIST 800-61r2](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-61r2.pdf) – for comparing incident response models
- Flashcards and diagrams created for personal reinforcement
- Case studies and room-based labs from TryHackMe

## Key Concepts and Takeaways

- The most valuable indicators for detection are often the hardest for attackers to change (e.g., TTPs and tools).
- The traditional Kill Chain helps defenders break the attack flow at specific stages, but it is too linear for advanced persistent threats.
- The Unified Kill Chain provides a more flexible and complete representation of modern threats, especially those involving social engineering or lateral movement.
- The Diamond Model enhances analytical thinking and is particularly useful for pivoting during threat investigations.
- MITRE ATT&CK is not only a learning resource but also a working tool used by real SOC teams to build rules, investigate alerts, and guide hunts.

---

## Lessons Learned and Real-World Reflections

Going into this section, I’d heard of these frameworks but didn’t fully grasp how they’re used in real security work. Now, I see how they shape the way SOC teams think, respond, and detect threats.

The Pyramid of Pain helped me understand that good defense is about disrupting attacker behavior, not just blocking IOCs. The Kill Chain and Unified Kill Chain gave me a clearer view of how attacks unfold — and how to catch them early. The Diamond Model showed me how to break down threats from multiple angles, and MITRE ATT&CK gave me the structure to turn technical activity into actionable detection.
