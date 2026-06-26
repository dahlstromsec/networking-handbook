# UDP (User Datagram Protocol)

> **Estimated Reading Time:** 10–15 minutes  
> **Difficulty:** Beginner  
> **Prerequisites:** TCP

User Datagram Protocol (UDP) is a lightweight transport protocol designed for speed rather than reliability. Unlike TCP, UDP does not establish a connection before sending data and does not guarantee that packets arrive successfully.

Many real-time applications rely on UDP because receiving data quickly is often more important than receiving every packet.

---

# What You'll Learn

- What UDP is
- Why UDP exists
- How UDP differs from TCP
- Common UDP applications
- Advantages and disadvantages

---

# Why It Matters

Imagine participating in a live video conference.

If one video frame is lost, you may barely notice.

However, waiting for the missing frame to be retransmitted would cause noticeable delays.

UDP accepts occasional packet loss to keep communication fast and responsive.

---

# Core Concepts

UDP is a **connectionless** protocol.

Unlike TCP, UDP:

- Does not establish a connection.
- Does not acknowledge received packets.
- Does not retransmit lost packets.
- Does not guarantee packet order.

Because of this, UDP introduces very little overhead and is significantly faster than TCP in many situations.

---

# How It Works

An application creates data.

↓

UDP places the data into a datagram.

↓

The datagram is sent immediately.

↓

The destination receives the packet.

↓

Communication ends.

If packets are lost during transmission, UDP simply continues sending new packets without attempting recovery.

---

# Diagram

```text
Application

↓

UDP Datagram

↓

Network

↓

Destination
```

---

# Real-World Example

During an online multiplayer game, hundreds of packets are exchanged every second.

If one packet is lost, the game continues.

Waiting for retransmissions would increase latency and negatively affect gameplay.

This makes UDP an ideal choice for real-time communication.

---

# Cybersecurity Context

UDP is frequently encountered during:

- DNS communication
- VoIP
- Live streaming
- Network scanning
- Reflection and amplification attacks

Security analysts often investigate unusual UDP traffic because attackers commonly abuse UDP-based services.

---

# Common Mistakes

| Mistake | Explanation |
|----------|-------------|
| UDP is better than TCP | UDP is faster, but TCP is more reliable. |
| UDP guarantees delivery | Lost packets are not retransmitted. |
| UDP is only used for gaming | Many important services such as DNS also use UDP. |

---

# Interview Questions

- What is UDP?
- Why is UDP faster than TCP?
- Which applications commonly use UDP?
- Does UDP guarantee packet delivery?
- When should UDP be preferred over TCP?

---

# Summary

UDP is a fast, connectionless transport protocol that prioritizes speed over reliability. It is commonly used for real-time communication where low latency is more important than guaranteed delivery.

---

# Related Chapters

- TCP
- ICMP
- DNS
- HTTP
