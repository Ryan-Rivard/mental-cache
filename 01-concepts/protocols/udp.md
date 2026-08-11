---
alias: [User Datagram Protocol, udp, connectionless]
tags: [backend, fundamentals, networking, protocol]
created: 2026-08-11
status: master-node
---

# User Datagram Protocol (UDP)

UDP is a lightweight, connectionless Transport Layer protocol optimized for maximum speed and execution efficiency over reliability.

---

## ⚙️ Core Architecture
- **Connectionless Execution**: Sends data immediately without running an initial handshake or connection check.
- **Independent Datagrams**: Treats every packet as a fully isolated, standalone message entity.
- **Minimalist Footprint**: Uses a tiny, fixed header size of exactly **8 bytes** containing only Ports, Length, and Checksum fields.

---

## ⚠️ Known Limitations
- **No Delivery Guarantee**: Packets are cast onto the network blindly. Dropped or missing packets are discarded without retransmission.
- **Unordered Delivery**: Packets may traverse different pathways and arrive at the destination in complete disarray.
- **No Flow Control**: Fires packets at full physical speed, which can cause network drops if buffers fill up.

---

## 🎯 Ideal Use Cases
- **Real-Time Streaming**: Voice over IP (VoIP), live video conferencing, and online multi-player video games where speed matters more than absolute pixel perfect accuracy.
- **Fast, One-Shot Lookups**: Network micro-transactions like [[DNS (Domain Name System)]] or DHCP.

---
## 🔗 Connected Nodes
- [[TCP]] *(The connection-oriented counterpart)*
- [[QUIC Protocol]] *(The modern extension of UDP)*
