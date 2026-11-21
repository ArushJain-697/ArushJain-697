# Arush Jain

CS @ IIIT Bangalore. Into systems, AI, infrastructure, and the rabbit holes that come with trying to build something.

Mostly backend and infra, plus the occasional thing that probably shouldn't work offline but does. Usually working on something, or thinking about what to build next.

## Stuff I've built

### [SAKSHI](https://github.com/ArushJain-697/namma-ai) · won Namma AI Hackathon 2026 (PS1: AI for Inclusive Education)

A tutor that runs on a Raspberry Pi 5 with the internet off. You give it a textbook passage and it writes a summary and a quiz, where every wrong option is a misconception students actually have. Pick one and it works out what you probably believe, explains why it's wrong, drops back to the simpler idea underneath, and keeps asking about it on later days until it's gone.

Under the hood it's GURU-0.6B (Qwen3-0.6B fine-tuned with LoRA) running 4-bit on ExecuTorch, Arm CPU only. There's a graph of 4,080 misconceptions, Bayesian diagnosis to pin down the belief, BKT to track what's actually learned, and FSRS-6 to schedule revision. Summary plus 3 questions takes 57.9 s on the Pi.

Built with Trishanu Mazumdar and Vishnu Suhas Chinta as Team Nucleus. We got felicitated at Bengaluru Tech Summit 2026 and took home ₹1,50,000.

### [Dwarpal](https://github.com/ArushJain-697/Dwarpal)

My own mini Cloudflare. It's a reverse proxy and WAF that sits in front of your backends and checks every request for SQLi, XSS, path traversal, command injection and SSRF before letting it through. It rate-limits with a Redis token bucket, streams to whichever backend is healthy, logs everything to Postgres, and has a dashboard where you can watch attacks get blocked live.

Node.js (raw `http`), Postgres, Redis, Docker Compose. Run `docker compose up` and go attack it from the browser.

### [OMEN](https://github.com/ArushJain-697/Offline-mesh-emergency-network)

A peer-to-peer mesh network in C that works with no router, no internet and no server. Laptops on the same Wi-Fi or a phone hotspot find each other and message each other, encrypted, and messages hop through other nodes to reach ones that are out of range.

UDP discovery, stop-and-wait ARQ (RDT 3.0), libsodium encryption, pthreads, Docker.

### [SEAM](https://github.com/ArushJain-697/SIH-2026) · Smart India Hackathon 2026 (NTRO, PS 26163)

A security assessment of a big open-source app that anyone can re-run and check for themselves. It pulls the source at a fixed commit, runs the app locally, scans seven areas, scores everything in code (CVSS 3.1/4.0, EPSS), and rebuilds two of the app's published vulnerabilities to prove the method works. CI regenerates the whole report on every push. The CVSS 4.0 calculator matches FIRST's reference on 2000 out of 2000 random vectors.

Node.js with zero deps, TypeScript Compiler API, React, GitHub Actions. [Live report](https://arushjain-697.github.io/SIH-2026/)

### [Sicari.works](https://sicari.works)

A role-based job board. It's self-hosted on an Azure VM with Nginx and PM2, Cloudflare in front, and GitHub Actions for CI/CD, plus audit logging, idempotency protection, timing-safe request signing and a fair bit of security hardening.

I mostly built it to figure out what production infra actually looks like outside tutorials.

## What I'm into

Backend, distributed systems, infra and DevOps, security, and getting ML to run on small devices.

## Stack

- **Backend:** Node.js · Express · Python · C
- **Data:** MySQL · PostgreSQL · Redis
- **ML / on-device:** PyTorch · LoRA (PEFT) · ExecuTorch · Raspberry Pi
- **Infra:** Azure VM · Nginx · Docker · PM2 · Cloudflare · GitHub Actions
- **Security:** JWT · bcrypt · audit logging · idempotency protection · input sanitization

## Find me

[LinkedIn](https://www.linkedin.com/in/arush-jain-42054a385/) · [Resume](https://github.com/ArushJain-697/ArushJain-697/raw/main/RESUME.pdf) · [Email](mailto:arushjain.work697@gmail.com)
