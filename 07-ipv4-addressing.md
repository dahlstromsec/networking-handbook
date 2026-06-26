# IPv4 Addressing

> **Estimated Reading Time:** 10–15 minutes  
> **Difficulty:** Beginner  
> **Prerequisites:** VLANs

Every device connected to an IP network requires an Internet Protocol (IP) address. An IPv4 address uniquely identifies a device and allows routers to determine where packets should be delivered.

IPv4 remains the most widely used addressing system in modern networks, although it is gradually being complemented by IPv6.

---

# What You'll Learn

- What an IPv4 address is
- Public and private IP addresses
- Network and host portions
- Special IPv4 addresses
- Why IP addressing is important

---

# Why It Matters

Imagine trying to mail a letter without writing an address on the envelope.

No one would know where it should be delivered.

IPv4 addresses solve the same problem for computer networks by uniquely identifying devices and allowing routers to forward packets correctly.

---

# Core Concepts

An IPv4 address is a **32-bit logical address** written as four decimal numbers separated by periods.

Example:

```text
192.168.1.25
```

Every IPv4 address consists of two parts:

- **Network Portion** – Identifies the network.
- **Host Portion** – Identifies a specific device.

Common private IPv4 ranges include:

| Range | CIDR |
|--------|------|
| 10.0.0.0 – 10.255.255.255 | /8 |
| 172.16.0.0 – 172.31.255.255 | /12 |
| 192.168.0.0 – 192.168.255.255 | /16 |

Private addresses are used inside local networks and are not directly routable across the Internet.

---

# How It Works

Your computer wants to visit a website.

↓

It creates a packet using its own IP address as the source.

↓

The destination website's IP address is added to the packet.

↓

The packet is sent to the default gateway.

↓

Routers examine the destination IP address and forward the packet until it reaches the correct network.

Every router along the path repeats this process.

---

# Diagram

```text
PC

192.168.1.25

↓

Router

↓

Internet

↓

203.0.113.10

Web Server
```

---

# Real-World Example

Your home router assigns private IPv4 addresses to your laptop, phone and smart TV.

Although each device has its own private IP address, the router uses Network Address Translation (NAT) to allow all devices to share a single public IP address when accessing the Internet.

---

# Cybersecurity Context

IPv4 addresses appear throughout cybersecurity.

Security professionals use them to:

- Investigate suspicious traffic.
- Configure firewall rules.
- Analyze logs.
- Perform network scans.
- Identify affected systems during incidents.

Understanding IP addressing is one of the most fundamental networking skills.

---

# Common Mistakes

| Mistake | Explanation |
|----------|-------------|
| IP addresses never change | Many devices receive dynamic addresses from DHCP. |
| Private IP addresses work across the Internet | Private addresses require NAT to communicate externally. |
| MAC addresses and IP addresses are the same | MAC addresses identify devices locally, while IP addresses identify devices across networks. |

---

# Interview Questions

- What is an IPv4 address?
- What is the difference between public and private IP addresses?
- What are the two parts of an IPv4 address?
- Why are routers dependent on IP addresses?

---

# Summary

IPv4 addressing provides the logical addressing system used to identify devices and route packets across networks. Understanding IP addressing is essential before learning subnetting and routing.

---

# Related Chapters

- Subnetting
- Routing
- NAT & PAT
- ARP
