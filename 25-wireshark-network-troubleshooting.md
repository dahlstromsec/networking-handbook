# Wireshark & Network Troubleshooting

> Estimated Reading Time: 10 minutes
> Difficulty: Beginner
> Prerequisites: ICMP

## Introduction

Wireshark is one of the most widely used packet analysis tools. Combined with a structured troubleshooting process, it helps identify connectivity issues, performance problems and suspicious traffic.

---

## What You'll Learn

- Basic packet capture
- Display filters
- Troubleshooting workflow
- Common networking tools

---

## Why It Matters

Many networking and cybersecurity problems can only be understood by examining the packets travelling across a network.

---

## Common Commands

```bash
ping 8.8.8.8
traceroute example.com
ip a
ip r
ss -tulpn
nslookup example.com
```

---

## Useful Wireshark Filters

```text
dns
http
icmp
tcp.port == 443
ip.addr == 192.168.1.10
```

---

## Suggested Workflow

1. Verify physical connectivity.
2. Check IP configuration.
3. Test connectivity with `ping`.
4. Verify DNS resolution.
5. Capture packets with Wireshark if the problem persists.

---

## Cybersecurity Context

Packet analysis is used during incident response, malware investigations, network troubleshooting and threat hunting.

---

## Interview Questions

- What is Wireshark used for?
- Why would you use `ping` before opening Wireshark?
- What is a packet capture?

---

## Summary

Successful troubleshooting follows a structured process, and Wireshark provides visibility into what is happening on the network.

---

## Related Chapters

- ICMP
- DNS
- TCP
