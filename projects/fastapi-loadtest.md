---
layout: post
title: FastAPI Under Load — From Prototype to Kubernetes
date: 2025-07-27
---

[🔗 View the full project on GitHub](https://github.com/kgadgil/backend-lab)

---

This weekend, I explored how a simple FastAPI notes app evolves into a production-ready, scalable system capable of handling real-world traffic. What started as a local SQLite prototype transformed into a secure, containerized, and load-tested web service running on Kubernetes.

### 💡 Project Goals

- Build a simple FastAPI app with user authentication and note-taking
- Start with SQLite for rapid prototyping
- Replace SQLite with PostgreSQL for concurrency and durability
- Containerize the app using Docker for reproducibility
- Deploy to Kubernetes for scalability and fault tolerance
- Simulate real-world load (many users registering, logging in, writing notes)
- Document key architectural decisions throughout

### 🧱 Design Highlights

- **FastAPI**: Chosen for its async-first design, excellent developer experience, and speed
- **SQLite**: Used initially for its simplicity in the prototype stage
- **PostgreSQL**: Swapped in for better concurrency handling under load
- **SQLAlchemy + Pydantic**: Powerful ORM + validation combo
- **Docker**: Ensures consistency across environments
- **Kubernetes**: Enables orchestration, auto-scaling, and resilience

Design decisions are documented in detail in the [`docs/`](https://github.com/kgadgil/backend-lab/tree/main/doc/adr) folder using ADRs (Architectural Decision Records).

### 🔬 Load Testing Results

- With SQLite, the app crashes under a flood of concurrent requests (10,000+) due to connection timeouts
- Switching to PostgreSQL stabilized the app under pressure
- More detailed load test metrics and automation scripts are in progress (see [TODOs in README](https://github.com/kgadgil/backend-lab))

### 🧠 Reflections

This project helped me understand where quick prototypes start to break down — and how to scale thoughtfully. From database selection to containerization to orchestration, each step was a deliberate decision in building toward production readiness.

---

**Keywords**: FastAPI, SQLAlchemy, Pydantic, SQLite, PostgreSQL, Docker, Kubernetes, Load Testing, Authentication
