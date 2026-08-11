---
alias: [HTTP Protocol Versions, web protocols]
tags: [backend, fundamentals, networking, concept]
created: 2026-08-11
status: master-node
---

# HTTP Evolution

The Hypertext Transfer Protocol has evolved from a simple text-based protocol into a highly optimized, binary transport stream. Each iteration directly solved the performance bottlenecks of its predecessor.

## 📊 Quick Comparison

| Version                 | Transport Protocol | Format | Connection Architecture           | Head-of-Line Blocking     |
| :---------------------- | :----------------- | :----- | :-------------------------------- | :------------------------ |
| [[HTTP 1.0\| HTTP 1.0]] | TCP                | Text   | 1 Connection per Request          | Severe                    |
| [[HTTP 1.1\| HTTP 1.1]] | TCP                | Text   | Persistent (Sequential)           | Application-Layer HOLB    |
| [[HTTP 2.0\| HTTP 2.0]] | TCP                | Binary | Multiplexed (Single Connection)   | Transport-Layer HOLB      |
| [[HTTP 3.0\| HTTP 3.0]] | QUIC (over UDP)    | Binary | Multiplexed (Independent Streams) | **Completely Eliminated** |

---

## 🔍 Key Performance Milestones

### 1. Persistent Connections
- Introduced in [[HTTP 1.1|HTTP 1.1]].
- Kept the underlying TCP handshake alive across multiple requests to eliminate connection overhead.

### 2. Multiplexing
- Introduced in [[HTTP 2.0|HTTP 2.0]].
- Allowed bidirectional interleaved streaming of data segments, cutting out queue lines.

### 3. QUIC & UDP Migration
- Introduced in [[HTTP 3.0|HTTP 3.0]].
- Abandoned TCP entirely to resolve connection drop-freezes at the hardware level.

---
## 🔗 Parent Hub
- [[HTTP]]
