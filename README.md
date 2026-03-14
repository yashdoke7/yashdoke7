<h1 align="center">Hi 👋, I'm Yash Doke</h1>

<p align="center">
AI Systems • LLM Infrastructure • Multi-Agent Learning • Robotics <br>
Computer Engineering @ SPPU | CGPA: 9.34/10
</p>

<p align="center">
Designing intelligent systems that move from <b>research ideas → real-world deployment</b>.
</p>

---

## 🔬 Research & Core Systems

### 🧠 HierMem — Hierarchical Context Management for LLMs
`Python` `Ollama` `ChromaDB` `nomic-embed-text`

OS-inspired hierarchical paged memory system (L0–L3: topic index → segment summaries → semantic embeddings → raw turns) with a dedicated constraint store for long-context LLM reasoning.
- **3.3× higher constraint compliance** than RAG (LLM-as-judge: 6.67 vs 2.00/10)
- **67% pairwise win rate** over all baselines on Qwen 2.5 14B
- **50% lower vector storage** than RAG at equivalent API cost per conversation
- Discovered the *RAG compliance paradox* — 100% keyword accuracy yet 2.0/10 adherence score
- LLM-based curator for dynamic context assembly within a fixed token budget with adaptive passthrough mode

### 🔬 LLM Reasoning Pipeline
`PyTorch` `Hugging Face TRL` `QLoRA` `PEFT` `GGUF` `Ollama`

Step-level chain-of-thought evaluation framework identifying *where* LLMs fail, with targeted fine-tuning.
- **63% reduction** in reasoning failure rate on multi-step arithmetic tasks (Qwen 2.5 3B)
- Step-level CoT evaluation with ground-truth backtracking and error propagation detection across GSM8K
- Quantized fine-tuned model to **GGUF** for zero-cost local inference via Ollama
- Automated dataset generation pipeline producing structured CoT training traces with step-by-step annotations

### 🎥 AI-Generated Video Detection
`PyTorch` `SigLIP` `Transformer` `Continual Learning`

Continual-learning deepfake detection pipeline using transformer embeddings with domain robustness.
- **92% AUC-ROC** across 8 cross-dataset benchmarks (DFDC, Celeb-DF, WildDeepfake, VidProM)
- Replay buffers, bottleneck adapters, and knowledge distillation to mitigate catastrophic forgetting
- Automated frame sampling and block-level aggregation for end-to-end video analysis

---

## 🚀 Featured Projects

### 🤖 ABU Robocon 2026 — Robotics AI System
`NVIDIA Isaac Sim` `Modified A*` `Python` `MATLAB` `PPO`

Autonomous robot navigation system for the ABU Robocon 2026 competition.
- Modified A* algorithm for traversal under partial observability with obstacle avoidance and step climbing
- PPO-based reinforcement learning with structured reward shaping for rule compliance
- Physics-accurate simulation validation in NVIDIA Isaac Sim

### ⚓ Ship Route Optimization
Weather-aware A* navigation system integrating real-time environmental data  
with scalable geospatial backend and visualization dashboard.

### 💳 Fraud Detection System
Production-style ML pipeline for real-time transaction monitoring  
using ensemble learning and FastAPI inference services.

### ⚡ CodeArc
Mining Git commit histories to learn how software evolves — training models  
on the transition from prototype → production systems.

---

## 🛠 Tech Stack

<p align="center">

<img src="https://skillicons.dev/icons?i=python,cpp,java,js,ts,pytorch,tensorflow,fastapi,flask,nextjs,react,mysql,mongodb,postgres,docker,linux,git,aws" />

</p>

<p align="center">
Transformers • QLoRA/PEFT • Reinforcement Learning • Computer Vision • AI Agents • ROS2 • NVIDIA Isaac Sim
</p>

---

## 📌 Affiliations

- **ACM Student Chapter** — Marketing Head  
- **Team Vulcans Robotics** — AI Systems

---

## 🌐 Connect

<p align="center">
📧 yashdoke215@gmail.com • 
<a href="https://linkedin.com/in/yash-doke">LinkedIn</a> • 
<a href="https://github.com/yashdoke7">GitHub</a>
</p>
