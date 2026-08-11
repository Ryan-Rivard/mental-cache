---
alias: [HTTP/1.1]
tags: [backend, networking, protocol]
created: 2026-08-11
status: clear
---

# HTTP 1.1 (1997)

The longest-running baseline version of the modern web.

## ⚙️ Core Architecture
- **Persistent Connections**: Uses `Connection: keep-alive` headers to reuse a single TCP connection for multiple sequential requests.
- **Pipelining**: Allowed clients to send multiple requests down the pipe before receiving responses (though poorly supported by browsers).

## ⚠️ The Bottleneck: Application HOL Blocking
- **Head-of-Line (HOL) Blocking**: Requests must be answered in the *exact order* they were requested. If the first image takes 5 seconds to load, all other assets behind it are completely blocked.
