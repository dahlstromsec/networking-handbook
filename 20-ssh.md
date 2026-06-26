# SSH (Secure Shell)

> **Estimated Reading Time:** 10–15 minutes  
> **Difficulty:** Beginner  
> **Prerequisites:** TCP

Secure Shell (SSH) is a protocol used to securely connect to remote computers over a network. It encrypts all communication between the client and the remote system, protecting credentials and commands from being intercepted.

SSH has become the standard method for remotely administering Linux servers, networking equipment and cloud infrastructure.

---

# What You'll Learn

- What SSH is
- Why SSH exists
- Password vs Key Authentication
- Common SSH usage
- Why encryption is important

---

# Why It Matters

Imagine managing a server located in another country.

Travelling to the server every time you needed to change a configuration would be impossible.

SSH allows administrators to securely control remote systems from anywhere with network access.

---

# Core Concepts

SSH operates at the **Application Layer** and typically uses **TCP port 22**.

SSH provides:

- Encrypted communication
- Secure authentication
- Remote command execution
- Secure file transfers (SCP/SFTP)
- Port forwarding

Unlike older protocols such as Telnet, SSH encrypts all traffic between the client and server.

---

# How It Works

You run:

```bash
ssh username@192.168.1.10
```

↓

The SSH client contacts the server.

↓

The server presents its host key.

↓

The client verifies the server's identity.

↓

Authentication takes place.

↓

An encrypted session is established.

↓

Commands entered on your computer are securely executed on the remote server.

---

# Diagram

```text
Administrator

↓

SSH Client

↓

Encrypted Tunnel

↓

SSH Server

↓

Remote Linux System
```

---

# Common Commands

```bash
ssh username@server-ip
```

Connect to a remote server.

```bash
scp file.txt user@server:/home/user/
```

Copy a file securely.

```bash
sftp username@server-ip
```

Transfer files interactively.

---

# Real-World Example

A system administrator manages dozens of Linux servers hosted in a cloud environment.

Instead of physically accessing each machine, the administrator connects securely using SSH to install updates, review logs and restart services.

---

# Cybersecurity Context

SSH is one of the most important protocols in cybersecurity.

It is commonly used for:

- Remote server administration
- Penetration testing
- Secure automation
- Incident response
- Cloud infrastructure management

Organizations often disable password authentication and require SSH keys for improved security.

---

# Common Mistakes

| Mistake | Explanation |
|----------|-------------|
| SSH is only for Linux | SSH is available on Linux, macOS and Windows. |
| SSH is the same as Telnet | SSH encrypts communication, while Telnet does not. |
| Passwords are the most secure authentication method | SSH keys are generally more secure than passwords. |

---

# Interview Questions

- What is SSH used for?
- Why is SSH preferred over Telnet?
- Which port does SSH use by default?
- What is the difference between password and key authentication?
- Why is SSH important in cybersecurity?

---

# Summary

SSH provides secure remote administration by encrypting communication between clients and servers. It has become the standard protocol for managing modern systems and infrastructure.

---

# Related Chapters

- HTTPS
- TCP
- Firewalls
- VPNs
