# ARP

> Estimated Reading Time: 8–10 minutes
> Difficulty: Beginner
> Prerequisites: Routing

## Introduction

Address Resolution Protocol (ARP) maps IPv4 addresses to MAC addresses on a local network.

---

## What You'll Learn

- Why ARP exists
- ARP Requests and Replies
- ARP Cache
- ARP Spoofing

---

## Why It Matters

Devices know destination IP addresses, but Ethernet communication requires destination MAC addresses.

---

## Main Concept

Need MAC Address

↓

Broadcast ARP Request

↓

Target Replies

↓

Store in ARP Cache

↓

Send Ethernet Frame

---

## Useful Commands

```bash
arp -a
ip neigh
```

---

## Cybersecurity Context

ARP spoofing can redirect traffic and enable man-in-the-middle attacks on local networks.

---

## Interview Questions

- Why is ARP necessary?
- What information does ARP resolve?
- What is ARP spoofing?

---

## Summary

ARP bridges Layer 3 (IP) and Layer 2 (Ethernet) communication.

---

## Related Chapters

- MAC Addresses
- Ethernet
- IPv4 Addressing
