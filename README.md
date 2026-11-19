# Parth Jain

Backend and ML engineer. B.Tech CSE at VIT Bhopal and BS Data Science at IIT Madras, studied side by side. Final year.

**Portfolio:** [porfoliosample-zeta.vercel.app](https://porfoliosample-zeta.vercel.app/)  |  [LinkedIn](https://www.linkedin.com/in/jainparth22)  |  [Email](mailto:parthjain0722@gmail.com)

> Most students build for the happy path. I build for edge cases, race conditions, and partial failures.

I build backend services that stay correct under concurrency and keep running when a dependency fails, and ML systems whose results I can defend with an experiment log. I am looking for SDE, backend, or ML-focused engineering roles at teams that care about system design and reliability.

## Live projects

| Project | What it is | Stack | Links |
|---|---|---|---|
| **Placement Portal** | Campus hiring platform for students, recruiters and admins. 53 documented REST endpoints, stateful JWT logout (JTI blacklist), Redis caching, Celery jobs, and fallbacks at every dependency. | Flask, Vue 3, SQLAlchemy, Redis, Celery | [Code](https://github.com/Jainparth22/PlacementPortalApp) / [Live](https://ppa-v5.fly.dev) |
| **Healthcare Appointment Manager** | Clinic booking where two patients cannot take the same slot (compare-and-set holds, idempotency keys, race tests). Gemini triage and summaries with a deterministic fallback, email outbox, Google Calendar sync. | FastAPI, PostgreSQL, Redis, Celery, Docker | [Code](https://github.com/Jainparth22/Healthcare-Appointment-Follow-up-Manager) / [Live](https://hcv-parth.up.railway.app/) |
| **InventoryPro** | Inventory SaaS where stock changes only through valid order-state transitions. Edge-verified JWT, Recharts dashboards, PWA. | Next.js, TypeScript, Prisma, PostgreSQL | [Code](https://github.com/Jainparth22/Inventory-app) / [Live](https://inventory-parth.vercel.app) |

## Machine learning

| Project | Result |
|---|---|
| [Smart MCQ Solver](https://github.com/Jainparth22/SmartMCQsolver) | 0.75084 MAP@3 (Kaggle private) on a 2,000-row STEM dataset. Fine-tuning lost to zero-shot LLM logit scoring, and the repo documents all 16 approaches. |
| [FinSight AI](https://github.com/Jainparth22/Langchain-Workshop) | Multi-agent RAG over financial documents: LangGraph, BM25 plus FAISS with rank fusion, cross-encoder reranking, guardrails, RAGAS evaluation. |
| [Toxic comment classifier](https://github.com/Jainparth22/MLtextclassificationpipeline) | 0.826 Macro F1, top ~150 of 600+ teams, classical ML only. Stacking beat voting; SMOTE tested and rejected. |
| [Solari demand forecasting](https://github.com/Jainparth22/Cerebal-ross-store-sales-problem) | 970K rows, 1,115 hubs, LightGBM, XGBoost and CatBoost behind a FastAPI service with CI. |
| Hugging Face semantic matcher | FlashText, KeyBERT and BGE embeddings in tiers; 50% lower inference memory with one shared model instance. |

## System design

[hld-distributed-systems-portfolio](https://github.com/Jainparth22/hld-distributed-systems-portfolio) holds five runnable services, each also its own repo.

| Service | Pattern |
|---|---|
| [URL shortener](https://github.com/Jainparth22/distributed-url-shortener) | Base62 codes, LRU cache with single-flight, JWT |
| [Rate limiter](https://github.com/Jainparth22/distributed-rate-limiter) | Five algorithms, Redis or in-memory, fail-open or fail-closed |
| [Real-time chat](https://github.com/Jainparth22/scalable-realtime-chat) | WebSockets, Redis Pub/Sub backplane, transactional outbox |
| [News feed](https://github.com/Jainparth22/scalable-newsfeed-system) | Push, pull and hybrid fan-out, cursor pagination |
| [Ticket booking](https://github.com/Jainparth22/high-concurrency-ticket-booking) | Optimistic locking, expiring holds, saga with compensation |

These run locally; payments and some storage are simulated, and the READMEs say so.

## How I work

- **Concurrency.** Compare-and-set state changes and idempotency keys instead of heavy table locks.
- **Resilience.** If Redis, a queue or an LLM is down, the core flow degrades to a simpler path instead of failing.
- **Experiments.** I keep negative results, because they usually explain the final number.
- **Documentation.** Design notes and READMEs state what is simulated and what is production.

## Stack

- **Languages:** Python, C++, C, Java, TypeScript, JavaScript, SQL
- **Backend:** FastAPI, Flask, SQLAlchemy, Celery, Redis, PostgreSQL, SQLite, JWT, WebSockets
- **ML and AI:** PyTorch, scikit-learn, LightGBM, XGBoost, Hugging Face, Sentence-Transformers, LangChain, LangGraph, FAISS, Weights & Biases
- **Tools:** Git, Docker, Linux, GitHub Actions, Vercel, Railway, Fly.io

## Education and credentials

- B.Tech CSE, VIT Bhopal (expected 2027)
- BS Data Science and Applications, IIT Madras (expected 2027): Diploma in Programming, Diploma in Data Science, two advanced certificates
- NPTEL Elite certificates (Machine Learning, Marketing Analytics), HackerRank SQL (Advanced), Coursera Supervised ML, AWS Educate badges
- MPOnline (Govt. of MP and TCS JV) AI/ML and software engineering internship, May to Jul 2026
- 950+ day GeeksforGeeks streak, 200+ LeetCode problems

## Coding streaks

<p align="center">
  <img src="https://streak-stats.demolab.com?user=Jainparth22&hide_border=true&theme=default" alt="GitHub streak" height="170" />
</p>

<p align="center">
  <a href="https://leetcode.com/u/jain22parth/"><img src="https://leetcard.jacoblin.cool/jain22parth?theme=light&font=Karma&ext=heatmap" alt="LeetCode stats and heatmap" width="520" /></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/GeeksforGeeks-950%2B%20day%20streak-2F8D46?style=for-the-badge" alt="GeeksforGeeks 950+ day streak" />
</p>

## Contact

[parthjain0722@gmail.com](mailto:parthjain0722@gmail.com)  |  [LinkedIn](https://www.linkedin.com/in/jainparth22)  |  [Portfolio](https://porfoliosample-zeta.vercel.app/)
