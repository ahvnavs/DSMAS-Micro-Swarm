@article{dsmas2026,
  title={Architecture of Decentralized Spatial Multi-Agent Systems: Lightweight Swarms, Proximity Routing, and Stigmergic Coordination},
  author={[Abhinav Sharma]},
  year={2026},
  url={[https://github.com/ahvnavs/DSMAS-Micro-Swarm](https://github.com/ahvnav/DSMAS-Micro-Swarm)}
}

# DSMAS: Decentralized Spatial Multi-Agent System

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)
![Status: Prototype](https://img.shields.io/badge/Status-Phase_1_Prototype-orange.svg)

> **A stigmergic, spatially-routed architecture for lightweight LLM swarms operating on fractional edge compute.**

This repository contains the foundational research, proof-of-concept simulation, and open-source infrastructure for **DSMAS**. It demonstrates how thousands of resource-constrained Small Language Models (SLMs) can process complex logic in a decentralized topology without a central orchestrator, utilizing K-Nearest Neighbor (KNN) proximity routing and Conflict-Free Replicated Data Types (CRDTs) for shared memory.

---

## 📖 Table of Contents
- [Core Architecture](#core-architecture)
- [Project Roadmap](#project-roadmap)
- [Micro-Swarm Simulator (Phase 1)](#micro-swarm-simulator)
- [Academic Citation](#academic-citation)
- [Contributing](#contributing)

---

## 🧠 Core Architecture

Current AI paradigms rely on monolithic, gigawatt-consuming cloud architectures. DSMAS inverts this by distributing reasoning across a continuously moving virtual topology. 

1. **Fractional Compute:** Designed for quantized SLMs (e.g., DeepSeek-Distill 1.5B, Llama 3 8B) running on edge devices.
2. **Voronoi Overlay Networks (VON):** Agents establish Spatial Publish-Subscribe (SPS) neighborhoods dynamically without global mapping.
3. **Loop-Free Proximity Routing:** Tasks are mathematically forced forward using Dynamic Source Routing (DSR) exclusion lists and KNN ($k=2$) spatial queries.
4. **Stigmergic Coordination:** Agents communicate indirectly via digital pressure fields and shared CRDT databases, ensuring exponential intelligence compounding without centralized servers.

---

## 🗺️ Project Roadmap

- [x] **Phase 0:** Theoretical Framework & Architectural White Paper
- [ ] **Phase 1: Localized Micro-Swarm Simulation** (Current Focus)
  - Simulating the Voronoi spatial topology natively in Python.
  - Proving DSR loop-prevention mechanics using local LLM inference.
- [ ] **Phase 2: Semantic Memory Integration**
  - Integrating a local CRDT backend to prove shared intelligence compounding across distributed nodes.
- [ ] **Phase 3: Physical Edge Deployment**
  - Porting the swarm to physical IoT arrays (e.g., Raspberry Pi clusters) over MANET.

---

## 🚀 Micro-Swarm Simulator

*(Note: The simulation engine is currently under active development. Installation instructions will be updated upon the v0.1 release).*

### Prerequisites
- Python 3.10+
- [Ollama](https://ollama.com/) (For local, zero-cost SLM inference)

### Quick Start
```bash
# Clone the repository
git clone [https://github.com/YOUR-USERNAME/DSMAS-Micro-Swarm.git](https://github.com/YOUR-USERNAME/DSMAS-Micro-Swarm.git)
cd DSMAS-Micro-Swarm

# Install dependencies
pip install -r requirements.txt

# Run the localized spatial simulation
python src/simulator.py
