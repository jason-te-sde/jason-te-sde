<!-- ============ Header banner (animated gradient wave) ============ -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:8E2DE2,100:4A00E0&height=220&section=header&text=Jason%20Te&fontSize=80&fontColor=ffffff&fontAlignY=36&desc=Software%20Engineer%20%C2%B7%20Distributed%20Systems%20%C2%B7%20AI%20Engineering&descSize=18&descAlignY=58&animation=fadeIn" width="100%"/>
</p>

<!-- ============ Typing animation subtitle ============ -->
<p align="center">
  <a href="https://github.com/jason-te-sde">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=8E2DE2&center=true&vCenter=true&width=640&lines=Distributed+systems+you+can+crash-test;AI+systems+measured%2C+not+demoed;M.S.+CS+%40+Northeastern%2C+May+2027" alt="Typing SVG"/>
  </a>
</p>

<!-- ============ Contact badges ============ -->
<p align="center">
  <a href="mailto:jason.te.sde@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://www.linkedin.com/in/jason-te-sde"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="https://github.com/jason-te-sde"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
  <img src="https://komarev.com/ghpvc/?username=jason-te-sde&style=for-the-badge&color=8E2DE2" alt="profile views"/>
</p>

---

## 🧑‍💻 About Me

I build systems whose claims can be checked: every number below links to the test, benchmark or
committed run that produced it.

