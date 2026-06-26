# DHCP (Dynamic Host Configuration Protocol)

> **Estimated Reading Time:** 10–15 minutes  
> **Difficulty:** Beginner  
> **Prerequisites:** DNS

The Dynamic Host Configuration Protocol (DHCP) automatically assigns network configuration to devices when they connect to a network. Instead of manually configuring every computer with an IP address, subnet mask and default gateway, DHCP performs the process automatically.

Nearly every home and business network relies on DHCP.

---

# What You'll Learn

- What DHCP is
- Why DHCP exists
- The DORA process
- DHCP leases
- Common troubleshooting

---

# Why It Matters

Imagine manually configuring the network settings for hundreds of employee computers.

Every new laptop, printer or phone would require manual configuration.

DHCP eliminates this work by automatically assigning network settings whenever a device joins the network.

---

# Core Concepts

A DHCP server provides devices with:

- IP Address
- Subnet Mask
- Default Gateway
- DNS Server
- Lease Duration

Instead of permanently assigning an address, DHCP leases an address for a limited period.

When the lease expires, the device renews it automatically.

---

# How It Works

The DHCP process is commonly remembered as **DORA**.

**Discover**

↓

The client searches for a DHCP server.

↓

**Offer**

The DHCP server offers an available IP address.

↓

**Request**

The client requests the offered address.

↓

**Acknowledge**

The server confirms the lease.

The entire process usually completes in only a few seconds.

---

# Diagram

```text
Client

↓

Discover

↓

Offer

↓

Request

↓

Acknowledge

↓

IP Address Assigned
```

---

# Useful Commands

```bash
ip a
```

View the assigned IP address.

```bash
ipconfig /all
```

(View DHCP information on Windows.)

---

# Real-World Example

You connect your laptop to a coffee shop Wi-Fi network.

Within seconds your computer automatically receives:

- An IP address
- Default gateway
- DNS server
- Subnet mask

No manual configuration is required.

---

# Cybersecurity Context

DHCP simplifies administration but also introduces risks.

Examples include:

- Rogue DHCP servers
- Incorrect network configuration
- Traffic redirection attacks
- Unauthorized devices joining the network

Enterprise networks often implement DHCP Snooping to protect against malicious DHCP servers.

---

# Common Mistakes

| Mistake | Explanation |
|----------|-------------|
| DHCP only assigns IP addresses | DHCP also provides DNS servers, gateways and other configuration. |
| DHCP addresses never change | Addresses are leased and may change over time. |
| Every network requires DHCP | Static IP addresses can also be configured manually. |

---

# Interview Questions

- What is DHCP?
- What does DORA stand for?
- What information does DHCP provide?
- What is a DHCP lease?
- Why is DHCP important?

---

# Summary

DHCP automates network configuration by assigning IP addresses and other essential settings to devices. This simplifies administration and allows new devices to join a network quickly.

---

# Related Chapters

- DNS
- NAT & PAT
- IPv4 Addressing
- Routing
