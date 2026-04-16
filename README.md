<div align="center">

# Stephen Junyi Li

**Software Engineer** · Systems · ML · Full-Stack

[![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)](#)
[![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)](#)
[![Go](https://img.shields.io/badge/-Go-00ADD8?style=flat-square&logo=go&logoColor=white)](#)
[![Java](https://img.shields.io/badge/-Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)](#)
[![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=black)](#)
[![Node.js](https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)](#)
[![AWS](https://img.shields.io/badge/-AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)](#)
[![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)](#)
[![Kubernetes](https://img.shields.io/badge/-K8s-326CE5?style=flat-square&logo=kubernetes&logoColor=white)](#)
[![Neo4j](https://img.shields.io/badge/-Neo4j-4581C3?style=flat-square&logo=neo4j&logoColor=white)](#)

</div>

---

### [`MultiAgents4Copilot`](https://github.com/VincentPit/MultiAgents4Copilot) — Multi-Agent AI System for VS Code

A DAG-orchestrated multi-agent system inside VS Code Copilot Chat. Nine specialist agents collaborate through a shared message bus to plan, code, test, and review — mirroring a Meta engineering team.

> Go goroutines for true OS-level parallelism · JSON-RPC bridge to Node.js · Meta-style quality gates (`build → lint → test → diff → self-review`) · Live webview dashboard with per-domain log cards · DAG state-machine with conditional routing and parallel fan-out

---

### [`CSLGraphBuilder`](https://github.com/VincentPit/CSLGraphBuilder) — Biomedical Knowledge Graph Pipeline

Enterprise knowledge graph platform for CSL Behring. Ingests biomedical literature (PubMed, Open Targets, PDFs, web crawls), extracts entities via GPT-4, and persists them into Neo4j with provenance tracking.

> Two-stage LLM dedup (vector pre-filter → LLM confirmation) · Cascading verification (text-match → embedding → LLM) with confidence-based escalation · Conflict detection (INHIBITS vs ACTIVATES) with source trust scoring · FastAPI + Next.js 14 + Docker Compose · 191 tests across 3 tiers

---

### [`StockGang`](https://github.com/VincentPit/StockGang) — A-Share Quantitative Trading Platform

Full-stack quant trading system for A-share markets. Event-driven backtesting, LightGBM ML signals, and paper-trading simulator wired to a Next.js dashboard.

> 5-strategy ensemble (LightGBM, MA Crossover, RSI, MACD, News Sentiment) · 7-layer risk gate (drawdown breaker → position limit → sector cap → VaR) · Causal trace on every screener result · Two-level cache (L1 memory + L2 SQLite) · 307 pytest + 67 Jest tests

---

### [`GraphBuilder`](https://github.com/VincentPit/GraphBuilder) — Enterprise Knowledge Graph Builder

Transforms unstructured content into knowledge graphs using LLM extraction and Neo4j. Domain-driven design with clean layered architecture.

> DDD: domain models → use cases → infrastructure adapters · Async pipeline with task orchestration and exponential-backoff retry · Multi-LLM (OpenAI, Azure OpenAI) with entity dedup and Cypher optimization · Automated migration from legacy scripts

---

### [`Bi_Memit`](https://github.com/VincentPit/Bi_Memit) — Bidirectional Model Editing Framework

Research framework for editing factual knowledge in transformers while maintaining logical consistency in both directions. Extends MEMIT with bidirectional enforcement.

> Forward + reverse edits validated together · Symmetric parameter updates across both pathways · Adaptive threshold controller (96% consistency in high-precision mode) · 23% improvement over unidirectional baselines

---

### [`MAE_SIMP`](https://github.com/VincentPit/MAE_SIMP) — Unified Vision Transformer Framework

Production-ready framework for vision transformer research. MAE, ViT, Image GPT, and Gray2Color with distributed training infrastructure.

> Multi-architecture registry with shared components via factory pattern · Multi-node DDP/NCCL + mixed precision + gradient checkpointing · Docker + K8s deployment with FastAPI serving · MAE-ViT-Huge: 87.8% ImageNet at 632M params

---

<div align="center">
  <img src="https://komarev.com/ghpvc/?username=VincentPit&style=flat-square&color=6366f1&label=visitors" alt="Profile Views" />
</div>
