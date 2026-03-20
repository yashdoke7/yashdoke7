<h1 align="center">Hi 👋, I'm Yash Doke</h1>

<p align="center">
<b>AI Systems • LLM Infrastructure • Multi-Agent Learning • Robotics</b><br>
Computer Engineering @ SPPU | CGPA: 9.34/10
</p>

<p align="center">
<i>Designing intelligent systems that bridge the gap from <b>research concepts → scalable deployment</b>.</i>
</p>

---

## 🔬 Research & Core Systems

### 🧠 HierMem — Hierarchical Context Management for LLMs
`Python` `Ollama` `ChromaDB` `nomic-embed-text`

Architected an OS-inspired paged memory system (L0–L3: Topic Index → Summaries → Embeddings → Raw Turns) enabling infinite context scaling with **adaptive token consumption (~6k tokens/turn)**.
- **3.3× Higher Compliance:** Outperformed RAG baselines (6.67 vs 2.00/10) in constraint-heavy reasoning tasks via a dedicated constraint store.
- **Efficiency at Scale:** Achieved a **67% pairwise win rate** against full-context (32k) baselines while reducing token usage by **~25%**.
- **Resource Optimization:** Cut vector storage costs by **50%** compared to standard RAG at equivalent retrieval performance.
- **Key Insight:** Identified the *RAG Compliance Paradox*—demonstrating that 100% keyword retrieval accuracy often yields low (2.0/10) reasoning adherence.

### 🔬 LLM Reasoning Pipeline — Chain-of-Thought Evaluation
`PyTorch` `Hugging Face TRL` `QLoRA` `PEFT` `GGUF` `Ollama`

Developed a granular evaluation pipeline for diagnosing *step-level* reasoning failures in Large Language Models.
- **63% Error Reduction:** Fine-tuned Qwen 2.5 3B to drastically reduce reasoning failures on multi-step arithmetic tasks.
- **Deep Diagnostics:** Implemented ground-truth backtracking and error propagation detection to isolate failure points in GSM8K traces.
- **Edge Deployment:** Quantized fine-tuned models to **GGUF** format, enabling zero-cost local inference via Ollama.
- **Automated Data Pipeline:** Built a synthetic data engine to generate structured CoT training traces with step-by-step annotations.

### 🎥 AI-Generated Video Detection
`PyTorch` `SigLIP` `Transformer` `Continual Learning`

Engineered a domain-robust deepfake detection system using continual learning transformers to combat model drift.
- **92% AUC-ROC:** State-of-the-art performance across 8 cross-domain benchmarks (DFDC, Celeb-DF, WildDeepfake, VidProM).
- **Catastrophic Forgetting Mitigation:** Integrated replay buffers, bottleneck adapters, and knowledge distillation to retain performance across diverse datasets.
- **End-to-End Analysis:** Automated frame sampling and block-level aggregation for real-time video verification.

---

## 🚀 Featured Projects

### 🤖 ABU Robocon 2026 — Autonomous Navigation Stack
`NVIDIA Isaac Sim` `Path Planning` `Python` `MATLAB` `PPO`

Lead Architect for the autonomous navigation system in the ABU Robocon 2026 competition.
- **Adaptive Pathfinding:** Implemented a modified A* algorithm for traversal under partial observability, handling dynamic obstacles and terrain changes.
- **Reinforcement Learning:** Deployed PPO agents with structured reward shaping to ensure strict rule compliance during navigation.
- **Simulation-to-Reality:** Validated control logic via high-fidelity physics simulations in NVIDIA Isaac Sim.

### ⚓ Ship Route Optimization
`Geospatial Analysis` `A* Algorithm` `Real-time Data`

Developed a weather-aware navigation system integrating real-time environmental data with a scalable geospatial backend for optimal route planning.

### 💳 Fraud Detection System
`Ensemble Learning` `FastAPI` `Production ML`

Built a production-grade ML pipeline for real-time transaction monitoring, deploying ensemble models via high-throughput FastAPI microservices.

### ⚡ CodeArc
`Repository Mining` `Predictive Modeling` `Git Internals`

Analyzed extensive Git commit histories to model software evolution, training predictive models on the transition patterns from prototype to production code.

---

## 🛠 Tech Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,cpp,java,js,ts,pytorch,tensorflow,fastapi,flask,nextjs,react,mysql,mongodb,postgres,docker,linux,git,aws" />
</p>

<p align="center">
<b>Transformers • QLoRA/PEFT • Reinforcement Learning • Computer Vision • AI Agents • ROS2 • NVIDIA Isaac Sim</b>
</p>

---

## 📌 Affiliations

- **ACM Student Chapter** — Marketing Head  
- **Team Vulcans Robotics** — AI Systems Engineer

---

## 🌐 Connect

<p align="center">
📧 <a href="mailto:yashdoke215@gmail.com">yashdoke215@gmail.com</a> • 
<a href="https://linkedin.com/in/yash-doke">LinkedIn</a> • 
<a href="https://github.com/yashdoke7">GitHub</a>
</p>
