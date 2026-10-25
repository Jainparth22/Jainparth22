<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0F172A,45:1D4ED8,100:7C3AED&height=220&section=header&text=Parth%20Jain&fontSize=48&fontColor=FFFFFF&animation=fadeIn&fontAlignY=36&desc=Distributed%20Systems%20%7C%20High-Level%20Design%20%7C%20Applied%20Machine%20Learning&descAlignY=59&descSize=16" alt="Parth Jain Banner" width="100%" />

  <h3>Bridging Production-Grade Distributed Systems with Applied Machine Learning</h3>
  <p>
    <a href="https://www.linkedin.com/in/jainparth22"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
    <a href="mailto:parthjain0722@gmail.com"><img src="https://img.shields.io/badge/Email-Contact-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
    <a href="https://github.com/Jainparth22"><img src="https://img.shields.io/badge/GitHub-Jainparth22-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub" /></a>
    <a href="https://github.com/Jainparth22/hld-distributed-systems-portfolio"><img src="https://img.shields.io/badge/HLD%20Portfolio-Explore-6D28D9?style=flat-square&logo=buffer&logoColor=white" alt="HLD Portfolio" /></a>
    <img src="https://komarev.com/ghpvc/?username=Jainparth22&style=flat-square&color=2563EB" alt="Profile views" />
  </p>
</div>

---

### 💡 Engineering Philosophy

> **"Most students build for the happy path. I build for edge cases, race conditions, and partial failures."**

I am a final-year Computer Science student (**IIT Madras BS in Data Science** + **VIT Bhopal B.Tech CSE**) bridging advanced Machine Learning with production-grade backend systems. I do not just write CRUD APIs; I engineer resilient, scalable architectures that behave deterministically under real-world traffic, concurrency, and network partitions.

```text
┌────────────────────────────────────────────────────────────────────────────────────────┐
│                        PARTH JAIN — CORE ENGINEERING DUALITY                           │
├───────────────────────────────────────────┬────────────────────────────────────────────┤
│    DISTRIBUTED SYSTEMS & SYSTEM DESIGN    │       APPLIED MACHINE LEARNING & AI        │
├───────────────────────────────────────────┼────────────────────────────────────────────┤
│ • Lock-Free CAS State Machines (OCC)      │ • 3-Tier NLP Pipeline (FlashText ➔ BGE)   │
│ • Single-Flight Stampede Coroutine Locks  │ • 50% Inference RAM Savings (Singleton)    │
│ • Horizontal WebSocket Redis Pub/Sub Bus  │ • Multi-Agent RAG (RRF + Cross-Encoders)   │
│ • 5-Engine Distributed Rate Limiting      │ • 0.7508 MAP@3 Zero-Shot Logit Extraction │
│ • Hybrid Fan-Out & O(1) Cursor Feeds      │ • Edge Biosignal Streaming (SQLite WAL)    │
└───────────────────────────────────────────┴────────────────────────────────────────────┘
```

---

## ⚡ How I Approach Engineering

### 1. 🏛️ Architecture & Distributed Systems
I build decoupled, event-driven backends using a **modular monolith** approach. This avoids premature microservices complexity while maintaining strict separation of concerns and clear domain boundaries. By leveraging asynchronous message brokers (**Redis Pub/Sub**, **Celery**), I ensure compute-intensive background workloads and broadcast fans never block latency-sensitive core user flows.

### 2. 🔒 Concurrency & Data Integrity
I architect **lock-free Compare-And-Swap (CAS)** state machines with Optimistic Concurrency Control (OCC) to handle extreme contention. This eliminates **TOCTOU (Time-of-Check to Time-of-Use)** race conditions and completely prevents duplicate bookings, ensuring strict ACID compliance across concurrent threads without stalling the engine with heavy database table locks.