- 🎓 M.S. in Computer Science at Northeastern University (Seattle), graduating May 2027
- 🔭 Looking for new-grad roles in backend, distributed systems and AI engineering
- 📫 [jason.te.sde@gmail.com](mailto:jason.te.sde@gmail.com) · [portfolio](https://jason-te.vercel.app)

---

## 🧱 Distributed systems and storage

| Project | What it is | A number you can check |
| --- | --- | --- |
| [**till**](https://github.com/jason-te-sde/till) | Full-stack game store on AWS: React, Spring Boot, Kafka through a transactional outbox, Aurora, Terraform on ECS Fargate | 8,000 concurrent shoppers at a **p99 of 134 ms**, down from 20.8 s, one measured bottleneck at a time |
| [**keel**](https://github.com/jason-te-sde/keel) | Linearizable key-value store in Java: Raft from scratch, a deterministic fault-injection simulator, a linearizability checker | **3 safety violations** a 10,000-seed simulation sweep found that hand-written tests could not reach ([seeds 1695, 1537, 2626](https://github.com/jason-te-sde/keel#bugs-the-tests-found)) |
| [**shale**](https://github.com/jason-te-sde/shale) | Crash-safe LSM-tree storage engine in C++20 with no third-party runtime dependency | **200 rounds of a real `kill -9`** in CI; writes level with LevelDB ([0.98 to 0.99 of its ops/s](https://github.com/jason-te-sde/shale/blob/main/docs/benchmarks.md)) |
| [**quarry**](https://github.com/jason-te-sde/quarry) | Vectorized SQL query engine in C++20 over Apache Arrow and Parquet, every result checked against DuckDB | A join-estimate fix took Q5 from **4,730 ms to 590.5 ms**; it still takes [3.57× to 6.29× the time of single-threaded DuckDB](https://github.com/jason-te-sde/quarry#measured-numbers), and the README says so first |
| [**distributed-job-queue**](https://github.com/jason-te-sde/distributed-job-queue) | Job queue for Go services on PostgreSQL: leased at-least-once delivery, fencing tokens, weighted fair scheduling | **3,781 jobs/s** on one broker; under a 100,000-job flood a small tenant waits 18 ms at p99 instead of 28.5 s |
| [**CollabDocs**](https://github.com/jason-te-sde/collabdocs) | Real-time collaborative editor: Yjs CRDT over Socket.IO, TipTap, PostgreSQL, Redis between instances, and a role check on every route and socket event | Sync latency **p95 6.7 ms** at 50 editors on one document, one in five typing ([worst of 3 runs, one machine, loopback](https://github.com/jason-te-sde/collabdocs#performance)) |

## 🤖 AI engineering

| Project | What it is | A number you can check |
| --- | --- | --- |
| [**arxiv-research-agent**](https://github.com/jason-te-sde/arxiv-research-agent) | ReAct research agent over arXiv: two-stage retrieval, citations checked against the retrieved passages, streamed over FastAPI | Reranking adds **0.164 MRR@5** (95% interval +0.039 to +0.297); [every run committed](https://github.com/jason-te-sde/arxiv-research-agent/tree/main/eval/runs) |
| [**timeseriesguard**](https://github.com/jason-te-sde/timeseriesguard) | Anomaly detection on the Server Machine Dataset, with leakage guards the code enforces | **0.70 event-level AUC-PR**, under a protocol where random scores get 0.04 (point adjust would give them an F1 of 0.77) |
| [**nano-claude-code**](https://github.com/jason-te-sde/nano-claude-code) | Terminal coding agent for Anthropic, OpenAI-compatible and local models, with a model per role | An **MCP client** that pins every tool definition and asks again when one changes; a read-only explore sub-agent on its own model; 4,955 tests |
| [**cairn**](https://github.com/jason-te-sde/cairn) | Deterministic ML model registry in Java: immutable versions, content-addressed artifacts | **12 invariants** checked after every step of a seeded simulation |

---

## 🛠️ Tech Stack

**Languages**
<p>
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java"/>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript"/>
  <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" alt="C++"/>
  <img src="https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=black" alt="C"/>
  <img src="https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white" alt="Bash"/>
</p>

**Backend & API**
<p>
  <img src="https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white" alt="Spring"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI"/>
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js"/>
  <img src="https://img.shields.io/badge/WebSocket-010101?style=for-the-badge&logo=socketdotio&logoColor=white" alt="WebSocket"/>
  <img src="https://img.shields.io/badge/Apache%20Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white" alt="Kafka"/>
  <img src="https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white" alt="Maven"/>
  <img src="https://img.shields.io/badge/Gradle-02303A?style=for-the-badge&logo=gradle&logoColor=white" alt="Gradle"/>
</p>

**Frontend**
<p>
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React"/>
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5"/>
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3"/>
</p>

**AI / ML**
<p>
  <img src="https://img.shields.io/badge/Anthropic%20Claude-191919?style=for-the-badge&logo=anthropic&logoColor=white" alt="Anthropic Claude"/>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="PyTorch"/>
  <img src="https://img.shields.io/badge/Hugging%20Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black" alt="Hugging Face"/>
  <img src="https://img.shields.io/badge/ChromaDB-FF6F61?style=for-the-badge&logo=databricks&logoColor=white" alt="ChromaDB"/>
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy"/>
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas"/>
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter"/>
</p>

**Databases**
<p>
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL"/>
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" alt="Redis"/>
</p>

**Cloud & DevOps**
<p>
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white" alt="AWS"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker"/>
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" alt="Kubernetes"/>
  <img src="https://img.shields.io/badge/Helm-0F1689?style=for-the-badge&logo=helm&logoColor=white" alt="Helm"/>
  <img src="https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white" alt="Nginx"/>
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" alt="Linux"/>
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git"/>
</p>

**Observability**
<p>
  <img src="https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white" alt="Prometheus"/>
  <img src="https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white" alt="Grafana"/>
  <img src="https://img.shields.io/badge/Grafana%20Loki-F46800?style=for-the-badge&logo=grafana&logoColor=white" alt="Loki"/>
  <img src="https://img.shields.io/badge/OpenTelemetry-425CC7?style=for-the-badge&logo=opentelemetry&logoColor=white" alt="OpenTelemetry"/>
</p>

---

## 📈 GitHub Stats

<p align="center">
  <img height="170" src="https://github-readme-streak-stats.herokuapp.com/?user=jason-te-sde&theme=gruvbox_light&hide_border=true&date_format=M%20j%5B%2C%20Y%5D" alt="GitHub Streak"/>
</p>
<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=jason-te-sde&theme=zenburn" alt="GitHub Profile Summary Card" />
</p>

## 🐍 Contribution Snake

<picture>
  <source media="(prefers-color-scheme: dark)"  srcset="https://raw.githubusercontent.com/jason-te-sde/jason-te-sde/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/jason-te-sde/jason-te-sde/output/github-snake.svg" />
  <img alt="github-snake" src="https://raw.githubusercontent.com/jason-te-sde/jason-te-sde/output/github-snake.svg" />
</picture>

<!-- ============ Footer wave ============ -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:4A00E0,100:8E2DE2&height=100&section=footer" width="100%"/>
</p>
