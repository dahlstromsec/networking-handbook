# TCP/IP Model

> Estimated Reading Time: 8–10 minutes
> Difficulty: Beginner
> Prerequisites: OSI Model

## Introduction

The TCP/IP model describes how modern networks communicate. Unlike the OSI model, it is based on protocols actually used on today's Internet.

## What You'll Learn

- Four TCP/IP layers
- Relationship to the OSI model
- Common protocols

## Why It Matters

Most network troubleshooting, Wireshark analysis, and cybersecurity work use TCP/IP terminology.

## Layers

| Layer | Common Protocols |
|---|---|
|Application|HTTP, HTTPS, DNS, SSH|
|Transport|TCP, UDP|
|Internet|IP, ICMP|
|Network Access|Ethernet, Wi-Fi|

## Diagram

Browser
↓
TCP
↓
IP
↓
Ethernet
↓
Network

## Real-World Example

When visiting a website, HTTP uses TCP, TCP uses IP, and IP travels across Ethernet or Wi-Fi.

## Cybersecurity Context

Understanding TCP/IP helps analyze packets, firewall rules, VPNs, and network attacks.

## Interview Questions

- Why is TCP/IP used instead of OSI in real networks?
- Which protocols belong to the Transport layer?
- Which layer contains IP?

## Summary

TCP/IP is the practical networking model used across the Internet and forms the foundation for modern networking.

## Related Chapters

- OSI Model
- IPv4 Addressing
- TCP
- UDP
