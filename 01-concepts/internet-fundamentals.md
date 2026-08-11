---
alias: How the Internet Works
tags: [backend, fundamentals, networking, study-guide]
created: 2026-08-11
status: clear
---

# How Does the Internet Work?

- **Source**: [cs.fyi Guide](https://cs.fyi/guide/how-does-internet-work)
- **Core Concept**: The internet is a global network of networks connecting devices using standardized communication protocols.

---

## 🌐 1. Network Fundamentals & History
- **What is a Network?**: A group of connected computers or devices.
- **The Internet**: A massive global "network of networks".
- **Origin**: Developed in the late 1960s by the US Department of Defense to create a decentralized network capable of surviving partial infrastructure destruction.

---

## 🛠️ 2. Core Concepts & Terminology
- [[Packet]]: A small unit of data transmitted across the network.
- [[Router]]: Hardware responsible for directing traffic packets between different networks.
- [[IP Address]]: A unique numerical identifier (e.g., `192.168.1.1`) assigned to every network device.
- [[Domain Name]]: Human-readable website names (e.g., `google.com`).
- [[DNS (Domain Name System)]]: The system that translates domain names into numerical IP addresses.
- [[HTTP & HTTPS]]: Protocols used to transfer data between web clients and servers.
- [[SSL & TLS]]: Encryption protocols used to establish secure, private internet communication.

---

## ⚡ 3. The TCP/IP Suite & Building Applications
TCP/IP provides reliable, ordered, and error-checked delivery of data between systems.

### Application Anchors
- **Ports**: Unique numbers assigned to specific applications/services running on a device to identify incoming traffic.
- **Sockets**: The definitive combination of an **IP Address + Port Number** representing an active communication endpoint.
- **Connections**: The established link between two sockets where transmission rules (like packet size) are negotiated.
- **Data Transfer**: Information is systematically broken down and sent via structured data segments.

---

## 🔒 4. The Security Handshake (SSL/TLS)
Securing sensitive data transmission relies on three structural phases:
1. **Certificates**: Third-party verification assets signed by a Certificate Authority (CA) to prove server identity.
2. **Handshake**: A quick negotiation where client and server exchange parameters to agree on an encryption algorithm.
3. **Encryption**: The execution layer where all subsequent data is scrambled according to the agreed algorithm.

---

## 🚀 5. Emerging Future Trends
Technologies fundamentally shaping the next era of the internet:
- **5G Network Tech**: Offering faster mobile speeds, higher capacity, and lower latency.
- **Internet of Things (IoT)**: Interconnecting everyday physical devices to global data streams.
- **Artificial Intelligence (AI)**: Driving specialized services like advanced fraud detection and machine learning engines.
- **Blockchain**: Powering decentralized, secure transaction ledgers.
- **Edge Computing**: Shifting data processing to the edge of the network instead of relying entirely on centralized servers.
