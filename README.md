Perfect — here's a **README-style specification** for each of the three projects. These are structured to help you **scope, implement, and extend** them incrementally.

---

# 📦 Go Projects README

## Project 1: **Job Queue (In-Memory Worker Pool)**

### ✅ Goal

Build a simple job queue system in Go that accepts jobs (simulated tasks) and distributes them to a fixed-size worker pool.

---

### 📋 Requirements

* [ ] Define a `Job` struct (ID, payload, retry count, timestamp)
* [ ] Create a buffered job queue (`chan Job`)
* [ ] Spawn N worker goroutines to listen to the queue
* [ ] Simulate processing time (e.g., with `time.Sleep`)
* [ ] Log when a job starts and finishes
* [ ] Handle failed jobs with retries (exponential backoff)
* [ ] Cancel jobs gracefully with `context.Context`
* [ ] Allow enqueueing new jobs from:

  * [ ] CLI or
  * [ ] HTTP `/enqueue` endpoint (optional)

---

### 🌱 Optional Features

* [ ] Job priority (high vs low priority jobs)
* [ ] Persist jobs to disk (JSON file or SQLite)
* [ ] Admin API: view queue length, active jobs
* [ ] Metrics (processed, failed, retry count)
