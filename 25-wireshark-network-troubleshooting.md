# Wireshark & Network Troubleshooting

> **Estimated Reading Time:** 12–15 minutes  
> **Difficulty:** Beginner  
> **Prerequisites:** ICMP

Wireshark is one of the world's most widely used network protocol analyzers. It allows administrators and cybersecurity professionals to capture, inspect and analyze network traffic in real time.

When combined with a structured troubleshooting process, Wireshark becomes an invaluable tool for identifying connectivity issues, performance problems and suspicious activity.

---

# What You'll Learn

- What Wireshark is
- Basic packet captures
- Display filters
- A structured troubleshooting process
- Why packet analysis is important

---

# Why It Matters

Imagine trying to repair a car without being able to see the engine.

You would only be guessing what was wrong.

Wireshark removes the guesswork from networking by allowing you to see exactly what devices are sending and receiving.

Instead of assuming what happened, you can inspect the packets directly.

---

# Core Concepts

A packet capture records network traffic exactly as it travels across the network.

Wireshark allows you to examine:

- Source IP addresses
- Destination IP addresses
- MAC addresses
- Protocols
- TCP conversations
- DNS lookups
- HTTP requests
- TLS handshakes

Every captured packet becomes evidence that can be analyzed.

---

# How It Works

A packet capture begins.

↓

Devices exchange network traffic.

↓

Wireshark records every packet.

↓

The analyst applies display filters.

↓

Individual conversations are examined.

↓

The root cause of the problem is identified.

Instead of guessing why communication failed, the packets provide the answer.

---

# Diagram

```text
Network Traffic

↓

Packet Capture

↓

Wireshark

↓

Filtering

↓

Analysis

↓

Troubleshooting
```

---

# Useful Commands

```bash
ping 8.8.8.8
```

Verify basic connectivity.

```bash
traceroute example.com
```

Trace the network path.

```bash
ip a
```

Display network configuration.

```bash
ip r
```

Display the routing table.

```bash
ss -tulpn
```

Display listening ports and active connections.

```bash
nslookup example.com
```

Verify DNS resolution.

---

# Useful Wireshark Filters

```text
dns

http

icmp

tcp.port == 443

ip.addr == 192.168.1.10
```

Learning a few filters dramatically improves packet analysis.

---

# Structured Troubleshooting Process

A good troubleshooter works methodically.

1. Verify physical connectivity.
2. Check IP configuration.
3. Test connectivity using `ping`.
4. Verify DNS resolution.
5. Inspect routing information.
6. Capture packets with Wireshark.
7. Analyze the results.

Avoid jumping directly to packet captures before checking the basics.

---

# Real-World Example

A user reports that a website will not load.

The administrator:

- Confirms the network cable is connected.
- Checks the assigned IP address.
- Uses `ping` to test connectivity.
- Verifies DNS resolution.
- Captures packets in Wireshark.

The capture reveals that DNS queries receive no response, identifying the actual cause of the problem.

---

# Cybersecurity Context

Wireshark is used daily by:

- Security Analysts
- Incident Responders
- Network Engineers
- Penetration Testers
- SOC Analysts

Packet captures help investigate malware communication, suspicious connections, phishing activity and network attacks.

Wireshark is one of the most valuable tools for anyone working in networking or cybersecurity.

---

# Common Mistakes

| Mistake | Explanation |
|----------|-------------|
| Wireshark fixes network problems | It analyzes traffic but does not repair issues. |
| More packets always mean more information | Applying filters makes analysis much easier. |
| Every problem requires Wireshark | Start with basic troubleshooting before capturing packets. |

---

# Interview Questions

- What is Wireshark used for?
- What is a packet capture?
- Why should basic troubleshooting come before packet analysis?
- What information can Wireshark display?
- Why is Wireshark important in cybersecurity?

---

# Summary

Wireshark provides visibility into network communication by capturing and analyzing packets. Combined with a structured troubleshooting process, it allows administrators and security professionals to identify problems quickly and accurately.

---

# Related Chapters

- ICMP
- DNS
- TCP
- UDP
- Firewalls
