## Project 2: **Rate Limiter (Token Bucket Algorithm)**

### ✅ Goal

Create a standalone rate-limiting library or HTTP middleware using the **token bucket** algorithm.

---

### 📋 Requirements

* [ ] Implement token bucket with:

  * [ ] Refill rate (tokens/sec)
  * [ ] Capacity (max burst)
* [ ] Track clients by key (e.g., IP or user ID)
* [ ] Use `time.Ticker` or `time.After` to refill tokens
* [ ] If no tokens, deny the request or job
* [ ] Build a CLI simulation to stress test limiter

---

### 🌱 Optional Features

* [ ] HTTP middleware: limit access to API routes
* [ ] Different rates per user/route
* [ ] Redis-based shared limiter (cluster-safe)
* [ ] TTL cleanup of stale buckets
* [ ] Logging and metrics per IP/client

---