### 3. 🛡️ Production-Grade Resilience & Graceful Degradation
I build systems designed to survive partial infrastructure failures. If an async message broker, cache cluster, or downstream microservice drops, distributed rate-limiters, pub/sub channels, and task queues **automatically degrade to atomic in-memory synchronous execution**, ensuring zero user-facing 500 errors. I also engineer stateful JWT security pipelines with **JTI blacklisting** for instant cryptographic token revocation.

### 4. 🤗 Open Source & Applied AI (Hugging Face)
Contributed a production-grade semantic matching engine to **Hugging Face Spaces**. Optimized cold-start and runtime inference memory by **50%** through a shared global `SentenceTransformer` singleton, and engineered a hallucination-resistant **3-tier NLP pipeline** (`FlashText Taxonomy` ➔ `KeyBERT Dynamic Extraction` ➔ `BGE Embeddings`) to replace fragile regex heuristics.

### 5. 🔬 Rigorous ML Experimentation
I treat ML as an empirical science, not an arbitrary script. Achieved **0.7508 MAP@3** on a constrained STEM ranking dataset by rigorously proving that zero-shot LLM logit extraction outperforms parameter fine-tuning (preventing catastrophic overfitting on small samples), and deliberately rejected SMOTE on high-dimensional sparse matrices to preserve true geometric distribution.

---

## 📊 Engineering by the Numbers

<div align="center">

| Metric | Quantitative Achievement | Core Engineering Mechanism |
|:---:|:---|:---|
| **`0`** | **Race Conditions / Double-Bookings** | CAS versioning + 5-min ephemeral holds under 100 concurrent workers |
| **`970K+`** | **Historical Sales Records Processed** | Heterogeneous Gradient Boosting ensemble across 1,115 retail hubs |
| **`50%`** | **Inference Memory Reduction** | Shared global embedding model singleton on Hugging Face Spaces |
| **`0.7508`** | **MAP@3 STEM Benchmark** | Zero-shot logit scoring avoiding catastrophic overfitting |
| **`40%`** | **API Latency Reduction** | Redis cache-aside + asynchronous Celery offload |
| **`N-Node`**| **WebSocket Horizontal Scaling** | Redis Pub/Sub cluster backplane (`chat:rooms:*`) with failover |
| **`808+`** | **Data Structures & Algo Problems** | 942-day POTD streak, Institute Rank #23 on GeeksforGeeks |

</div>

---

## 🏛️ Distributed Systems & High-Level Design (HLD) Portfolio

