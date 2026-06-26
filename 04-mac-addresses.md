# MAC Addresses

> **Estimated Reading Time:** 10–15 minutes  
> **Difficulty:** Beginner  
> **Prerequisites:** Ethernet

Every device connected to a network has a unique hardware address known as a **Media Access Control (MAC) address**. Unlike an IP address, which can change depending on the network, a MAC address identifies a network interface on the local network.

Whenever devices communicate using Ethernet, MAC addresses are used to ensure data reaches the correct destination.

---

# What You'll Learn

- What a MAC address is
- MAC address format
- MAC vs IP addresses
- How switches use MAC addresses
- Why MAC addresses are important

---

# Why It Matters

Imagine sending a package to a house without knowing the street address.

The package would never arrive.

The same idea applies to Ethernet networks.

IP addresses identify devices across different networks, while MAC addresses identify devices on the local network.

Without MAC addresses, Ethernet communication would not be possible.

---

# Core Concepts

A MAC address is a **48-bit hardware address** assigned to a network interface.

Example:

```text
00:1A:2B:3C:4D:5E
```

The first half identifies the manufacturer.

The second half uniquely identifies the device.

Unlike IP addresses, MAC addresses normally remain the same regardless of which network the device connects to.

---

# How It Works

Imagine Computer A wants to communicate with Computer B.

Computer A already knows Computer B's IP address.

↓

ARP is used to discover Computer B's MAC address.

↓

Computer A creates an Ethernet frame using Computer B's MAC address.

↓

The switch reads the destination MAC address.

↓

The frame is forwarded to the correct device.

Without MAC addresses, the switch would have no way of knowing where to send the frame.

---

# Diagram

```text
Computer A

↓

MAC Address

↓

Switch

↓

MAC Address

↓

Computer B
```

---

# Real-World Example

Your laptop connects to a switch in an office.

Although dozens of computers share the same switch, each device has a unique MAC address.

The switch learns these addresses and forwards frames only to the correct destination instead of sending them to every device.

---

# Cybersecurity Context

MAC addresses appear frequently during:

- Packet analysis
- ARP investigations
- Network troubleshooting
- MAC spoofing attacks
- Switch security configuration

Security analysts often examine MAC addresses when investigating devices connected to a local network.

---

# Common Mistakes

| Mistake | Explanation |
|----------|-------------|
| MAC addresses are the same as IP addresses | MAC addresses identify devices locally, while IP addresses identify devices across networks. |
| MAC addresses are used on the Internet | Routers forward packets using IP addresses, not MAC addresses. |
| MAC addresses never change | They normally remain fixed but can be spoofed or changed in software. |

---

# Interview Questions

- What is a MAC address?
- Which OSI layer uses MAC addresses?
- What is the difference between a MAC address and an IP address?
- Why are MAC addresses important for Ethernet communication?

---

# Summary

MAC addresses uniquely identify devices on a local network. Ethernet switches use MAC addresses to forward frames efficiently between connected devices.

---

# Related Chapters

- Ethernet
- ARP
- Switching
