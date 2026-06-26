# HTTP (Hypertext Transfer Protocol)

> **Estimated Reading Time:** 10–15 minutes  
> **Difficulty:** Beginner  
> **Prerequisites:** TCP

Hypertext Transfer Protocol (HTTP) is the foundation of communication on the World Wide Web. It defines how web browsers and web servers exchange information such as webpages, images, videos and files.

Every time you visit a website, your browser communicates with a web server using HTTP or its secure version, HTTPS.

---

# What You'll Learn

- What HTTP is
- How HTTP communication works
- Requests and responses
- Common HTTP methods
- Common HTTP status codes

---

# Why It Matters

Imagine ordering food at a restaurant.

You place an order.

↓

The kitchen prepares your food.

↓

The waiter delivers your meal.

HTTP follows a similar request-and-response model.

Your browser sends a request to a web server, and the server responds with the requested resource.

---

# Core Concepts

HTTP is an **Application Layer protocol** that runs on top of TCP.

Communication always follows the same pattern:

Client

↓

HTTP Request

↓

Web Server

↓

HTTP Response

↓

Client

The server never sends information until it first receives a request.

---

# How It Works

You enter:

```text
https://example.com
```

↓

Your browser performs a DNS lookup.

↓

A TCP connection is established.

↓

The browser sends an HTTP request.

↓

The server processes the request.

↓

The server returns an HTTP response.

↓

Your browser displays the webpage.

This process happens every time you open a website.

---

# Diagram

```text
Browser

↓

HTTP Request

↓

Web Server

↓

HTTP Response

↓

Webpage Displayed
```

---

# Common HTTP Methods

| Method | Purpose |
|----------|----------|
| GET | Retrieve data |
| POST | Send data |
| PUT | Update data |
| DELETE | Remove data |

---

# Common Status Codes

| Code | Meaning |
|------|----------------|
| 200 | OK |
| 301 | Moved Permanently |
| 400 | Bad Request |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |
| 500 | Internal Server Error |

---

# Real-World Example

You visit:

```text
https://github.com
```

Your browser sends an HTTP GET request asking for the homepage.

The server responds with HTML, CSS, JavaScript and images.

Your browser combines these resources and displays the completed webpage.

---

# Cybersecurity Context

HTTP is frequently analyzed during:

- Web application testing
- Packet analysis
- Proxy investigations
- Malware investigations
- API security testing

Because HTTP is unencrypted, attackers can potentially intercept or modify traffic unless HTTPS is used.

---

# Common Mistakes

| Mistake | Explanation |
|----------|-------------|
| HTTP encrypts traffic | HTTP sends data in plaintext. HTTPS provides encryption. |
| HTTP and HTML are the same | HTTP transfers webpages. HTML describes webpage content. |
| Browsers only use GET requests | Modern web applications use many different HTTP methods. |

---

# Interview Questions

- What is HTTP?
- What is the difference between HTTP and HTTPS?
- What does a 404 status code mean?
- What is an HTTP GET request?
- Why does HTTP require TCP?

---

# Summary

HTTP enables communication between web browsers and servers using a request-and-response model. It forms the foundation of modern web browsing and web applications.

---

# Related Chapters

- HTTPS
- TCP
- DNS
- Email Protocols
