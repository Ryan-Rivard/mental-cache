---
alias: [HTTP/3, HTTP 3]
tags: [backend, networking, protocol]
created: 2026-08-11
status: clear
---

# HTTP 3.0 (2022)

The modern standard designed for unreliable global wireless connections.

## ⚙️ Core Architecture
- **QUIC Migration**: Built on top of [[UDP]] via the **QUIC** protocol, bypassing classic TCP limitations.
- **Stream Independence**: True non-blocking concurrency. A dropped packet on stream A has **zero impact** on stream B, C, or D.
- **0-RTT Handshakes**: Combines encryption handshakes (TLS 1.3) directly into the initial network connection request.

---
## 🔗 Related Advanced Concepts
- [[QUIC| QUIC Protocol]]
- [[UDP]]
