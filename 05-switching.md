# Switching

> **Estimated Reading Time:** 10–15 minutes  
> **Difficulty:** Beginner  
> **Prerequisites:** MAC Addresses

A network switch connects devices within a Local Area Network (LAN) and forwards Ethernet frames to the correct destination. Modern switches make communication faster and more efficient by learning where devices are connected.

Without switches, today's business and home networks would be far less efficient.

---

# What You'll Learn

- What a switch is
- How switches forward traffic
- MAC address tables
- Broadcast and unicast traffic
- Why switches improve network performance

---

# Why It Matters

Imagine a classroom where every student shouts every message to everyone.

Communication would quickly become chaotic.

A switch avoids this problem by sending traffic only to the device that should receive it.

This reduces unnecessary network traffic and improves performance.

---

# Core Concepts

A switch operates at **Layer 2 (Data Link)** of the OSI Model.

Its primary job is to forward Ethernet frames using **MAC addresses**.

As frames pass through the switch, it builds a **MAC Address Table** that maps MAC addresses to physical switch ports.

Once the destination is known, the frame is sent only to that port.

---

# How It Works

Computer A sends a frame.

↓

The switch reads the source MAC address.

↓

The switch learns which port that MAC address is connected to.

↓

The switch checks the destination MAC address.

↓

If the destination is known, the frame is forwarded to the correct port.

↓

If unknown, the switch temporarily broadcasts the frame until the destination responds.

Over time, the switch learns where every connected device is located.

---

# Diagram

```text
Computer

↓

Switch

↓

MAC Address Table

↓

Correct Port

↓

Destination Device
```

---

# Real-World Example

A company has fifty computers connected to a single switch.

When one employee accesses a file server, the switch forwards the traffic only to the server instead of every computer on the network.

This keeps the network fast and efficient.

---

# Cybersecurity Context

Understanding switch behavior helps explain:

- MAC flooding attacks
- VLAN implementation
- Port security
- Packet forwarding
- Local network investigations

Switches are one of the most important devices in enterprise networks.

---

# Common Mistakes

| Mistake | Explanation |
|----------|-------------|
| Switches use IP addresses | Switches forward frames using MAC addresses. |
| Switches and routers perform the same job | Switches connect devices within a LAN, while routers connect different networks. |
| Switches always broadcast traffic | Modern switches normally send frames only to the intended destination. |

---

# Interview Questions

- What is the purpose of a network switch?
- Which OSI layer does a switch operate on?
- What is a MAC Address Table?
- How does a switch learn where devices are connected?

---

# Summary

Switches improve network efficiency by forwarding Ethernet frames only to their intended destination using MAC addresses.

---

# Related Chapters

- Ethernet
- VLANs
- Routing
- ARP
