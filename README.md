<h1 align="center">Hi 👋, I'm Yash Doke</h1>

<p align="center">
  <b>AI Systems • LLM Infrastructure • Multi-Agent Learning • Robotics</b><br>
  Computer Engineering @ SPPU | CGPA: 9.34/10
</p>

<p align="center">
  I build intelligent systems that connect <b>research ideas</b> with <b>practical deployment</b>.
</p>

---

## About Me

I work on long-horizon language systems, reasoning evaluation, retrieval and memory architectures, and applied AI systems that can move from experimentation to production.

My focus areas include:
- hierarchical memory for LLMs
- reasoning evaluation and fine-tuning
- computer vision and deepfake detection
- robotics, navigation, and reinforcement learning
- production ML systems and data-driven automation

---

## Research & Core Systems

### HierMem — Hierarchical Context Management for LLMs
`Python` `Ollama` `ChromaDB` `nomic-embed-text`

Built an OS-inspired paged memory system with L0–L3 hierarchy: Topic Index → Summaries → Embeddings → Raw Turns. Designed for long-horizon conversations with adaptive token usage.

- Achieved **8.4/10** and **8.7/10** adherence scores on constraint-tracking benchmarks.
- Outperformed RAG and RAG+Summary baselines on late-turn compliance.
- Reduced token usage through adaptive passthrough and hierarchical paging.
- Cut vector storage costs through structured memory layering.

### LLM Reasoning Pipeline
`PyTorch` `Hugging Face TRL` `QLoRA` `PEFT` `GGUF` `Ollama`

Developed a reasoning evaluation pipeline for diagnosing step-level failures in large language models.

- Fine-tuned Qwen 2.5 3B to reduce multi-step reasoning failures.
- Built ground-truth backtracking and error propagation analysis for CoT traces.
- Quantized models to **GGUF** for local inference through Ollama.
- Created synthetic structured training data for step-by-step reasoning tasks.

### AI-Generated Video Detection
`PyTorch` `SigLIP` `Transformer` `Continual Learning`

Engineered a deepfake detection system designed to stay robust across domains and changing video distributions.

- Reached **92% AUC-ROC** across cross-domain benchmarks.
- Used replay buffers, bottleneck adapters, and distillation to reduce catastrophic forgetting.
- Built an automated frame-sampling and block-aggregation pipeline for verification.

---

### ABU Robocon 2026 — Autonomous Navigation Stack
`NVIDIA Isaac Sim` `Path Planning` `Python` `MATLAB` `PPO`

Lead architect for the autonomous navigation system in the ABU Robocon 2026 competition.

- Implemented modified A* planning for partial observability and dynamic obstacles.
- Deployed PPO-based control with reward shaping for rule-compliant navigation.
- Validated logic in high-fidelity simulation before real-world integration.

---

## Tech Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,cpp,java,js,ts,pytorch,tensorflow,fastapi,flask,nextjs,react,mysql,mongodb,postgres,docker,linux,git,aws" />
</p>

<p align="center">
  <b>Transformers • QLoRA/PEFT • Reinforcement Learning • Computer Vision • AI Agents • ROS2 • NVIDIA Isaac Sim</b>
</p>

---

## Affiliations

- **ACM Student Chapter** — Marketing Head
- **Team Vulcans Robotics** — Software Team

---

## Contact

<p align="center">
  <a href="mailto:yashdoke215@gmail.com">Email</a> •
  <a href="https://linkedin.com/in/yash-doke">LinkedIn</a> •
  <a href="https://github.com/yashdoke7">GitHub</a>
</p>
