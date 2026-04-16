<h1 align="center">Hey there 👋, I'm Stephen Junyi Li</h1>

<p align="center">
  <em>Software Engineer — building things that matter</em>
</p>

---

### 🔭 About Me

- 💻 Software Engineer with a passion for building scalable, reliable systems
- 🌱 Always learning and exploring new technologies
- 🤝 Open to collaborating on interesting open-source projects

---

### 🛠️ Tech Stack

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
  <img src="https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white" />
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" />
</p>

---

### 🚀 Featured Projects

#### [`MultiAgents4Copilot`](https://github.com/VincentPit/MultiAgents4Copilot) — Multi-Agent AI System for VS Code
A DAG-orchestrated multi-agent system running inside VS Code Copilot Chat. Nine specialist agents (Supervisor, Planner, Coder Pool, Integrator, Reviewer, etc.) collaborate through a shared message bus to plan, code, test, and review — mirroring how a team of engineers operates at Meta. Key engineering decisions:
- **Go worker goroutines** for true OS-level parallelism across domain coders, with a JSON-RPC bridge back to Node.js — not just `Promise.allSettled`
- **Meta-style quality gates** on every agent: `build → lint → test → diff → self-review` before any code is submitted
- **Live webview dashboard** with per-domain log cards pushed via `postMessage` (single DOM mutations, no flicker)
- **DAG state-machine executor** with conditional routing, parallel fan-out, and 30-min wall-clock guard — no per-agent timeouts

#### [`CSLGraphBuilder`](https://github.com/VincentPit/CSLGraphBuilder) — Biomedical Knowledge Graph Pipeline
Enterprise knowledge graph construction platform for CSL Behring. Ingests biomedical literature (PubMed, Open Targets, PDFs, web crawls), extracts entities/relationships via GPT-4, and persists them into Neo4j with full provenance tracking. Key engineering decisions:
- **Two-stage LLM deduplication**: vector pre-filter (cheap cosine search) followed by LLM confirmation for domain-aware synonym resolution (e.g. "TNF-alpha" ≈ "Tumor Necrosis Factor Alpha")
- **Cascading verification pipeline**: text-match → embedding → LLM, with confidence-based escalation bands — expensive stages only fire when cheap stages are inconclusive
- **Conflict detection** with automatic contradiction identification (INHIBITS vs ACTIVATES) and source trust scoring
- **Full-stack deployment**: FastAPI + Next.js 14 + Docker Compose with human-in-the-loop curation queue (191 tests across 3 tiers)

#### [`StockGang`](https://github.com/VincentPit/StockGang) — A-Share Quantitative Trading Platform
Full-stack quant trading system for Shanghai & Shenzhen A-share markets. Combines an event-driven backtesting engine, LightGBM ML signals, and a paper-trading simulator wired to a Next.js dashboard. Key engineering decisions:
- **5-strategy ensemble** (LightGBM, MA Crossover, RSI, MACD, News Sentiment) with realistic cost modeling (commission + stamp duty + slippage)
- **7-layer risk gate**: market state → throttle → drawdown circuit breaker → position limit → sector exposure → VaR check → cooldown timer
- **Causal trace** shipped with every screener result — factor breakdowns showing exactly why a stock scored the way it did
- **Two-level cache** (in-memory L1 + SQLite L2) with per-type TTLs; background jobs via ThreadPoolExecutor with SQLite write-through (307 pytest + 67 Jest tests)

#### [`GraphBuilder`](https://github.com/VincentPit/GraphBuilder) — Enterprise Knowledge Graph Builder
Transforms unstructured content into knowledge graphs using LLM-powered extraction and Neo4j. Evolved from scripts into a production-grade system with domain-driven design. Key engineering decisions:
- **Domain-Driven Design** with clean layered architecture: domain models → application use cases → infrastructure adapters
- **Async processing pipeline** with task orchestration, dependency management, and intelligent retry with exponential backoff
- **Multi-LLM support** (OpenAI GPT, Azure OpenAI) with entity deduplication via similarity matching and Cypher query optimization
- **Full migration path** from legacy scripts with automated `migrate.py` and backward-compatible configuration loading

#### [`Bi_Memit`](https://github.com/VincentPit/Bi_Memit) — Bidirectional Model Editing Framework
Research framework for editing factual knowledge in transformer models while maintaining logical consistency in both directions. Extends MEMIT with bidirectional consistency enforcement. Key engineering decisions:
- **Bidirectional consistency tracking** — forward edit "Paris → Germany" and reverse "Germany's capital → Paris" are validated together, solving the fundamental one-direction problem in model editing
- **Symmetric parameter updates** that propagate changes to both forward and reverse pathways simultaneously
- **Adaptive threshold controller** that self-tunes consistency parameters per edit batch (96% consistency in high-precision mode)
- **Iterative refinement loop** that progressively improves consistency until convergence, achieving 23% improvement over unidirectional baselines

#### [`MAE_SIMP`](https://github.com/VincentPit/MAE_SIMP) — Unified Vision Transformer Framework
Production-ready framework for vision transformer research. Implements MAE, ViT, Image GPT, and Gray2Color architectures with distributed training infrastructure. Key engineering decisions:
- **Multi-architecture registry** — MAE, ViT, ImGPT, and Gray2Color share reusable components (attention, embeddings, layers) via a factory pattern
- **Distributed training** with multi-node DDP/NCCL, mixed precision, gradient checkpointing, and SLURM HPC integration
- **Production deployment** via Docker + Kubernetes manifests with FastAPI model serving and auto-scaling
- **MAE-ViT-Huge** achieving 87.8% ImageNet accuracy at 632M parameters with configurable masking strategies

---

### 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=VincentPit&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="Top Languages" height="165" />
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=VincentPit&theme=tokyo-night&hide_border=true&area=true" alt="Contribution Graph" />
</p>

---

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=VincentPit&style=flat-square&color=6366f1" alt="Profile Views" />
</p>
