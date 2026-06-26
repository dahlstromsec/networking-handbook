# IDS & IPS

> **Estimated Reading Time:** 10–15 minutes  
> **Difficulty:** Beginner  
> **Prerequisites:** Firewalls

Intrusion Detection Systems (IDS) and Intrusion Prevention Systems (IPS) monitor network traffic for suspicious or malicious activity. While both technologies inspect traffic, they differ in how they respond when threats are detected.

IDS focuses on detection and alerting, whereas IPS actively blocks malicious traffic.

---

# What You'll Learn

- What IDS and IPS are
- IDS vs IPS
- Detection methods
- Where IDS and IPS are deployed
- How they improve network security

---

# Why It Matters

Imagine security cameras inside a building.

A security guard watches the cameras.

If suspicious activity is detected, the guard can either:

- Notify security personnel (IDS)

or

- Immediately stop the intruder (IPS)

IDS and IPS work in much the same way for network traffic.

---

# Core Concepts

An IDS monitors network traffic and generates alerts when suspicious activity is detected.

An IPS performs the same inspection but can also:

- Block traffic
- Reset connections
- Drop malicious packets

Detection methods commonly include:

- Signature-based detection
- Anomaly-based detection
- Behavioral analysis

---

# How It Works

Network traffic enters the network.

↓

Traffic passes through the firewall.

↓

IDS/IPS analyzes each packet.

↓

Suspicious activity is detected.

↓

IDS generates an alert.

or

↓

IPS automatically blocks the connection.

---

# Diagram

```text
Internet

↓

Firewall

↓

IDS / IPS

↓

Internal Network
```

---

# Real-World Example

An attacker attempts to exploit a vulnerable web server.

The IPS recognizes the exploit signature.

↓

The malicious packets are blocked.

↓

The administrator receives an alert describing the attempted attack.

Without the IPS, the traffic might have reached the web server.

---

# Cybersecurity Context

IDS and IPS are commonly used in:

- Security Operations Centers (SOC)
- Enterprise networks
- Data centers
- Cloud environments

Analysts regularly investigate IDS alerts while IPS systems automatically prevent many known attacks.

---

# Common Mistakes

| Mistake | Explanation |
|----------|-------------|
| IDS blocks attacks | IDS only detects and alerts. |
| IPS replaces a firewall | IPS complements—not replaces—a firewall. |
| Signature detection catches every attack | Unknown threats may require anomaly or behavioral detection. |

---

# Interview Questions

- What is the difference between IDS and IPS?
- Does an IDS block malicious traffic?
- What is signature-based detection?
- Why are IDS and IPS deployed together?
- Where are IDS and IPS commonly used?

---

# Summary

IDS detects suspicious activity and alerts administrators, while IPS actively blocks malicious traffic before it reaches protected systems. Together they provide an additional layer of network defense.

---

# Related Chapters

- Firewalls
- VPNs
- Wireshark & Network Troubleshooting
- HTTPS
