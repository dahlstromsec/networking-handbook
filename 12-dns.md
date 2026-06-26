# DNS (Domain Name System)

> **Estimated Reading Time:** 10–15 minutes  
> **Difficulty:** Beginner  
> **Prerequisites:** IPv4 Addressing

The Domain Name System (DNS) translates human-readable domain names into IP addresses. Instead of remembering numeric IP addresses for every website or service, users can simply type a name such as **google.com** or **github.com**.

Without DNS, using the Internet would be significantly more difficult.

---

# What You'll Learn

- What DNS is
- Why DNS exists
- How DNS lookups work
- Common DNS record types
- Basic troubleshooting

---

# Why It Matters

Imagine having to remember the phone number of every person you wanted to call.

That would quickly become impossible.

DNS solves the same problem for the Internet.

Instead of remembering IP addresses, we remember names.

DNS performs the translation automatically.

---

# Core Concepts

DNS is often described as the **phonebook of the Internet**.

When you enter:

```text
github.com
```

Your computer asks a DNS server:

> "What IP address belongs to github.com?"

The DNS server replies with the correct IP address.

Only then can your computer establish a connection.

Common DNS record types include:

| Record | Purpose |
|---------|---------|
| A | IPv4 Address |
| AAAA | IPv6 Address |
| CNAME | Alias |
| MX | Mail Server |
| TXT | Text Information |

---

# How It Works

You enter:

```text
https://example.com
```

↓

Your computer checks its local DNS cache.

↓

If no record exists, it sends a DNS query.

↓

The DNS server replies with an IP address.

↓

Your browser connects to the destination server.

↓

The webpage loads.

Most DNS lookups complete in only a few milliseconds.

---

# Diagram

```text
Browser

↓

DNS Query

↓

DNS Server

↓

IP Address Returned

↓

Connection Established
```

---

# Useful Commands

```bash
nslookup example.com
```

Queries a DNS server.

```bash
dig example.com
```

Displays detailed DNS information.

---

# Real-World Example

You open your browser and visit:

```text
https://openai.com
```

Your computer does not know the server's IP address.

A DNS lookup is performed automatically.

Once the IP address is returned, your browser connects to the correct web server without you ever noticing the DNS request.

---

# Cybersecurity Context

DNS plays a major role in cybersecurity.

Security professionals investigate DNS traffic to identify:

- Malware communication
- Phishing domains
- Command-and-Control (C2) servers
- Suspicious domain lookups
- DNS tunneling attacks

Many security tools monitor DNS because almost every Internet connection begins with a DNS request.

---

# Common Mistakes

| Mistake | Explanation |
|----------|-------------|
| DNS hosts websites | DNS only translates names into IP addresses. |
| DNS is only used by browsers | Almost every Internet-connected application relies on DNS. |
| DNS requests are always encrypted | Traditional DNS is unencrypted unless technologies such as DNS over HTTPS (DoH) or DNS over TLS (DoT) are used. |

---

# Interview Questions

- What is DNS?
- Why is DNS necessary?
- What does an A record contain?
- What is the difference between an A record and an AAAA record?
- Why is DNS important in cybersecurity?

---

# Summary

DNS translates domain names into IP addresses, allowing users to access Internet resources using memorable names instead of numeric addresses.

---

# Related Chapters

- DHCP
- HTTP
- HTTPS
- IPv4 Addressing
