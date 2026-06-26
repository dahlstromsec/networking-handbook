# DNS

> Estimated Reading Time: 8–10 minutes
> Difficulty: Beginner
> Prerequisites: IPv4 Addressing

## Introduction

The Domain Name System (DNS) translates human-readable domain names into IP addresses so devices can locate one another.

---

## What You'll Learn

- DNS purpose
- Common record types
- DNS lookups
- Troubleshooting basics

---

## Why It Matters

Remembering IP addresses is impractical. DNS allows users to access services using names such as example.com.

---

## Main Concept

example.com

↓

DNS Query

↓

DNS Server

↓

93.184.216.34

↓

Connection Established

---

## Common Records

| Record | Purpose |
|---|---|
| A | IPv4 Address |
| AAAA | IPv6 Address |
| CNAME | Alias |
| MX | Mail Server |
| TXT | Text Information |

---

## Useful Commands

```bash
nslookup example.com
dig example.com
```

---

## Cybersecurity Context

DNS plays an important role in phishing, malware communication and threat hunting.

---

## Interview Questions

- What does DNS do?
- What is an A record?
- Why is DNS important?

---

## Summary

DNS converts names into IP addresses, allowing users to access services without memorizing numeric addresses.

---

## Related Chapters

- DHCP
- HTTP
