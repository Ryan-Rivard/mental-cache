---
alias: [Hypertext Transfer Protocol, http, web protocol]
tags: [backend, fundamentals, networking, concept]
created: 2026-08-11
status: master-node
---

# Hypertext Transfer Protocol (HTTP)

- **Source**: [Cloudflare Learning Center](https://www.cloudflare.com/learning/ddos/glossary/hypertext-transfer-protocol-http/)
- **Core Concept**: HTTP is the foundational, application-layer communication protocol used to load webpages across the internet using hypertext links.

---

## 🏗️ 1. Protocol Architecture
- **Layer 7 Protocol**: Operates strictly at the **Application Layer** of the network protocol stack.
- **Dependency**: Runs on top of transport layer protocols to handle actual device connections.
- **Core Mechanism**: A stateless, standard **Client-Server model** flow where a client makes a request and a server returns a response.

---

## 🔄 2. The Request-Response Lifecycle

### The HTTP Request
Sent by the client (browser) to pull data from a host server. Key components inside a request:
- **HTTP Method**: The verb defining the action (e.g., `GET`, `POST`, `PUT`, `DELETE`).
- **Target URL**: The path of the resource being requested.
- **HTTP Version**: Specifies the version used (e.g., `HTTP/1.1`, `HTTP/2`, `HTTP/3`).
- **HTTP Headers**: Metadata arrays holding transfer details, browser types, and cookie data.
- **Body**: Optional payload data (typically used in `POST` or `PUT` requests).

### The HTTP Response
Returned by the server after computing the client's request. Key components inside a response:
- **Status Code**: A 3-digit numerical indicator of request success or failure (e.g., `200 OK`, `404 Not Found`).
- **HTTP Headers**: Server-side metadata passing caching info, content-type, or connection rules.
- **Body**: The literal data payload requested (e.g., raw HTML code, images, or JSON data strings).

---

## 🔒 3. Evolution: HTTP vs HTTPS
- [[HTTP]]: Transmits data across the network in completely unencrypted clear text. Vulnerable to interception.
- [[What is HTTPS]]: The secure extension of HTTP. It uses **SSL/TLS encryption** to encrypt the request and response channels, ensuring data privacy and preventing credential tampering.

---

## 🔗 Related Concept Nodes
- [[Internet Fundamentals]]
- [[What is HTTPS]]
- [[Packet]]
- [[Router]]
