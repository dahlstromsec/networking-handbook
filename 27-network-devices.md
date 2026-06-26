# Network Devices

> **Estimated Reading Time:** 10–15 minutes  
> **Difficulty:** Beginner  
> **Prerequisites:** Routing, Switching

Computer networks are built using a variety of devices, each designed to perform a specific task. Some devices connect computers together, others forward traffic between networks, while others provide wireless access or protect the network from threats.

Understanding the purpose of each device makes it much easier to understand how networks are designed and how data travels from one device to another.

---

# What You'll Learn

- The purpose of common network devices
- How each device contributes to a network
- Where devices are typically deployed
- How networking devices work together
- Why these devices are important in cybersecurity

---

# Why It Matters

Imagine trying to build a road system without knowing the difference between a road, a bridge and a traffic light.

Although all are involved in transportation, each performs a different job.

Networking devices work the same way.

A switch, router and firewall may all handle network traffic, but they each have a unique purpose.

---

# Core Concepts

Modern networks are built using several common devices.

| Device | Primary Purpose |
|---------|-----------------|
| Switch | Connects devices within the same Local Area Network (LAN). |
| Router | Connects different networks together. |
| Firewall | Filters and protects network traffic. |
| Access Point | Provides wireless network access. |
| Modem | Connects a local network to an Internet Service Provider (ISP). |
| Hub | Broadcasts traffic to every connected device (largely obsolete). |

Each device performs one specialized function that contributes to the overall network.

---

# How It Works

Imagine a user opens a website.

```text
Laptop

↓

Access Point

↓

Switch

↓

Firewall

↓

Router

↓

Modem

↓

Internet

↓

Web Server
```

Every device along the path performs a different task before the request reaches the destination.

---

# Device Overview

## Switch

A switch connects devices on the same Local Area Network.

It forwards Ethernet frames using **MAC addresses**, allowing devices to communicate efficiently without sending traffic to every connected device.

Common examples:

- Office networks
- Schools
- Data centers

---

## Router

A router connects different networks together.

It examines **IP addresses** and forwards packets toward their destination using routing tables.

Common examples:

- Home routers
- Enterprise routers
- Internet Service Provider (ISP) infrastructure

---

## Firewall

A firewall examines network traffic and decides whether it should be allowed or blocked based on security rules.

Firewalls are commonly placed between trusted internal networks and untrusted external networks.

---

## Access Point (AP)

An Access Point provides wireless connectivity.

Instead of using Ethernet cables, devices communicate using Wi-Fi while still becoming part of the local network.

Most home Wi-Fi routers contain both a switch and an Access Point.

---

## Modem

A modem connects your local network to your Internet Service Provider.

Depending on the connection type, it converts signals between your home network and technologies such as:

- Cable
- DSL
- Fiber

Without a modem, most home networks would not have Internet access.

---

## Hub

A hub is an older networking device that broadcasts incoming traffic to every connected device.

Unlike switches, hubs do not learn MAC addresses.

Because of poor performance and security, hubs have almost entirely been replaced by switches.

---

# Real-World Example

A small business network might contain:

- One modem connected to the ISP.
- One firewall protecting the internal network.
- One router managing traffic between networks.
- Several switches connecting office computers.
- Multiple wireless Access Points providing Wi-Fi.

Although users simply connect to the Internet, many different devices work together behind the scenes.

---

# Cybersecurity Context

Networking devices play a major role in cybersecurity.

Examples include:

- Firewalls filtering malicious traffic.
- Routers controlling communication between networks.
- Switches supporting VLANs and network segmentation.
- Access Points securing wireless communication.
- Packet captures collected from switches or firewalls during investigations.

Understanding where each device sits within the network helps analysts troubleshoot incidents and investigate attacks.

---

# Common Mistakes

| Mistake | Explanation |
|----------|-------------|
| A switch and router perform the same job | Switches connect devices on the same network. Routers connect different networks. |
| A modem provides Wi-Fi | Wi-Fi is normally provided by an Access Point or wireless router. |
| Hubs and switches are identical | Switches intelligently forward traffic, while hubs broadcast everything. |
| Firewalls route Internet traffic | Firewalls primarily enforce security policies rather than route packets. |

---

# Interview Questions

- What is the difference between a switch and a router?
- What does a firewall do?
- What is the purpose of an Access Point?
- Why have hubs largely disappeared?
- Which device connects your home network to your ISP?

---

# Summary

Modern networks rely on several specialized devices working together. Understanding the role of switches, routers, firewalls, access points, modems and hubs provides a strong foundation for both networking and cybersecurity.

---

# Related Chapters

- Switching
- Routing
- Firewalls
- VLANs
- Wireshark & Network Troubleshooting
