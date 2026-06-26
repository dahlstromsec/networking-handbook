# Ethernet

> **Estimated Reading Time:** 10–15 minutes  
> **Difficulty:** Beginner  
> **Prerequisites:** TCP/IP Model

Ethernet is the most widely used technology for communication inside wired Local Area Networks (LANs). It defines how devices communicate on the same network using Ethernet frames and MAC addresses.

Although Wi-Fi is common today, most business networks still rely heavily on Ethernet for fast, reliable and stable communication.

---

# What You'll Learn

- What Ethernet is
- How Ethernet communication works
- Ethernet frames
- The role of MAC addresses
- Why Ethernet is important

---

# Why It Matters

Whenever two computers communicate on the same wired network, Ethernet is usually responsible for delivering the data.

Understanding Ethernet is essential before learning switches, VLANs and ARP.

---

# Core Concepts

Ethernet operates at **Layer 2 (Data Link)** of the OSI Model.

Instead of sending packets directly, Ethernet sends **frames** between devices connected to the same local network.

Every Ethernet frame contains information such as:

- Source MAC address
- Destination MAC address
- Data payload
- Error checking information

The destination device reads the frame and determines whether it should process or ignore it.

---

# How It Works

Imagine Computer A wants to send a file to Computer B.

Computer A creates the data.

↓

IP prepares the packet.

↓

Ethernet places the packet inside an Ethernet frame.

↓

The frame travels through a switch.

↓

Computer B receives the frame and extracts the original data.

This process happens thousands of times every second on busy networks.

---

# Diagram

```text
Computer

↓

Ethernet Frame

↓

Switch

↓

Destination Device
```

---

# Real-World Example

Imagine an office with twenty employee computers connected to the same switch.

When one employee prints a document, Ethernet delivers the data across the local network to the printer without involving the Internet.

This local communication happens extremely quickly because Ethernet is optimized for LAN environments.

---

# Cybersecurity Context

Understanding Ethernet helps explain:

- MAC spoofing
- MAC flooding attacks
- Packet captures
- Switch security
- VLAN implementation

Many investigations begin by examining Ethernet traffic before moving to higher-layer protocols.

---

# Common Mistakes

| Mistake | Explanation |
|----------|-------------|
| Ethernet and the Internet are the same thing | Ethernet is used inside local networks. |
| Ethernet uses IP addresses | Ethernet forwards frames using MAC addresses. |
| Ethernet only works with cables | Ethernet standards include copper and fiber connections. |

---

# Interview Questions

- What is Ethernet?
- Which OSI layer uses Ethernet?
- What information is stored inside an Ethernet frame?
- Why are MAC addresses important?
- Where is Ethernet commonly used?

---

# Summary

Ethernet is the foundation of most wired local networks. It allows devices to exchange data efficiently by sending Ethernet frames between MAC addresses on the same network.

---

# Related Chapters

- MAC Addresses
- Switching
- ARP
- VLANs
