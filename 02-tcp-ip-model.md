# TCP/IP Model

> **Estimated Reading Time:** 10–15 minutes  
> **Difficulty:** Beginner  
> **Prerequisites:** OSI Model

The TCP/IP Model is the networking model used by the modern Internet. Unlike the OSI Model, which is primarily a conceptual framework, TCP/IP describes the protocols that computers actually use to communicate.

Whenever you browse a website, send an email, connect with SSH, or stream a video, your data is travelling through the TCP/IP model.

---

# What You'll Learn

- What the TCP/IP Model is
- The four TCP/IP layers
- How it compares to the OSI Model
- Common protocols at each layer
- Why it is used in modern networking

---

# Why It Matters

The OSI Model helps explain networking.

The TCP/IP Model is how networking actually works.

Most operating systems, routers, switches and firewalls use TCP/IP terminology. Understanding this model makes it much easier to troubleshoot networks and understand packet captures.

---

# Core Concepts

The TCP/IP Model contains four layers.

| Layer | Common Protocols |
|--------|------------------|
| Application | HTTP, HTTPS, DNS, SSH, SMTP |
| Transport | TCP, UDP |
| Internet | IP, ICMP |
| Network Access | Ethernet, Wi-Fi |

Each layer performs a specific task before passing data to the next layer.

Unlike the OSI Model, some OSI layers are combined within the TCP/IP Model. This makes it simpler while still describing how modern networks operate.

---

# How It Works

Imagine opening your browser and visiting:

```text
https://example.com
```

Your browser creates an HTTP request.

↓

TCP prepares a reliable connection.

↓

IP determines where the packet should be sent.

↓

Ethernet or Wi-Fi transmits the frame across the local network.

↓

The destination server receives the data and processes it before sending a response back through the same layers.

Although this entire process usually takes less than a second, every request follows this layered approach.

---

# Diagram

```text
Application
    ↓
Transport
    ↓
Internet
    ↓
Network Access
```

---

# Real-World Example

When you visit a website:

- HTTP requests the webpage.
- TCP ensures every packet arrives correctly.
- IP routes the packets across different networks.
- Ethernet or Wi-Fi delivers the frames across the local network.

Each protocol performs one specific job before passing the data to the next layer.

---

# Cybersecurity Context

Most network investigations focus on TCP/IP rather than the OSI Model.

Security professionals use TCP/IP when:

- Analyzing packet captures in Wireshark.
- Configuring firewalls.
- Troubleshooting VPN connections.
- Investigating suspicious network traffic.
- Understanding malware communication.

---

# Common Mistakes

| Mistake | Explanation |
|----------|-------------|
| TCP/IP and OSI are identical | They describe networking differently and contain a different number of layers. |
| TCP/IP only refers to TCP and IP | The model includes many protocols such as HTTP, DNS, ICMP and UDP. |
| Every protocol belongs to the Application Layer | Protocols exist at multiple layers depending on their purpose. |

---

# Interview Questions

- What is the TCP/IP Model?
- How many layers does the TCP/IP Model contain?
- Which protocols belong to the Transport Layer?
- What is the difference between the OSI Model and the TCP/IP Model?
- Why is TCP/IP used on the Internet?

---

# Summary

The TCP/IP Model is the networking model used by today's Internet. It divides communication into four layers, each responsible for a different part of moving data between devices.

---

# Related Chapters

- OSI Model
- Ethernet
- IPv4 Addressing
- TCP
- UDP
