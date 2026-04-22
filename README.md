<h1 align="center">Hi 👋, I'm Yash Doke</h1>

<p align="center">
  <b>AI Systems • LLM Infrastructure • Multi-Agent Learning • Robotics</b><br>
  Computer Engineering @ SPPU | CGPA: 9.34/10
</p>

<p align="center">
  Designing intelligent systems that connect <b>research</b> with <b>practical deployment</b>.
</p>

---

## About Me

I work on long-horizon language systems, reasoning evaluation, retrieval and memory architectures, and applied AI systems that move from experimentation to production.

My current interests include:
- hierarchical memory for LLMs
- reasoning evaluation and fine-tuning
- production ML systems
- computer vision and deepfake detection
- robotics, navigation, and reinforcement learning

---

## Research & Core Systems

### 🚀 HierMem: OS-Inspired Memory for Infinite Conversations
`Pytorch` `Ollama` `ChromaDB` `LiteLLM` `RAG`
HierMem is a research-grade context management system that treats LLM memory like a paged OS hierarchy. It solves the "context window wall" by prioritizing smart pruning over raw token dumping.

📈 Performance: Achieved a 4.7x memory compression ratio and 33% lower inference costs without quality loss.
🧠 Intelligence: Maintains a 93.3% constraint survival rate, ensuring the LLM never "forgets" rules in long sessions.
🛠️ Architecture: Features a 4-layer paging system (L0-L3) driven by a stateless Curator Orchestrator agent.
🏆 Benchmarking: Outperformed standard RAG and Raw LLM baselines with a mean judge score of 8.46.

### LLM Reasoning Pipeline — Chain-of-Thought Evaluation
`PyTorch` `Hugging Face TRL` `QLoRA` `PEFT` `GGUF` `Ollama`

Developed a reasoning evaluation pipeline for diagnosing step-level failures in large language models.

- Fine-tuned Qwen 2.5 3B to reduce multi-step reasoning failures.
- Built ground-truth backtracking and error propagation analysis for CoT traces.
- Quantized fine-tuned models to **GGUF** for local inference through Ollama.
- Created a synthetic data pipeline for structured step-by-step reasoning traces.

### AI-Generated Video Detection
`PyTorch` `SigLIP` `Transformer` `Continual Learning`

Engineered a deepfake detection system designed to stay robust across domains and changing video distributions.

- Achieved **92% AUC-ROC** across cross-domain benchmarks.
- Used replay buffers, bottleneck adapters, and distillation to reduce catastrophic forgetting.
- Built an automated frame-sampling and block-aggregation pipeline for verification.

---

## Featured Projects

### ABU Robocon 2026 — Autonomous Navigation Stack
`NVIDIA Isaac Sim` `Path Planning` `Python` `MATLAB` `PPO`

Lead architect for the autonomous navigation system in the ABU Robocon 2026 competition.

- Implemented modified A* planning for partial observability and dynamic obstacles.
- Deployed PPO-based control with reward shaping for rule-compliant navigation.
- Validated logic in simulation before real-world integration.

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
