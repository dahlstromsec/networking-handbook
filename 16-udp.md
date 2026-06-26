# UDP

> Estimated Reading Time: 8–10 minutes
> Difficulty: Beginner
> Prerequisites: TCP

## Introduction

User Datagram Protocol (UDP) is a lightweight transport protocol designed for speed rather than reliability.

---

## What You'll Learn

- Why UDP exists
- TCP vs UDP
- Common UDP applications

---

## Why It Matters

Some applications value low latency more than guaranteed delivery.

---

## Main Concept

Application

↓

UDP

↓

IP

↓

Network

No connection setup.
No acknowledgements.
No retransmissions.

---

## Common Uses

- DNS
- VoIP
- Live streaming
- Online gaming

---

## Real-World Example

A live video call can tolerate an occasional lost packet better than delayed audio.

---

## Cybersecurity Context

Many attacks target UDP services because they are connectionless. Analysts also investigate unusual UDP traffic during incident response.

---

## Interview Questions

- Why is UDP faster than TCP?
- Which protocol uses UDP for name resolution?
- When would UDP be preferred?

---

## Summary

UDP sacrifices reliability to achieve low latency and fast communication.

---

## Related Chapters

- TCP
- DNS
- ICMP
