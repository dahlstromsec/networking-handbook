# IPv4 Addressing

> Estimated Reading Time: 8–10 minutes
> Difficulty: Beginner
> Prerequisites: VLANs

## Introduction

Every device connected to a network needs an IP address so other devices know where to send data. IPv4 is the most widely used addressing system on today's networks.

---

## What You'll Learn

- What an IPv4 address is
- Public vs Private IP addresses
- Network and host portions
- Special IPv4 addresses

---

## Why It Matters

Without IP addresses, routers would have no way to deliver packets between networks.

---

## Main Concept

Example IPv4 address:

192.168.1.25

An IPv4 address identifies a device on an IP network.

Common private ranges:

| Range | CIDR |
|------|------|
|10.0.0.0 - 10.255.255.255|10.0.0.0/8|
|172.16.0.0 - 172.31.255.255|172.16.0.0/12|
|192.168.0.0 - 192.168.255.255|192.168.0.0/16|

---

## Diagram

PC (192.168.1.25)

↓

Default Gateway (192.168.1.1)

↓

Internet

---

## Real-World Example

Your home router typically assigns private IPv4 addresses to every device while using one public IP address to communicate with the Internet.

---

## Cybersecurity Context

Understanding IPv4 addressing is essential for firewall rules, network scanning and incident response.

---

## Interview Questions

- What is an IPv4 address?
- What is the difference between a public and private IP?
- Why can't private IP addresses be routed across the Internet?

---

## Summary

IPv4 addresses uniquely identify devices and enable communication across networks.

---

## Related Chapters

- Subnetting
- Routing
- NAT & PAT
