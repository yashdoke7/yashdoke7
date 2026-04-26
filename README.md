<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0a1628,100:1a3a8f&height=120&section=header&text=Yash%20Doke&fontSize=42&fontColor=ffffff&fontAlignY=65&animation=fadeIn" width="100%"/>

### AI/ML Engineer · LLM Infrastructure · Robotics · Production ML

[![LinkedIn](https://img.shields.io/badge/LinkedIn-yash--doke-0a66c2?style=flat-square&logo=linkedin)](https://linkedin.com/in/yash-doke)
[![PyPI](https://img.shields.io/badge/PyPI-llm--hiermem-3775a9?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/llm-hiermem/)
[![HuggingFace](https://img.shields.io/badge/🤗%20Hugging%20Face-yashdoke7-ff9d00?style=flat-square)](https://huggingface.co/yashdoke7)
[![Email](https://img.shields.io/badge/Email-yashdoke215@gmail.com-ea4335?style=flat-square&logo=gmail&logoColor=white)](mailto:yashdoke215@gmail.com)
![Profile views](https://komarev.com/ghpvc/?username=yashdoke7&color=4a9eff&style=flat-square&label=Profile+Views)

*Rising 4th-year BE Computer Engineering @ PESMCOE, SPPU · CGPA 9.34/10*

*Building AI systems that work outside the lab — from research prototype to deployed package.*

</div>

---

## 🧠 Flagship Research — HierMem

> **LLMs forget. HierMem fixes that.**

HierMem is an OS-inspired hierarchical paged memory architecture for long-horizon LLM conversations. Inspired by virtual memory paging — the same design that lets your computer run programs larger than physical RAM — it uses a stateless curator agent, a priority-tagged constraint store, and a 4-level memory hierarchy (L0→L3) to prevent context degradation, constraint forgetting, and hallucination.

```
┌─────────────────────────────────────────────────────────────┐
│  Curator (~1000 tokens, constant)  →  reads L0 index only   │
│  Retrieval  →  KEYWORD / SEMANTIC / HIERARCHICAL / HYBRID   │
│  Assembler  →  4-zone attention-optimised context           │
│  Main LLM   →  generates from bounded ~6000-token budget    │
│  Post-Proc  →  extracts constraints, updates L0→L3 archive  │
└─────────────────────────────────────────────────────────────┘
```

| Metric | Result |
|--------|--------|
| Memory compression ratio | **4.7×** vs raw context |
| Constraint survival rate | **93.3%** over long sessions |
| LLM-as-Judge score | **8.4–8.7 / 10** (vs 5.4–7.6 baselines) |
| Outperforms | RAG · RAG+Summary · MemGPT-style · Raw LLM |

[![GitHub](https://img.shields.io/badge/GitHub-llm--hiermem-181717?style=flat-square&logo=github)](https://github.com/yashdoke7/llm-hiermem)
[![PyPI](https://img.shields.io/badge/PyPI-live-3775a9?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/llm-hiermem/)
[![Dataset](https://img.shields.io/badge/HuggingFace-dataset-ff9d00?style=flat-square)](https://huggingface.co/yashdoke7)

---

## 🔬 Projects

<table>
<tr>
<td width="50%" valign="top">

### [LLM Reasoning Pipeline](https://github.com/yashdoke7/llm-reasoning-pipeline)
Step-level diagnosis and targeted fine-tuning for LLM reasoning failures — diagnoses *where* models fail, not just *if* they fail.
- Fine-tuned Qwen 2.5 3B with QLoRA 4-bit
- **63% reduction** in step-level failure rate
- Ground-truth backtracking + error propagation analysis
- Runs fully local via llama.cpp — zero API cost

`PyTorch` `QLoRA` `PEFT` `GGUF` `Ollama`

</td>
<td width="50%" valign="top">

### [AI-Generated Video Detection](https://github.com/yashdoke7/ai-generated-video-detection)
Deepfake detection pipeline designed to stay robust across domains and changing distributions.
- **92% AUC-ROC** across DFDC, CelebDF, WildDeepfake
- SigLIP transformer embeddings + blockwise frame representation
- Continual learning via replay buffers + knowledge distillation
- Prevents catastrophic forgetting across dataset shifts

`PyTorch` `SigLIP` `Transformers` `Continual Learning`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### [Fraud Detection System](https://github.com/yashdoke7/FraudDetection)
Production-grade fraud detection — not a demo, a deployed pipeline.
- **96.2% accuracy**, **0.92 AUC-ROC**
- Processes **50K+ transactions/day**
- XGBoost + neural networks with advanced feature engineering
- Real-time FastAPI classification with geolocation tracking

`XGBoost` `FastAPI` `Neural Networks` `sklearn`

</td>
<td width="50%" valign="top">

### [Self-Evolving Multi-Agent Governance](https://github.com/Harsh-4210/Self_Evolving_Multi_Agent_Governance)
Decentralised agents that negotiate and evolve decision policies autonomously.
- PPO + quadratic voting with reputation weighting
- Agents negotiate rule proposals in a simulated digital economy
- PostgreSQL logging of governance events and adaptive reward strategies
- Delivered as a functional 24-hour hackathon proof-of-concept

`Ray RLlib` `PettingZoo` `PPO` `PostgreSQL`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### [AquaIntel](https://github.com/yashdoke7/AquaIntel) ⭐ 7
Ship routing system with live weather integration.
- Enhanced A* algorithm with adaptive grid weighting
- Integrates wind, depth risk, and fuel efficiency in real-time
- **Reduced route update time from 3.6h → 36 minutes** (6×)
- Full-stack with route visualisation via Leaflet.js

`TypeScript` `A* Algorithm` `OpenWeatherMap` `Leaflet.js`

</td>
<td width="50%" valign="top">

### [NutriSense](https://github.com/yashdoke7/nutrisense)
AI health platform built around generative AI orchestration.
- Gemini 2.0 Flash for multimodal food recognition
- NLP-driven dietary Q&A + longitudinal health trend analysis
- Serverless GCP backend with Firestore real-time persistence
- WCAG 2.1 accessible UI with Firebase Auth + server-side token validation

`Gemini API` `Google Cloud` `Firebase` `Vanilla CSS`

</td>
</tr>
</table>

---

## 🤖 Robotics — ABU Robocon 2026

**Team Vulcans · Software & AI Lead**

Building the autonomous navigation and AI stack for PESMCOE's entry in ABU Robocon 2026.

- Modified A\* planning for partial observability and dynamic obstacles
- PPO-based control with reward shaping for rule-compliant navigation
- ROS2 architecture + Gazebo simulation environments
- Validated in NVIDIA Isaac Sim before real-world hardware integration

`ROS2` `NVIDIA Isaac Sim` `Gazebo` `PPO` `Python` `MATLAB`

---

## ⚙️ Tech Stack

```python
LANGUAGES   = ["Python", "TypeScript", "C++", "SQL", "MATLAB"]

ML_AI       = ["PyTorch", "Hugging Face TRL", "QLoRA/PEFT", "LiteLLM",
               "LangChain", "XGBoost", "sentence-transformers", "SigLIP"]

LLM_INFRA   = ["Ollama", "llama.cpp", "GGUF", "ChromaDB",
               "RAG pipelines", "LLM-as-Judge evaluation"]

ROBOTICS    = ["ROS2", "NVIDIA Isaac Sim", "Gazebo", "A*", "PPO", "Ray RLlib"]

BACKEND     = ["FastAPI", "Flask", "PostgreSQL", "MongoDB", "Firebase"]

CLOUD       = ["Google Cloud Platform", "AWS"]

TOOLS       = ["Git", "Docker", "pytest", "Streamlit", "Weights & Biases"]
```

---

## 📊 GitHub Stats

<div align="center">

<img height="180" src="https://github-readme-stats.vercel.app/api?username=yashdoke7&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=4a9eff&icon_color=4a9eff&text_color=c9d1d9&include_all_commits=true&count_private=true" />
<img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=yashdoke7&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=4a9eff&text_color=c9d1d9&langs_count=8" />

</div>

<div align="center">

<img src="https://github-readme-streak-stats.herokuapp.com?user=yashdoke7&theme=github-dark-blue&hide_border=true&background=0d1117&stroke=4a9eff&ring=4a9eff&fire=ff6b35&currStreakLabel=4a9eff&dates=8b949e" />

</div>

<div align="center">

<img src="https://github-profile-trophy.vercel.app/?username=yashdoke7&theme=algolia&no-frame=true&no-bg=true&column=6&margin-w=8" />

</div>

---

## 📈 Contribution Activity

<img src="https://github-readme-activity-graph.vercel.app/graph?username=yashdoke7&bg_color=0d1117&color=4a9eff&line=1a3a8f&point=4a9eff&area=true&area_color=1a3a8f&hide_border=true" width="100%"/>

---

## 🎯 Currently

- 🔬 Extending HierMem — Needle-in-a-Haystack and multi-step reasoning benchmarks
- 🤖 Autonomous navigation stack for ABU Robocon 2026
- 📖 Rising 4th year BE CS · **Open to research internships & AI engineering roles (2025–26)**
- 📬 Reach me: [yashdoke215@gmail.com](mailto:yashdoke215@gmail.com) · [linkedin.com/in/yash-doke](https://linkedin.com/in/yash-doke)

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a3a8f,100:0a1628&height=80&section=footer" width="100%"/>

*"The gap between research and production is where I work."*

![Profile views](https://komarev.com/ghpvc/?username=yashdoke7&color=4a9eff&style=flat-square&label=Profile+Views)

</div>
