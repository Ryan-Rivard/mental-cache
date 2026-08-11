---
alias: [HTTP/2, HTTP 2]
tags: [backend, networking, protocol]
created: 2026-08-11
status: clear
---

# HTTP 2.0 (2015)

A major rewrite focused heavily on frontend asset load performance.

## ⚙️ Core Architecture
- **Binary Framing Layer**: Converts plain text commands into compact binary data frames.
- **Multiplexing**: Interleaves requests and responses simultaneously down a **single** active [[TCP| TCP]]  connection.
- **Header Compression (HPACK)**: Shrank redundant metadata sizes to save bandwidth.

## ⚠️ The Bottleneck: Transport HOL Blocking
- **TCP Vulnerability**: Because it still uses TCP, if an internet router drops a single packet, TCP pauses *all* active concurrent streams while waiting for retransmission.
