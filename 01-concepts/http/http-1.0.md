---
alias: [HTTP/1.0, HTTP 1]
tags: [backend, networking, history]
created: 2026-08-11
status: clear
---

# HTTP 1.0 (1996)

The foundational implementation of the modern web protocol. 

## ⚙️ Core Architecture
- **Short-Lived Connections**: Every asset exchange required opening a completely fresh TCP connection connection.
- **Cycle**: Client Connection ➡️ Request ➡️ Response ➡️ Connection Closed.

## ⚠️ The Bottleneck
- **High Overhead**: Heavy processing and latency costs from performing repeated TCP 3-way handshakes for every minor image or file on a page.
