# NAT & PAT

> **Estimated Reading Time:** 10–15 minutes  
> **Difficulty:** Beginner  
> **Prerequisites:** DHCP

Network Address Translation (NAT) allows devices using private IP addresses to communicate with public networks such as the Internet. Port Address Translation (PAT) extends NAT by allowing multiple devices to share a single public IP address.

Without NAT and PAT, the limited number of available IPv4 addresses would not be sufficient for today's Internet.

---

# What You'll Learn

- What NAT is
- What PAT is
- Public vs Private IP addresses
- Why NAT exists
- Advantages and limitations of NAT

---

# Why It Matters

Imagine every phone, laptop, smart TV and gaming console in your home required its own unique public IP address.

Internet Service Providers would quickly run out of IPv4 addresses.

NAT solves this problem by allowing many private devices to share a single public IP address.

---

# Core Concepts

Private IP addresses are used inside local networks.

Examples include:

```text
192.168.x.x

10.x.x.x

172.16.x.x – 172.31.x.x
```

These addresses cannot communicate directly across the Internet.

Instead, a router performs **Network Address Translation (NAT)**.

PAT (Port Address Translation) allows multiple devices to use the same public IP address by tracking connections using port numbers.

---

# How It Works

Your laptop sends a packet.

↓

Source IP:

```text
192.168.1.20
```

↓

The home router replaces the private address with its public IP.

↓

The packet travels across the Internet.

↓

The destination replies to the router.

↓

The router translates the destination back to your laptop using PAT.

To the Internet, every device in your home appears to use the same public IP address.

---

# Diagram

```text
Laptop

↓

192.168.1.20

↓

Home Router

(NAT / PAT)

↓

Public IP

↓

Internet
```

---

# Real-World Example

A family has:

- Two laptops
- Three phones
- A gaming console
- A smart TV

Although every device has a different private IP address, they all access the Internet using the home's single public IP address.

This is one of the most common uses of NAT and PAT.

---

# Cybersecurity Context

NAT hides internal IP addresses from external networks, making it more difficult for attackers to directly identify internal systems.

However, NAT should **never** be considered a replacement for a firewall.

Firewalls enforce security policies.

NAT simply translates addresses.

---

# Common Mistakes

| Mistake | Explanation |
|----------|-------------|
| NAT is a firewall | NAT performs address translation, not security filtering. |
| Private IP addresses work across the Internet | They must first be translated into public addresses. |
| NAT and PAT are identical | PAT uses port numbers to allow multiple devices to share one public IP. |

---

# Interview Questions

- Why was NAT created?
- What is the difference between NAT and PAT?
- Why are private IP addresses used?
- Does NAT improve security?
- Why is PAT important?

---

# Summary

NAT allows private networks to communicate with public networks by translating IP addresses. PAT extends this concept by allowing many devices to share a single public IPv4 address.

---

# Related Chapters

- IPv4 Addressing
- Routing
- DHCP
- Firewalls
