# Arush Jain

CSE @ IIIT Bangalore.
I build backend systems, infrastructure-heavy projects, and occasionally things that should probably not work offline.

## What I've Built

### [SAKSHI](https://github.com/ArushJain-697/namma-ai) · Winner, Namma AI Hackathon 2026 (PS1: AI for Inclusive Education)

Offline tutor on a Raspberry Pi 5. Give it a textbook passage and it writes a summary and a quiz where every wrong option is a known student misconception. When a student picks one, it works out which belief they probably hold, explains the fix, steps down to the prerequisite idea, and brings the belief back on later days until it's gone.

GURU-0.6B (Qwen3-0.6B + LoRA) on ExecuTorch, 4-bit, Arm CPU only, network off. Misconception graph of 4,080 beliefs. Bayesian diagnosis, BKT knowledge tracing, FSRS-6 spaced revision. Summary + 3 questions in 57.9 s on the Pi.

Team Nucleus with Trishanu Mazumdar and Vishnu Suhas Chinta. Felicitated at Bengaluru Tech Summit 2026, ₹1,50,000 prize.

---

### [Dwarpal](https://github.com/ArushJain-697/Dwarpal)

Self-hosted reverse proxy and web application firewall. Every request goes through an ordered pipeline of stages that check for SQLi, XSS, path traversal, command injection and SSRF, rate-limit abusers with a Redis token bucket, and stream to a healthy upstream without buffering the body. Logs go to day-partitioned Postgres, and a React dashboard shows attacks live over WebSocket.

Node.js (raw `http`) · PostgreSQL · Redis · Docker Compose. `docker compose up` and attack it from the browser.

---

### [OMEN](https://github.com/ArushJain-697/Offline-mesh-emergency-network)

Fully offline peer-to-peer mesh network written in C.

Custom UDP node discovery, RDT 3.0 stop-and-wait ARQ, libsodium authenticated encryption, POSIX threads, Dockerized.

No router. No internet. No central server.

---

### [SEAM](https://github.com/ArushJain-697/SIH-2026) · Smart India Hackathon 2026 (NTRO, PS 26163)

Re-runnable security assessment of an open-source app. Pins the source, runs it locally, scans seven scope areas, scores findings in code (CVSS 3.1/4.0, EPSS), reproduces published advisories as vulnerable/patched lab pairs, and publishes the report from CI on every push. The CVSS 4.0 calculator matches FIRST's reference on 2000/2000 random vectors.

Node.js (zero deps) · TypeScript Compiler API · React · GitHub Actions. [Live report](https://arushjain-697.github.io/SIH-2026/)

---

### [Sicari.works](https://sicari.works)

Role-based job board and backend system built solo.

Self hosted on Azure VM with Nginx, PM2, Cloudflare proxying, GitHub Actions CI/CD, audit logging, idempotency protection, timing-safe request signing, and production security hardening.

Built mainly to understand what production infrastructure actually looks like outside tutorials.

---

## Interests

* Backend engineering
* Distributed systems
* Infrastructure / DevOps
* Cybersecurity
* On-device ML

## Stack

**Backend**
Node.js · Express · Python · C

**Data**
MySQL · PostgreSQL · Redis

**ML / on-device**
PyTorch · LoRA (PEFT) · ExecuTorch · Raspberry Pi

**Infrastructure**
Azure VM · Nginx · Docker · PM2 · Cloudflare · GitHub Actions

**Security**
JWT · bcrypt · audit logging · idempotency protection · input sanitization

## Elsewhere

[LinkedIn](https://www.linkedin.com/in/arush-jain-42054a385/) · [Resume](https://github.com/ArushJain-697/ArushJain-697/raw/main/RESUME.pdf) · [Email](mailto:arushjain.work697@gmail.com)