> **Master Monorepo:** [hld-distributed-systems-portfolio](https://github.com/Jainparth22/hld-distributed-systems-portfolio) · Production-ready backend reference architectures featuring Docker Compose orchestration, automated concurrency suites, and strict resilience patterns.

<table>
  <thead>
    <tr>
      <th width="28%">System</th>
      <th width="48%">Core Distributed Architecture & Failure Modes Handled</th>
      <th width="24%">Standalone Repository</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><b>🔗 Distributed URL Shortener</b></td>
      <td>
        • Base62 bi-directional bijective encoding with collision probe offset<br>
        • High-throughput LRU cache with TTL + <b>Single-Flight coroutine lock</b> to eliminate cache stampedes on viral URLs<br>
        • Persistent SQLite/PostgreSQL transactional index<br>
        • Cryptographic JWT Bearer auth with asynchronous non-blocking analytics ingestion
      </td>
      <td><a href="https://github.com/Jainparth22/distributed-url-shortener"><b>distributed-url-shortener</b></a></td>
    </tr>
    <tr>
      <td><b>🚦 Distributed Rate Limiter</b></td>
      <td>
        • <b>5 Pluggable Algorithmic Engines:</b> Token Bucket, Leaky Bucket, Sliding Window Counter, Sliding Window Log, Fixed Window<br>
        • <b>Dual-Engine Tier:</b> Distributed Redis (<code>redis.asyncio</code>) with atomic in-memory CAS fallback<br>
        • Hot-key traffic detection dynamically sharded across virtual key slots<br>
        • Configurable <b>Fail-Open vs. Fail-Closed</b> operational modes
      </td>
      <td><a href="https://github.com/Jainparth22/distributed-rate-limiter"><b>distributed-rate-limiter</b></a></td>
    </tr>
    <tr>
      <td><b>💬 Scalable Real-Time Chat</b></td>
      <td>
        • Bidirectional persistent <b>WebSockets</b> with 30s heartbeat ping/pong<br>
        • <b>Horizontal Scale-Out:</b> Multi-node Redis Pub/Sub cluster backplane with auto-reconnect & local process fallback<br>
        • <b>Transactional Outbox Pattern</b> ensuring zero lost messages during network drops<br>
        • Monotonic 64-bit sequence counters + client reconnect replay buffer
      </td>
      <td><a href="https://github.com/Jainparth22/scalable-realtime-chat"><b>scalable-realtime-chat</b></a></td>
    </tr>
    <tr>
      <td><b>📰 Scalable News Feed Engine</b></td>
      <td>
        • <b>Hybrid Fan-Out Architecture:</b> Push (fan-out-on-write) for standard creators, Pull (fan-out-on-read) for high-follower celebrities<br>
        • Celebrity thresholding mitigating write amplification & queue backpressure<br>
        • Deterministic <b>O(1) cursor-based pagination</b> eliminating deep OFFSET query degradation<br>
        • Multi-factor engagement ranking algorithm with temporal exponential decay
      </td>
      <td><a href="https://github.com/Jainparth22/scalable-newsfeed-system"><b>scalable-newsfeed-system</b></a></td>
    </tr>
    <tr>
      <td><b>🎟️ High-Concurrency Ticket Booking</b></td>
      <td>
        • <b>Optimistic Concurrency Control (OCC CAS versioning)</b> with pessimistic row-locking fallback<br>
        • Two-phase reservation state machine with 5-minute expiring holds (zero TOCTOU race window)<br>
        • <b>Distributed Saga Orchestrator</b> executing automated compensating rollbacks upon payment drop<br>
        • Idempotent payment webhook receiver supporting Stripe & Razorpay payloads
      </td>
      <td><a href="https://github.com/Jainparth22/high-concurrency-ticket-booking"><b>high-concurrency-ticket-booking</b></a></td>
    </tr>
  </tbody>
</table>

---

## 🧠 Applied AI, Machine Learning & Intelligent Systems

### 1. Solari — Enterprise Demand Forecasting Engine
**[Repository](https://github.com/Jainparth22/Cerebal-ross-store-sales-problem)** · Python · FastAPI · LightGBM · XGBoost · Docker · GitHub Actions  
- Engineered a multi-hub quick-commerce demand forecasting engine on **970K+ historical retail records across 1,115 hubs**.
- Built a heterogeneous gradient boosting ensemble with year-over-year anchoring, reducing RMSE across high-variance promotional windows.
- Packaged with sub-50ms FastAPI batch and single-item inference endpoints, containerized with automated CI/CD.

### 2. MayaCardio — Biosignal Edge-to-Cloud Pipeline
**[Pipeline Source](https://github.com/Jainparth22/MayaCardio/tree/main/pipeline)** · Python · SQLite WAL · Flask · Supabase  
- Real-time biosensor streaming pipeline tailored for resource-constrained edge environments (Linux / Raspberry Pi).
- Durably writes concurrent telemetry into SQLite in **Write-Ahead Logging (WAL)** mode, calculating rolling-window signal statistics.
- Built-in gap/loss tracking with an offline store-and-forward queue that automatically synchronizes with cloud endpoints upon network restoration.

### 3. ResumeAnalyser — 3-Tier Semantic Matching Engine
**[Repository](https://github.com/Jainparth22/Resumeanalyser)** · Hugging Face Spaces · BGE Embeddings · KeyBERT · FlashText · RapidFuzz · Gradio  
- Built a hallucination-resistant resume-to-JD match engine deployed on Hugging Face Spaces.
- Combined exact skill taxonomy parsing (`FlashText`), dynamic candidate keyword extraction (`KeyBERT`), and dense contextual vector matching (`BGE`).
- Slashed runtime RAM by **50%** via a global singleton model instance with batched inference.

### 4. FinSight AI — Multi-Agent Financial Document Intelligence
**[Repository](https://github.com/Jainparth22/Langchain-Workshop)** · FastAPI · LangChain · LangGraph · FAISS · BM25 · Docker  
- Multi-agent agentic RAG workflow performing deep analysis and synthesis across complex corporate 10-K financial filings.
- Leveraged hybrid retrieval combining dense semantic embeddings with lexical **BM25**, unified via **Reciprocal Rank Fusion (RRF)** and cross-encoder reranking.
- Implemented human-in-the-loop review nodes, critique loops, and formal benchmark validation via **RAGAS**.

### 5. Smart MCQ Solver — Top-3 Ranking Engine
**[Repository](https://github.com/Jainparth22/SmartMCQsolver)** · PyTorch · Transformers · RoBERTa · BiLSTM · LightGBM · WandB  
- STEM multiple-choice ranking system achieving a **0.75084 MAP@3** benchmark score.
- Demonstrated that zero-shot LLM logit extraction outperformed fine-tuning by avoiding catastrophic parameter drift on small training partitions.
- Ensembled RoBERTa contextual logits with BiLSTM attention layers and LightGBM relative-rank meta-features.

### 6. Toxic Comment Multi-Label Pipeline
**[Repository](https://github.com/Jainparth22/MLtextclassificationpipeline)** · Python · scikit-learn · LinearSVC · Ensembles  
- High-throughput text categorization pipeline on a 200K-row dataset with severe label imbalance.
- Achieved **0.826 Macro F1** (Top 150 of 600+ teams) through character/word n-gram TF-IDF representations and cost-sensitive loss calibration, deliberately rejecting SMOTE to preserve sparse vector geometry.

---

## 💼 Full-Stack SaaS & Production Applications

### 1. Placement Portal Application (PPA)
**[Repository](https://github.com/Jainparth22/PlacementPortalApp)** · [Live Demo](https://ppa-v5.fly.dev) · Flask · Vue 3 · SQLAlchemy · Redis · Celery · JWT  
- Full-lifecycle campus hiring platform managing student applicants, corporate recruiters, and placement officers across **40+ REST endpoints**.
- Integrated Redis cache-aside and asynchronous Celery workers for PDF resume parsing and scheduled email delivery, cutting API response latency by **40%**.
- Enforced role-based access control (RBAC), tenant isolation, and atomic transactional state transitions for job drives.

### 2. InventoryPro — Modern Inventory SaaS
**[Repository](https://github.com/Jainparth22/Inventory-app)** · [Live Demo](https://inventory-parth.vercel.app) · Next.js · React · TypeScript · Prisma · PostgreSQL · Recharts  
- Production inventory tracking platform built with the Next.js App Router, Prisma ORM, and PostgreSQL.
- Implemented real-time stock-level analytics, automated reorder notifications, JOSE-secured JWT authentication, and responsive dashboards.

### 3. Healthcare Appointment & Follow-Up Manager
**[Repository](https://github.com/Jainparth22/Healthcare-Appointment-Follow-up-Manager)** · [Live Demo](https://hcv-parth.up.railway.app/) · FastAPI · SQLAlchemy · Alembic · Redis · Celery · Gemini  
- Clinic workflow system handling appointment slot reservations, medical history intake, and automated patient follow-ups.
- Implemented double-booking race condition prevention and graceful fallback behavior when third-party notification services experience downtime.

<details>
  <summary><b>📂 Additional Production Applications & System Scaffolds (Click to expand)</b></summary>
  <br>

  - **[Vehicle Parking App](https://github.com/Jainparth22/Vehicle-Parking-App-VPA)** — Flask REST API, Vue 3, SQLAlchemy, Redis, Celery; parking space reservation, automated hourly billing, analytics, and scheduled reporting.
  - **[A–Z Household Services](https://github.com/Jainparth22/Household-Services-Application-HSA)** — Multi-tenant service marketplace with customer, technician, and admin roles, background invoice generation, and provider approval workflows.
  - **[Hospital Management System](https://github.com/Jainparth22/Hospital-Management-App-HMA)** — Comprehensive clinical platform with doctor availability scheduling, patient consultation history, and treatment logs.
  - **[CampusCart](https://github.com/Jainparth22/Campus-Cart)** — Hyperlocal campus grocery and printing service platform with order tracking, inventory validation, and fulfillment workflows.
  - **[Phishing URL Scanner](https://github.com/Jainparth22/MLworkshopProj)** — Heuristic URL structure parsing combined with scikit-learn models for real-time malicious domain detection.
  - **[Job Attrition Rate AI (JAR)](https://github.com/Jainparth22/JAR)** — Research prototype combining VAE representations, Transformer feature interactions, LightGBM, and Dueling DDQN reinforcement learning.
  - **[FastAPI Coursework](https://github.com/Jainparth22/FastAPI-Coursework)** — Comprehensive architectural patterns for modern asynchronous Python APIs, Pydantic v2 schemas, and dependency injection.
  - **[System Design Notes & Diagrams](https://github.com/Jainparth22/ION_interview_helpful)** — Curated technical breakdowns and flowcharts covering Redis caching architectures, Instagram Reels feeds, and ride-sharing dispatch engines.
</details>

---

## 🛠️ Technology Stack

<table>
  <tr>
    <td width="25%"><b>Backend & Distributed</b></td>
    <td>
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
      <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" />
      <img src="https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white" />
      <img src="https://img.shields.io/badge/WebSockets-010101?style=flat-square&logo=socketdotio&logoColor=white" />
      <img src="https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white" />
      <img src="https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat-square" />
      <img src="https://img.shields.io/badge/Pydantic-E92063?style=flat-square" />
      <img src="https://img.shields.io/badge/JWT_Auth-000000?style=flat-square&logo=jsonwebtokens&logoColor=white" />
    </td>
  </tr>
  <tr>
    <td><b>Databases & Caching</b></td>
    <td>
      <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
      <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" />
      <img src="https://img.shields.io/badge/SQLite_WAL-003B57?style=flat-square&logo=sqlite&logoColor=white" />
      <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" />
      <img src="https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white" />
      <img src="https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white" />
    </td>
  </tr>
  <tr>
    <td><b>Machine Learning & Data</b></td>
    <td>
      <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" />
      <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" />
      <img src="https://img.shields.io/badge/LightGBM-2E8B57?style=flat-square" />
      <img src="https://img.shields.io/badge/XGBoost-EC6B23?style=flat-square" />
      <img src="https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white" />
      <img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white" />
      <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white" />
      <img src="https://img.shields.io/badge/Weights_%26_Biases-FFBE00?style=flat-square&logo=weightsandbiases&logoColor=black" />
    </td>
  </tr>
  <tr>
    <td><b>NLP & Generative AI</b></td>
    <td>
      <img src="https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black" />
      <img src="https://img.shields.io/badge/Sentence_Transformers-4F46E5?style=flat-square" />
      <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square" />
      <img src="https://img.shields.io/badge/LangGraph-6B4FBB?style=flat-square" />
      <img src="https://img.shields.io/badge/FAISS_VectorDB-2563EB?style=flat-square" />
      <img src="https://img.shields.io/badge/BM25_Lexical-0F766E?style=flat-square" />
      <img src="https://img.shields.io/badge/FlashText-2563EB?style=flat-square" />
      <img src="https://img.shields.io/badge/KeyBERT-5B21B6?style=flat-square" />
      <img src="https://img.shields.io/badge/RAGAS_Eval-EF6C57?style=flat-square" />
    </td>
  </tr>
  <tr>
    <td><b>DevOps & Infrastructure</b></td>
    <td>
      <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
      <img src="https://img.shields.io/badge/Docker_Compose-2496ED?style=flat-square&logo=docker&logoColor=white" />
      <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" />
      <img src="https://img.shields.io/badge/Linux_Ubuntu-FCC624?style=flat-square&logo=linux&logoColor=black" />
      <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white" />
      <img src="https://img.shields.io/badge/Fly.io-4638E2?style=flat-square&logo=flydotio&logoColor=white" />
      <img src="https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white" />
      <img src="https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white" />
    </td>
  </tr>
  <tr>
    <td><b>Frontend & UI</b></td>
    <td>
      <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" />
      <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" />
      <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
      <img src="https://img.shields.io/badge/Vue.js_3-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white" />
      <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" />
      <img src="https://img.shields.io/badge/Gradio-F97316?style=flat-square" />
    </td>
  </tr>
</table>

---

## 🎓 Education & Credentials

| Institution | Degree / Programme | Timeline |
|:---|:---|:---:|
| **Indian Institute of Technology Madras (IIT Madras)** | BS in Data Science and Applications | May 2023 – May 2027 *(Expected)* |
| **Vellore Institute of Technology (VIT Bhopal)** | B.Tech in Computer Science and Engineering | 2023 – June 2027 *(Expected)* |

*Pursuing both degree programmes concurrently with focus on Distributed Systems, Advanced Machine Learning, and Algorithms.*

### Verified Certifications & Digital Badges

- **IIT Madras BS Programme:** Diploma in Data Science (Completed May 2026 term) · *NLP with Transformers using Hugging Face* · *ML in Production*
- **NPTEL / SWAYAM (Elite):** Marketing Analytics (**Elite, 94%** — IIT Kharagpur) · Introduction to Machine Learning (**Elite, 62%** — IIT Madras)
- **DeepLearning.AI / Stanford Online:** Supervised Machine Learning: Regression and Classification ([Verify 71DAGQ41QNHW](https://coursera.org/verify/71DAGQ41QNHW))
- **Duke University:** Introduction to FastAPI Framework ([Verify SFO87EQ4XDCW](https://coursera.org/verify/SFO87EQ4XDCW))
- **AWS Educate:** Databases · Networking · Serverless · Storage
- **ServiceNow:** Administration Fundamentals On Demand · Academic Partnerships Participant

---

## 📈 Activity & GitHub Metrics

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=Jainparth22&show_icons=true&hide_border=true&theme=transparent&rank_icon=github" alt="GitHub stats" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Jainparth22&layout=compact&hide_border=true&theme=transparent&langs_count=8" alt="Top languages" />
</p>
<p align="center">
  <img src="https://streak-stats.demolab.com?user=Jainparth22&hide_border=true&theme=transparent" alt="GitHub contribution streak" />
</p>

---

## 🤝 Let's Connect

I am actively looking for **Software Development Engineer (SDE)**, **Backend Engineer**, or **AI Infrastructure** roles at engineering-first companies that value system design, concurrency control, and production reliability over tutorial-following.

If you are building systems that need to scale, handle extreme concurrency without data corruption, or deploy Machine Learning models reliably into production, let's talk:

- **LinkedIn:** [linkedin.com/in/jainparth22](https://www.linkedin.com/in/jainparth22)
- **Email:** [parthjain0722@gmail.com](mailto:parthjain0722@gmail.com)
- **GitHub:** [github.com/Jainparth22](https://github.com/Jainparth22)
- **Master HLD Portfolio:** [hld-distributed-systems-portfolio](https://github.com/Jainparth22/hld-distributed-systems-portfolio)

<div align="center">
  <sub>Engineered for edge cases, race conditions, and graceful degradation • Built by Parth Jain</sub>
</div>
