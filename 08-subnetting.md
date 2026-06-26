# Subnetting

> Estimated Reading Time: 10 minutes
> Difficulty: Beginner–Intermediate
> Prerequisites: IPv4 Addressing

## Introduction

Subnetting divides a network into smaller networks. It improves organization, security and efficient use of IP addresses.

---

## What You'll Learn

- Network vs Host bits
- CIDR notation
- Subnet masks
- Why subnetting is important

---

## Why It Matters

Organizations rarely place every device on one giant network. Smaller networks improve performance and reduce security risks.

---

## Main Concept

Common subnet masks:

| CIDR | Mask |
|------|----------------|
|/24|255.255.255.0|
|/25|255.255.255.128|
|/26|255.255.255.192|

Smaller subnets create more networks with fewer hosts.

---

## Diagram

192.168.1.0/24

↓

Office

↓

Servers

↓

Guest Wi-Fi

---

## Real-World Example

A company separates employees, servers and guest devices into different subnets to improve performance and security.

---

## Cybersecurity Context

Subnetting limits broadcast traffic and supports network segmentation, reducing an attacker's ability to move across a network.

---

## Interview Questions

- What does /24 mean?
- Why do organizations subnet networks?
- What is the purpose of a subnet mask?

---

## Summary

Subnetting organizes networks into smaller, more manageable sections.

---

## Related Chapters

- IPv4 Addressing
- Routing
- VLANs
