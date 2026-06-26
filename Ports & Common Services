# Ports & Common Services

> **Estimated Reading Time:** 10–15 minutes  
> **Difficulty:** Beginner  
> **Prerequisites:** TCP, UDP

Network ports allow multiple applications and services to communicate over a single IP address. While an IP address identifies a device on a network, a **port identifies the specific service or application** running on that device.

Every time you browse the web, connect to a remote server, or send an email, your computer communicates using one or more network ports.

---

# What You'll Learn

- What network ports are
- Why ports exist
- TCP vs UDP ports
- Common well-known ports
- Why ports are important in cybersecurity

---

# Why It Matters

Imagine calling a large company.

The company's phone number gets you to the building.

The extension number connects you to the correct department.

Networking works in a similar way.

An IP address identifies the computer.

A port identifies the application or service you want to communicate with.

Without ports, computers wouldn't know whether incoming traffic was intended for a web server, email server or SSH service.

---

# Core Concepts

A network port is a **logical communication endpoint**.

Ports range from:

```text
0 - 65535
```

Ports are divided into three categories.

| Range | Description |
|---------|------------------------------|
| 0–1023 | Well-Known Ports |
| 1024–49151 | Registered Ports |
| 49152–65535 | Dynamic / Ephemeral Ports |

Servers usually listen on well-known ports.

Clients typically use temporary (ephemeral) ports when connecting.

---

# How It Works

You open:

```text
https://example.com
```

↓

DNS finds the server's IP address.

↓

Your browser opens a temporary source port.

↓

The browser connects to:

```text
Destination Port 443
```

↓

The web server receives the request.

↓

The webpage is returned to your browser.

Although many users may connect to the same server simultaneously, port numbers keep each connection separate.

---

# Diagram

```text
Browser

↓

192.168.1.20:52341

↓

Internet

↓

203.0.113.15:443

↓

HTTPS Server
```

---

# Common Ports

| Port | Protocol | Service |
|------:|----------|----------|
| 20/21 | TCP | FTP |
| 22 | TCP | SSH |
| 23 | TCP | Telnet |
| 25 | TCP | SMTP |
| 53 | TCP / UDP | DNS |
| 67/68 | UDP | DHCP |
| 80 | TCP | HTTP |
| 110 | TCP | POP3 |
| 143 | TCP | IMAP |
| 161 | UDP | SNMP |
| 389 | TCP / UDP | LDAP |
| 443 | TCP | HTTPS |
| 445 | TCP | SMB |
| 3389 | TCP | Remote Desktop (RDP) |

---

# Real-World Example

A company hosts a public website.

The firewall allows:

- TCP Port 443 (HTTPS)

Everything else remains blocked from the Internet.

Employees connect securely through HTTPS while unnecessary services remain inaccessible.

---

# Cybersecurity Context

Port numbers appear constantly during cybersecurity work.

Analysts use them when:

- Performing Nmap scans.
- Reviewing firewall rules.
- Analyzing packet captures.
- Investigating suspicious network traffic.
- Detecting exposed services.

Knowing common ports makes it much easier to understand what network traffic is attempting to do.

---

# Common Mistakes

| Mistake | Explanation |
|----------|-------------|
| Port 443 makes a website secure | HTTPS provides security, not the port number itself. |
| Ports are physical hardware | Ports are logical software endpoints used by applications. |
| Closed ports are always a problem | Many services should remain closed to reduce the attack surface. |

---

# Interview Questions

- What is a network port?
- What is the difference between an IP address and a port?
- Which port does HTTPS use?
- Why do clients use ephemeral ports?
- Why are ports important in cybersecurity?

---

# Summary

Ports allow multiple applications to communicate over a single IP address by identifying the destination service. Understanding common ports is essential for networking, firewall configuration, troubleshooting and cybersecurity.

---

# Related Chapters

- TCP
- UDP
- HTTP
- HTTPS
- SSH
- Firewalls
- Wireshark & Network Troubleshooting
