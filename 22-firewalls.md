# Firewalls

> **Estimated Reading Time:** 10–15 minutes  
> **Difficulty:** Beginner  
> **Prerequisites:** Routing

A firewall is a network security device or software application that monitors and filters incoming and outgoing network traffic based on predefined security rules.

Firewalls are one of the most important security controls in modern networks. They help prevent unauthorized access while allowing legitimate communication to continue.

---

# What You'll Learn

- What a firewall is
- Why firewalls exist
- Stateful vs Stateless firewalls
- Inbound and outbound filtering
- How firewalls improve security

---

# Why It Matters

Imagine a security guard standing at the entrance of a building.

Every visitor is checked before entering.

Some visitors are allowed inside.

Others are turned away.

A firewall performs the same function for network traffic by deciding which connections should be allowed or denied.

---

# Core Concepts

A firewall examines network traffic and compares it against a set of security rules.

Common decisions include:

- Allow
- Deny
- Log
- Inspect

Modern firewalls often inspect:

- Source IP address
- Destination IP address
- Port numbers
- Protocols
- Connection state

Some advanced firewalls also inspect application-layer traffic.

---

# How It Works

A device sends a packet.

↓

The packet reaches the firewall.

↓

The firewall compares the packet against its rules.

↓

If permitted, the packet continues.

↓

If denied, the packet is dropped.

↓

The firewall may record the event in a log for administrators to review.

---

# Diagram

```text
Internet

↓

Firewall

↓

Allow / Deny

↓

Internal Network
```

---

# Types of Firewalls

| Type | Description |
|--------|-------------|
| Packet Filtering | Filters packets using basic rules. |
| Stateful Firewall | Tracks active network connections. |
| Next-Generation Firewall (NGFW) | Inspects applications, users and threats. |
| Host-Based Firewall | Runs directly on a computer. |

---

# Real-World Example

A company hosts a public website.

The firewall allows:

- HTTPS (443)
- SSH (22) for administrators

All other unsolicited inbound traffic is blocked.

This significantly reduces the organization's attack surface.

---

# Cybersecurity Context

Firewalls play a critical role in:

- Network segmentation
- Access control
- Threat prevention
- Incident response
- Defense-in-depth strategies

Although firewalls cannot stop every attack, they are one of the first layers protecting enterprise networks.

---

# Common Mistakes

| Mistake | Explanation |
|----------|-------------|
| Firewalls stop every cyber attack | They reduce risk but cannot stop attacks exploiting allowed services. |
| A firewall replaces antivirus software | Firewalls and endpoint protection serve different purposes. |
| Firewalls only protect large organizations | Home routers also contain firewall functionality. |

---

# Interview Questions

- What is a firewall?
- What is the difference between stateful and stateless firewalls?
- What information does a firewall inspect?
- Why are firewalls important?
- Can a firewall replace antivirus software?

---

# Summary

Firewalls enforce security policies by allowing or blocking network traffic based on predefined rules. They are a fundamental component of modern network security.

---

# Related Chapters

- Routing
- HTTPS
- IDS & IPS
- VPNs
