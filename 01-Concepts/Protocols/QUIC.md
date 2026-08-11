---
alias: [QUIC Protocol, quic, quick-udp]
tags: [backend, fundamentals, networking, protocol]
created: 2026-08-11
status: master-node
---

# QUIC Protocol

QUIC (Quick UDP Internet Connections) is a modern transport protocol developed to replace TCP, solving basic hardware latency limits by running directly on top of [[UDP]].

---

## 🚀 Why QUIC Was Invented
While [[TCP]] and [[HTTP 2.0|HTTP 2.0]] allow multiple streams over one link, they suffer from **Transport-Layer Head-of-Line (HOL) Blocking**. If TCP loses a single packet, it pauses *every* parallel asset lane until retransmission occurs. QUIC runs over UDP to manage stream loss limits independently.

> [!failure] 🐢 Classic TCP Architecture
> - **Pipeline**: Uses a single shared connection lane.
> - **Behavior**: One dropped packet pauses the *entire* connection stream.
> - **Result**: **Severe Head-of-Line Blocking** (everything behind the dropped packet freezes).

> [!success] 🚀 Modern QUIC Architecture
> - **Pipeline**: Uses an independent multi-stream grid.
> - **Behavior**: One dropped packet *only* pauses its own isolated lane.
> - **Result**: **No Head-of-Line Blocking** (lanes 2, 3, and 4 keep downloading instantly).

---

## ⚙️ Core Performance Advantages

### 1. Zero Round-Trip Time Handshake (0-RTT)
- **Classic TCP + TLS**: Requires separate network back-and-forth roundtrips to connect and verify encryption keys.
- **QUIC Solution**: Fuses connection initialization and **TLS 1.3 security** parameters directly into the very first packet swap, dropping connection latency drastically.

### 2. Independent Multiplexed Streams
- Implements packet loss checking on an individual asset stream level.
- If packet data drops on an image stream, scripts or styling sheets loading on companion streams continue rendering unhindered.

### 3. Connection Migration
- Connections are identified by a unique **Connection ID token** instead of the changing device IP address.
- Allows your smartphone to swap from Home Wi-Fi to a Mobile LTE data network seamlessly without dropping active server downloads.

---
## 🔗 Connected Nodes
- [[UDP]] *(The foundation layer)*
- [[HTTP 3.0|HTTP 3.0]] *(The web application tier using QUIC)*
