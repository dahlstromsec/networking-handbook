# Email Protocols

> **Estimated Reading Time:** 10–15 minutes  
> **Difficulty:** Beginner  
> **Prerequisites:** TCP

Email communication relies on several protocols working together. SMTP is responsible for sending messages, while POP3 and IMAP allow users to retrieve email from a mail server.

Although users rarely notice these protocols, they are essential for modern communication and are frequently encountered in cybersecurity investigations.

---

# What You'll Learn

- SMTP
- POP3
- IMAP
- How email is delivered
- Differences between POP3 and IMAP

---

# Why It Matters

When you send an email, it doesn't travel directly from your computer to the recipient.

Instead, it passes through multiple mail servers before reaching the recipient's mailbox.

Different protocols handle sending and receiving during this journey.

---

# Core Concepts

Three primary email protocols exist.

| Protocol | Purpose |
|----------|----------------|
| SMTP | Sends email |
| POP3 | Downloads email |
| IMAP | Synchronizes email |

SMTP is responsible for sending messages.

POP3 downloads messages to a device.

IMAP synchronizes messages across multiple devices, allowing users to access the same mailbox from phones, tablets and computers.

---

# How It Works

You send an email.

↓

Your email client sends the message using SMTP.

↓

The message reaches the recipient's mail server.

↓

The recipient opens their email application.

↓

POP3 or IMAP retrieves the message.

↓

The email appears in the recipient's inbox.

---

# Diagram

```text
Sender

↓

SMTP

↓

Mail Server

↓

POP3 / IMAP

↓

Recipient
```

---

# Real-World Example

You send an email from your laptop.

The message travels through your organization's SMTP server before being delivered to the recipient's mail provider.

Later, the recipient reads the message on both their phone and laptop using IMAP, keeping both devices synchronized.

---

# Cybersecurity Context

Email remains one of the most common attack vectors.

Security professionals investigate:

- Phishing emails
- Malicious attachments
- Email spoofing
- Business Email Compromise (BEC)
- Spam campaigns

Understanding email protocols helps analysts investigate how malicious emails are delivered and received.

---

# Common Mistakes

| Mistake | Explanation |
|----------|-------------|
| SMTP receives email | SMTP sends email. |
| POP3 and IMAP perform the same function | IMAP synchronizes mail while POP3 primarily downloads it. |
| Email travels directly between users | Messages pass through one or more mail servers. |

---

# Interview Questions

- What protocol sends email?
- What is the difference between POP3 and IMAP?
- Why do organizations use SMTP?
- Why is email important in cybersecurity?
- Which protocol is best for multiple devices?

---

# Summary

Email communication depends on SMTP for sending messages and POP3 or IMAP for receiving them. Together, these protocols enable reliable email delivery across the Internet.

---

# Related Chapters

- TCP
- HTTPS
- DNS
