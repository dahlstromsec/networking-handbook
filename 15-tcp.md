# TCP

> Estimated Reading Time: 8–10 minutes
> Difficulty: Beginner
> Prerequisites: NAT & PAT

## Introduction

Transmission Control Protocol (TCP) is a reliable transport protocol used whenever data must arrive completely and in the correct order.

---

## What You'll Learn

- Why TCP exists
- The three-way handshake
- Reliable delivery
- Common TCP applications

---

## Why It Matters

Banking, web browsing, email and SSH rely on TCP because lost or out-of-order data could cause problems.

---

## Main Concept

Connection setup:

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

Connection established.

---

## Key Features

- Reliable delivery
- Ordered packets
- Error checking
- Retransmission
- Flow control

---

## Real-World Example

When downloading a PDF, TCP ensures every piece of the file arrives before it is opened.

---

## Cybersecurity Context

TCP is heavily analyzed during incident response, firewall configuration and packet captures.

---

## Interview Questions

- Why is TCP reliable?
- What is the three-way handshake?
- Name three protocols that use TCP.

---

## Summary

TCP prioritizes reliability and accuracy over speed.

---

## Related Chapters

- UDP
- HTTP
- HTTPS
- SSH
