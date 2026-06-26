# TCP (Transmission Control Protocol)

> **Estimated Reading Time:** 10–15 minutes  
> **Difficulty:** Beginner  
> **Prerequisites:** NAT & PAT

Transmission Control Protocol (TCP) is one of the core transport protocols used on modern networks. It provides reliable, ordered communication between devices, ensuring that data arrives completely and in the correct sequence.

Many of the Internet's most important services, including web browsing, email and remote administration, rely on TCP.

---

# What You'll Learn

- What TCP is
- Why TCP exists
- The Three-Way Handshake
- Reliable communication
- Common TCP applications

---

# Why It Matters

Imagine downloading an important document.

If pieces of the file were lost or arrived out of order, the file would become corrupted.

TCP solves this problem by ensuring that every packet arrives successfully before communication continues.

---

# Core Concepts

TCP is a **connection-oriented** protocol.

Before data is exchanged, both devices establish a connection.

TCP provides:

- Reliable delivery
- Packet sequencing
- Error detection
- Retransmission of lost packets
- Flow control

These features make TCP slower than UDP but significantly more reliable.

---

# How It Works

Before communication begins, TCP performs the **Three-Way Handshake**.

```text
Client

↓

SYN

↓

Server

↓

SYN-ACK

↓

Client

↓

ACK

↓

Connection Established
```

Once the connection has been established, both devices exchange data while acknowledging successful delivery.

If a packet is lost, TCP automatically retransmits it.

---

# Diagram

```text
Client

↓

Three-Way Handshake

↓

Reliable Connection

↓

Data Transfer

↓

Connection Closed
```

---

# Real-World Example

You download a PDF from a website.

The file may be divided into hundreds of packets.

TCP ensures every packet arrives correctly and reorders them if necessary before the document is opened.

Without TCP, the downloaded file could become incomplete or corrupted.

---

# Cybersecurity Context

TCP appears constantly during cybersecurity investigations.

Analysts examine TCP traffic when:

- Reviewing packet captures
- Troubleshooting network issues
- Investigating suspicious connections
- Configuring firewall rules
- Detecting network attacks

Understanding TCP is essential when using tools such as Wireshark.

---

# Common Mistakes

| Mistake | Explanation |
|----------|-------------|
| TCP is faster than UDP | TCP sacrifices speed to achieve reliability. |
| TCP guarantees low latency | Reliable communication often introduces additional overhead. |
| TCP only transfers files | TCP supports many protocols including HTTP, HTTPS and SSH. |

---

# Interview Questions

- What is TCP?
- Why is TCP considered reliable?
- What is the Three-Way Handshake?
- Why does TCP retransmit packets?
- Name three protocols that use TCP.

---

# Summary

TCP provides reliable communication by establishing a connection, verifying packet delivery and retransmitting lost data when necessary.

---

# Related Chapters

- UDP
- HTTP
- HTTPS
- SSH
