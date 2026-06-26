# VLANs

> **Estimated Reading Time:** 10–15 minutes  
> **Difficulty:** Beginner  
> **Prerequisites:** Switching

A Virtual Local Area Network (VLAN) allows a physical network to be divided into multiple logical networks. Although devices may be connected to the same switch, VLANs isolate traffic so devices communicate only with others in the same VLAN unless routing is configured.

VLANs are one of the most common technologies used in business networks because they improve organization, performance and security.

---

# What You'll Learn

- What a VLAN is
- Why VLANs exist
- Broadcast domains
- Access and trunk ports
- How VLANs improve security

---

# Why It Matters

Imagine a company with 200 employees.

Without VLANs, every computer, printer, server and guest device belongs to the same network.

This creates unnecessary broadcast traffic and allows compromised devices to communicate more easily with other systems.

VLANs solve this problem by separating one physical network into multiple isolated logical networks.

---

# Core Concepts

A VLAN creates a separate **broadcast domain**.

Devices inside the same VLAN can communicate directly.

Devices in different VLANs cannot communicate unless traffic passes through a router or Layer 3 switch.

A company might organize its network like this:

- **VLAN 10** – Office Computers
- **VLAN 20** – Servers
- **VLAN 30** – Printers
- **VLAN 40** – Guest Wi-Fi

Although all devices are connected to the same physical switch, they behave as though they are on different networks.

---

# How It Works

A computer sends an Ethernet frame.

↓

The switch identifies which VLAN the incoming port belongs to.

↓

The frame is forwarded only to ports within that VLAN.

↓

Devices in other VLANs never receive the traffic.

↓

If communication between VLANs is required, a router or Layer 3 switch performs the routing.

---

# Diagram

```text
                Switch

        ┌─────────────────┐

 VLAN 10 │ Office Computers │

 VLAN 20 │     Servers      │

 VLAN 30 │     Printers     │

 VLAN 40 │    Guest Wi-Fi   │

        └─────────────────┘
```

Each VLAN behaves like an independent network.

---

# Real-World Example

Imagine a company with employees, servers and visitors.

Instead of allowing every device to share one network, the company creates separate VLANs.

Employees cannot directly access the guest Wi-Fi network.

Guests cannot communicate with internal servers.

This reduces unnecessary traffic while improving overall security.

---

# Cybersecurity Context

VLANs are an important part of **network segmentation**.

If one employee computer becomes infected with malware, VLANs help limit an attacker's ability to move laterally across the network.

Although VLANs are not a replacement for firewalls, they provide an additional layer of protection by separating different parts of the network.

---

# Common Mistakes

| Mistake | Explanation |
|----------|-------------|
| VLANs require multiple switches | One switch can contain many VLANs. |
| VLANs are physical networks | VLANs are logical networks created through switch configuration. |
| Devices in different VLANs communicate automatically | Routing is required for communication between VLANs. |

---

# Interview Questions

- What problem do VLANs solve?
- What is a broadcast domain?
- What is the difference between an access port and a trunk port?
- Why are VLANs important for network security?

---

# Summary

VLANs logically divide one physical network into multiple isolated networks. This improves organization, reduces broadcast traffic and strengthens network security.

---

# Related Chapters

- Switching
- IPv4 Addressing
- Routing
- Firewalls
