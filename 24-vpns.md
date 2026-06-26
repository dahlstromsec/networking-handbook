# VPNs (Virtual Private Networks)

> **Estimated Reading Time:** 10–15 minutes  
> **Difficulty:** Beginner  
> **Prerequisites:** HTTPS

A Virtual Private Network (VPN) creates an encrypted connection between devices across an untrusted network such as the Internet. Instead of sending data in plaintext, a VPN protects communication by creating a secure tunnel between two endpoints.

VPNs are widely used by businesses to provide secure remote access and by individuals to protect data when using public networks.

---

# What You'll Learn

- What a VPN is
- Why VPNs exist
- Remote Access vs Site-to-Site VPNs
- VPN tunnels
- Common business use cases

---

# Why It Matters

Imagine sending confidential documents through the mail.

Instead of mailing them openly, you place them inside a locked container that only the recipient can open.

A VPN works in a similar way by encrypting network traffic before it travels across the Internet.

Even if someone intercepts the traffic, they cannot easily read its contents.

---

# Core Concepts

A VPN creates an encrypted tunnel between two devices or networks.

Common VPN types include:

| Type | Purpose |
|--------|---------------------------|
| Remote Access VPN | Connects individual users to a company network. |
| Site-to-Site VPN | Connects two separate networks together. |

VPNs provide:

- Encryption
- Authentication
- Secure remote access
- Data confidentiality

A VPN protects data while it is travelling across untrusted networks.

---

# How It Works

An employee works from home.

↓

The employee opens the VPN client.

↓

The VPN authenticates the user.

↓

An encrypted tunnel is established.

↓

The employee securely accesses company resources.

To anyone observing the traffic, the data appears encrypted and unreadable.

---

# Diagram

```text
Remote User

↓

VPN Client

↓

Encrypted Tunnel

↓

Company Firewall

↓

Internal Network
```

---

# Real-World Example

An employee working from home needs access to internal company file servers.

Instead of exposing those servers directly to the Internet, the employee first connects to the company VPN.

Once authenticated, the employee can securely access internal resources as though they were physically in the office.

---

# Cybersecurity Context

VPNs are widely used for:

- Secure remote work
- Site-to-site office connectivity
- Secure administration
- Protecting traffic on public Wi-Fi

Modern organizations often combine VPNs with Multi-Factor Authentication (MFA) to strengthen security.

---

# Common Mistakes

| Mistake | Explanation |
|----------|-------------|
| VPNs make users anonymous | VPNs encrypt traffic but do not guarantee anonymity. |
| VPNs replace HTTPS | HTTPS and VPNs protect different parts of the communication process. |
| VPNs eliminate all cyber threats | VPNs secure communication but cannot prevent malware or phishing attacks. |

---

# Interview Questions

- What is a VPN?
- What is the difference between a Remote Access VPN and a Site-to-Site VPN?
- Why are VPNs important?
- What does a VPN encrypt?
- Does a VPN replace HTTPS?

---

# Summary

VPNs provide encrypted communication across untrusted networks, allowing users and organizations to securely access resources while protecting sensitive data in transit.

---

# Related Chapters

- HTTPS
- Firewalls
- SSH
- Routing
