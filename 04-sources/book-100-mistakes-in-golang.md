# 📖 Source: 100 Mistakes in Go (and How to Avoid Them)
- **Author:** Teiva Harsanyi
- **Status:** 📖 Reading
- **MOC Link:** [[backend-developer-roadmap-moc]]

## 📝 Raw Highlights & Notes

### Chapter 2: Code and Project Organization
- Mistake #1: Unintended variable shadowing. It happens when using `:=` in an inner block.
- *Code snippet captured:*
  ```go
  var client *http.Client
  if jsonShadow {
      client, err := net.LookupIP("...") // Explodes because client is shadowed locally
  }
  ```

### Chapter 5: Strings
- Strings in Go are immutable. Every time you concatenate strings using `+`, it allocates a completely new string in memory.
- **Solution:** Use `strings.Builder` for high-performance loops.

---
## 🔄 Knowledge Extraction Checklist
- [x] Extracted "String Mutability" concept into [[go-string-performance]] note.
- [ ] Extract variable shadowing rules into my main [[go]] language note.
